# Google Sheets Entegrasyonu Kurulum Rehberi

Bu rehber, araştırma asistanlığı başvuru formunuzun Google Sheets ile entegrasyonunu nasıl kuracağınızı açıklar.

## Adım 1: Google Sheets Oluşturma

1. [Google Sheets](https://sheets.google.com) adresine gidin
2. Yeni bir elektronik tablo oluşturun
3. İlk satıra şu başlıkları ekleyin (A1'den başlayarak):

```
Tarih | Ad Soyad | E-posta | Telefon | Üniversite | Bölüm | Eğitim Seviyesi | Yıl | Araştırma İlgi Alanları | CV Dosya Adı | CV Linki
```

## Adım 2: Google Apps Script Oluşturma

1. Google Sheets dosyanızda `Uzantılar` > `Apps Script` menüsüne tıklayın
2. Aşağıdaki kodu `Code.gs` dosyasına yapıştırın:

```javascript
function doPost(e) {
  try {
    // Aktif elektronik tabloyu ve sayfayı al
    const sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
    
    // Form verilerini al
    const params = e.parameter;
    
    // CV dosyası varsa Google Drive'a yükle
    let cvDriveLink = '';
    if (params.cv_data && params.cv_name) {
      cvDriveLink = uploadToGoogleDrive(params.cv_data, params.cv_name, params.cv_type);
    }
    
    // Veriyi sayfaya ekle
    const rowData = [
      params.timestamp || new Date().toLocaleString('tr-TR'),
      params.fullName || '',
      params.email || '',
      params.phone || '',
      params.university || '',
      params.major || '',
      params.degree || '',
      params.year || '',
      params.research_interest || '',
      params.cv_name || '',
      cvDriveLink
    ];
    
    sheet.appendRow(rowData);
    
    // E-posta bildirimi gönder (isteğe bağlı)
    sendEmailNotification(params);
    
    // Başarılı yanıt döndür
    return ContentService
      .createTextOutput(JSON.stringify({
        status: 'success',
        message: 'Başvuru başarıyla kaydedildi'
      }))
      .setMimeType(ContentService.MimeType.JSON);
      
  } catch (error) {
    console.error('Error:', error);
    
    // Hata yanıtı döndür
    return ContentService
      .createTextOutput(JSON.stringify({
        status: 'error',
        message: 'Başvuru kaydedilirken hata oluştu'
      }))
      .setMimeType(ContentService.MimeType.JSON);
  }
}

function uploadToGoogleDrive(base64Data, fileName, mimeType) {
  try {
    // Base64 verisini blob'a çevir
    const decodedData = Utilities.base64Decode(base64Data);
    const blob = Utilities.newBlob(decodedData, mimeType, fileName);
    
    // CV'ler için klasör oluştur (yoksa)
    const folders = DriveApp.getFoldersByName('Araştırma Asistanlığı Başvuruları');
    let folder;
    if (folders.hasNext()) {
      folder = folders.next();
    } else {
      folder = DriveApp.createFolder('Araştırma Asistanlığı Başvuruları');
    }
    
    // Dosyayı yükle
    const file = folder.createFile(blob);
    
    // Dosyayı herkese açık yap (isteğe bağlı)
    file.setSharing(DriveApp.Access.ANYONE_WITH_LINK, DriveApp.Permission.VIEW);
    
    return file.getUrl();
    
  } catch (error) {
    console.error('Drive upload error:', error);
    return 'CV yüklenemedi';
  }
}

function sendEmailNotification(params) {
  try {
    // E-posta adresinizi buraya yazın
    const YOUR_EMAIL = 'your-email@example.com';
    
    const subject = 'Yeni Araştırma Asistanlığı Başvurusu';
    const body = `
Yeni bir araştırma asistanlığı başvurusu alındı:

Ad Soyad: ${params.fullName}
E-posta: ${params.email}
Telefon: ${params.phone}
Üniversite: ${params.university}
Bölüm: ${params.major}
Eğitim Seviyesi: ${params.degree}
Yıl: ${params.year}

Araştırma İlgi Alanları:
${params.research_interest}

Başvuru Tarihi: ${params.timestamp}

Google Sheets'i kontrol etmek için: ${SpreadsheetApp.getActiveSpreadsheet().getUrl()}
    `;
    
    MailApp.sendEmail(YOUR_EMAIL, subject, body);
    
  } catch (error) {
    console.error('Email notification error:', error);
  }
}

function doGet() {
  return ContentService
    .createTextOutput('Google Apps Script çalışıyor!')
    .setMimeType(ContentService.MimeType.TEXT);
}
```

## Adım 3: Apps Script'i Yayınlama

1. Apps Script editöründe `Dağıt` > `Yeni dağıtım` butonuna tıklayın
2. `Tür` olarak `Web uygulaması`'nı seçin
3. `Şu kişi olarak yürüt`: `Ben` seçin
4. `Erişim izni olan kişiler`: `Herkes` seçin
5. `Dağıt` butonuna tıklayın
6. İzinleri onaylayın
7. Verilen **Web App URL**'sini kopyalayın

## Adım 4: Form'da URL'yi Güncelleme

1. `content/application.md` dosyasında şu satırı bulun:
```javascript
const GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec';
```

2. `YOUR_SCRIPT_ID` kısmını Apps Script'ten aldığınız URL ile değiştirin.

## Adım 5: E-posta Bildirimini Ayarlama (İsteğe Bağlı)

`sendEmailNotification` fonksiyonundaki `YOUR_EMAIL` değişkenini kendi e-posta adresinizle değiştirin:

```javascript
const YOUR_EMAIL = 'fatih.kansoy@example.com';
```

## Test Etme

1. Formu test etmek için bir deneme başvurusu gönderin
2. Google Sheets'te verinin kaydedildiğini kontrol edin
3. CV dosyasının Google Drive'a yüklendiğini kontrol edin
4. E-posta bildirimi geldiğini kontrol edin

## Güvenlik Notları

- Google Apps Script otomatik olarak CORS (Cross-Origin Resource Sharing) destekler
- Dosyalar Google Drive'da güvenli şekilde saklanır
- Form verileri Google Sheets'te şifrelenir
- E-posta bildirimleri Gmail üzerinden güvenli şekilde gönderilir

## Sorun Giderme

### Form gönderilmiyor:
- Apps Script URL'sinin doğru olduğundan emin olun
- Web uygulamasının "Herkes" erişimine açık olduğundan emin olun

### CV yüklenmiyor:
- Dosya boyutunun 5MB'dan küçük olduğundan emin olun
- Google Drive'da yeterli alanınız olduğundan emin olun

### E-posta gelmiyor:
- E-posta adresinin doğru olduğundan emin olun
- Gmail spam klasörünü kontrol edin

## Özelleştirme Seçenekleri

### Ek alanlar eklemek:
1. Google Sheets'e yeni sütunlar ekleyin
2. Form'a yeni input alanları ekleyin
3. Apps Script'te `rowData` array'ine yeni alanları ekleyin

### Otomatik e-posta yanıtı:
Başvuru sahiplerine otomatik onay e-postası göndermek için `sendEmailNotification` fonksiyonunu genişletebilirsiniz.

### Dosya organizasyonu:
CV dosyalarını tarih veya bölüme göre klasörlere ayırmak için `uploadToGoogleDrive` fonksiyonunu özelleştirebilirsiniz. 