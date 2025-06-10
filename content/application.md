---
title: "Araştırma Asistanlığı Başvurusu"
date: 2025-01-21
draft: false
description: "Araştırma asistanlığı pozisyonu için başvuru yapın"
showDate: false
showAuthor: false
showReadingTime: false
showEdit: false
showTableOfContents: false
---

<div class="max-w-4xl mx-auto bg-white dark:bg-neutral-800 rounded-lg shadow-lg p-8">
  
  <!-- Form Header -->
  <div class="text-center mb-8">
    <!-- <h1 class="text-3xl font-bold text-neutral-800 dark:text-neutral-100 mb-4">Research Assistantship Application</h1> -->
    <p class="text-neutral-600 dark:text-neutral-300">Araştırma asistanlığı pozisyonu için aşağıdaki formu doldurunuz.</p>
  </div>

  <!-- Success Message (Hidden by default) -->
  <div id="successMessage" class="hidden mb-6 p-4 bg-green-100 dark:bg-green-900 border border-green-400 dark:border-green-600 text-green-700 dark:text-green-300 rounded-lg">
    <div class="flex items-center">
      <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path>
      </svg>
      <span><strong>Başvurunuz başarıyla gönderildi!</strong> En kısa sürede size dönüş yapacağız.</span>
    </div>
  </div>

  <!-- Error Message (Hidden by default) -->
  <div id="errorMessage" class="hidden mb-6 p-4 bg-red-100 dark:bg-red-900 border border-red-400 dark:border-red-600 text-red-700 dark:text-red-300 rounded-lg">
    <div class="flex items-center">
      <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"></path>
      </svg>
      <span><strong>Hata!</strong> Başvuru gönderilirken bir sorun oluştu. Lütfen tekrar deneyiniz.</span>
    </div>
  </div>

  <!-- Loading Spinner (Hidden by default) -->
  <div id="loadingSpinner" class="hidden mb-6 p-4 text-center">
    <div class="inline-flex items-center px-4 py-2 font-semibold leading-6 text-sm shadow rounded-md text-blue-500 bg-blue-100 dark:bg-blue-900 dark:text-blue-300">
      <svg class="animate-spin -ml-1 mr-3 h-5 w-5 text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
        <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
        <path class="opacity-75" fill="currentColor" d="m4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
      </svg>
      Başvurunuz gönderiliyor...
    </div>
  </div>

  <!-- Application Form -->
  <form id="applicationForm" class="space-y-8">
    
<!-- Basic Information Section -->
<div class="bg-neutral-50 dark:bg-neutral-700 rounded-lg p-6">
      <div class="flex items-center mb-6">
        <div class="bg-blue-100 dark:bg-blue-900 p-2 rounded-full mr-3">
          <svg class="w-6 h-6 text-blue-600 dark:text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"></path>
          </svg>
        </div>
        <h2 class="text-xl font-semibold text-neutral-800 dark:text-neutral-100">Temel Bilgiler</h2>
      </div>
      
 <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Full Name -->
        <div>
          <label for="fullName" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            Ad Soyad <span class="text-red-500">*</span>
          </label>
          <input 
            type="text" 
            id="fullName" 
            name="fullName" 
            required
            placeholder="örn., Ahmet Yılmaz"
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
          >
        </div>
        
<!-- Email Address -->
 <div>
          <label for="email" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            E-posta Adresi <span class="text-red-500">*</span>
          </label>
          <input 
            type="email" 
            id="email" 
            name="email" 
            required
            placeholder="örn., ahmet.yilmaz@universite.edu.tr"
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
          >
        </div>
      </div>
      
<!-- Phone Number -->
<div class="mt-6">
        <label for="phone" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
          Telefon Numarası (İsteğe Bağlı)
        </label>
        <input 
          type="tel" 
          id="phone" 
          name="phone"
          placeholder="örn., (0212) 123-4567"
          class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
        >
      </div>
    </div>

<!-- Educational Background Section -->
 <div class="bg-neutral-50 dark:bg-neutral-700 rounded-lg p-6">
      <div class="flex items-center mb-6">
        <div class="bg-green-100 dark:bg-green-900 p-2 rounded-full mr-3">
          <svg class="w-6 h-6 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5z"></path>
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path>
          </svg>
        </div>
        <h2 class="text-xl font-semibold text-neutral-800 dark:text-neutral-100">Eğitim Geçmişi</h2>
      </div>
      
<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- School/University -->
        <div>
          <label for="university" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            Okul/Üniversite <span class="text-red-500">*</span>
          </label>
          <input 
            type="text" 
            id="university" 
            name="university" 
            required
            placeholder="örn., İstanbul Üniversitesi"
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
          >
        </div>
        
   <!-- Department/Major -->
 <div>
          <label for="major" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            Bölüm/Ana Dal <span class="text-red-500">*</span>
          </label>
          <input 
            type="text" 
            id="major" 
            name="major" 
            required
            placeholder="örn., İktisat"
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
          >
        </div>
      </div>
      
<div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-6">
        <!-- Degree Level -->
        <div>
          <label for="degree" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            Mevcut Eğitim Seviyesi <span class="text-red-500">*</span>
          </label>
          <select 
            id="degree" 
            name="degree" 
            required
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100"
          >
            <option value="">Eğitim seviyenizi seçiniz</option>
            <option value="lisans">Lisans</option>
            <option value="yuksek_lisans">Yüksek Lisans</option>
            <option value="doktora">Doktora</option>
            <option value="doktora_sonrasi">Doktora Sonrası</option>
          </select>
        </div>
        
<!-- Year of Study -->
 <div>
          <label for="year" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
            Kaçıncı Yıl <span class="text-red-500">*</span>
          </label>
          <select 
            id="year" 
            name="year" 
            required
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100"
          >
            <option value="">Yılı seçiniz</option>
            <option value="1">1. Yıl</option>
            <option value="2">2. Yıl</option>
            <option value="3">3. Yıl</option>
            <option value="4">4. Yıl</option>
            <option value="5">5. Yıl</option>
            <option value="6+">6+ Yıl</option>
          </select>
        </div>
      </div>
    </div>

<!-- Research Interest Section -->
 <div class="bg-neutral-50 dark:bg-neutral-700 rounded-lg p-6">
      <div class="flex items-center mb-6">
        <div class="bg-purple-100 dark:bg-purple-900 p-2 rounded-full mr-3">
          <svg class="w-6 h-6 text-purple-600 dark:text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
          </svg>
        </div>
        <h2 class="text-xl font-semibold text-neutral-800 dark:text-neutral-100">Araştırma İlgi Alanları</h2>
      </div>
      
 <div>
        <label for="research_interest" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
          Araştırma İlgi Alanlarınızın Kısa Açıklaması <span class="text-red-500">*</span>
        </label>
        <textarea 
          id="research_interest" 
          name="research_interest" 
          required
          rows="4"
          placeholder="Lütfen araştırma ilgi alanlarınızı ve bunların bizim araştırma alanlarımızla nasıl örtüştüğünü açıklayınız..."
          class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 placeholder-neutral-500 dark:placeholder-neutral-400"
        ></textarea>
      </div>
    </div>

<!-- CV Upload Section -->
<div class="bg-neutral-50 dark:bg-neutral-700 rounded-lg p-6">
      <div class="flex items-center mb-6">
        <div class="bg-orange-100 dark:bg-orange-900 p-2 rounded-full mr-3">
          <svg class="w-6 h-6 text-orange-600 dark:text-orange-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
          </svg>
        </div>
        <h2 class="text-xl font-semibold text-neutral-800 dark:text-neutral-100">CV Yükleme</h2>
      </div>
      
 <div>
        <label for="cv" class="block text-sm font-medium text-neutral-700 dark:text-neutral-300 mb-2">
          CV Yükleyin (PDF veya Word, max 5MB) <span class="text-red-500">*</span>
        </label>
        <div class="relative">
          <input 
            type="file" 
            id="cv" 
            name="cv" 
            accept=".pdf,.doc,.docx"
            required
            class="w-full px-4 py-3 border border-neutral-300 dark:border-neutral-600 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent bg-white dark:bg-neutral-800 text-neutral-900 dark:text-neutral-100 file:mr-4 file:py-2 file:px-4 file:rounded-full file:border-0 file:text-sm file:font-medium file:bg-blue-50 file:text-blue-700 hover:file:bg-blue-100 dark:file:bg-blue-900 dark:file:text-blue-300"
          >
        </div>
        <p class="mt-2 text-sm text-neutral-500 dark:text-neutral-400">
          Lütfen en güncel CV'nizi PDF veya Word formatında yükleyiniz.
        </p>
      </div>
    </div>

<!-- Submit Button -->
<div class="flex justify-center pt-6">
      <button 
        type="submit"
        id="submitBtn"
        class="bg-blue-600 hover:bg-blue-700 text-white font-medium py-3 px-8 rounded-lg transition duration-200 ease-in-out transform hover:scale-105 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2 dark:focus:ring-offset-neutral-800 disabled:opacity-50 disabled:cursor-not-allowed"
      >
        Başvuruyu Gönder
      </button>
    </div>
    
<!-- Form Footer -->
 <div class="text-center text-sm text-neutral-500 dark:text-neutral-400 pt-4">
      <p><span class="text-red-500">*</span> ile işaretlenmiş alanlar zorunludur.</p>
      <p class="mt-2">Başvurunuzu değerlendirip 1-2 hafta içinde size dönüş yapacağız.</p>
    </div>
  </form>
</div>

<style>
/* Custom styles for better file input appearance */
input[type="file"]::-webkit-file-upload-button {
  visibility: hidden;
}

input[type="file"]::before {
  content: 'Dosya Seç';
  display: inline-block;
  background: linear-gradient(top, #f9f9f9, #e3e3e3);
  border: thin solid grey;
  border-radius: 3px;
  padding: 5px 8px;
  outline: none;
  white-space: nowrap;
  -webkit-user-select: none;
  cursor: pointer;
  text-shadow: 1px 1px #fff;
  font-weight: 700;
  font-size: 10pt;
}

input[type="file"]:hover::before {
  border-color: black;
}

input[type="file"]:active::before {
  background: -webkit-linear-gradient(top, #e3e3e3, #f9f9f9);
}
</style>

<script>
// Google Sheets integration setup
// You'll need to replace this URL with your Google Apps Script Web App URL
const GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec';

document.addEventListener('DOMContentLoaded', function() {
  const form = document.getElementById('applicationForm');
  const fileInput = document.getElementById('cv');
  const submitBtn = document.getElementById('submitBtn');
  const successMessage = document.getElementById('successMessage');
  const errorMessage = document.getElementById('errorMessage');
  const loadingSpinner = document.getElementById('loadingSpinner');
  
  // File size validation
  fileInput.addEventListener('change', function() {
    const file = this.files[0];
    if (file && file.size > 5 * 1024 * 1024) { // 5MB in bytes
      alert('Dosya boyutu 5MB\'dan küçük olmalıdır. Lütfen daha küçük bir dosya seçiniz.');
      this.value = '';
    }
  });
  
  // Form submission handling with Google Sheets integration
  form.addEventListener('submit', async function(e) {
    e.preventDefault();
    
    // Reset messages
    successMessage.classList.add('hidden');
    errorMessage.classList.add('hidden');
    loadingSpinner.classList.remove('hidden');
    submitBtn.disabled = true;
    
    // Basic validation
    const requiredFields = form.querySelectorAll('[required]');
    let isValid = true;
    
    requiredFields.forEach(field => {
      if (!field.value.trim()) {
        isValid = false;
        field.classList.add('border-red-500');
      } else {
        field.classList.remove('border-red-500');
      }
    });
    
    if (!isValid) {
      loadingSpinner.classList.add('hidden');
      submitBtn.disabled = false;
      errorMessage.querySelector('span').innerHTML = '<strong>Hata!</strong> Lütfen tüm zorunlu alanları doldurunuz.';
      errorMessage.classList.remove('hidden');
      return;
    }
    
    try {
      // Prepare form data
      const formData = new FormData();
      formData.append('fullName', document.getElementById('fullName').value);
      formData.append('email', document.getElementById('email').value);
      formData.append('phone', document.getElementById('phone').value);
      formData.append('university', document.getElementById('university').value);
      formData.append('major', document.getElementById('major').value);
      formData.append('degree', document.getElementById('degree').value);
      formData.append('year', document.getElementById('year').value);
      formData.append('research_interest', document.getElementById('research_interest').value);
      formData.append('timestamp', new Date().toLocaleString('tr-TR'));
      
      // Handle CV file
      const cvFile = document.getElementById('cv').files[0];
      if (cvFile) {
        // Convert file to base64 for Google Sheets
        const base64 = await fileToBase64(cvFile);
        formData.append('cv_name', cvFile.name);
        formData.append('cv_data', base64);
        formData.append('cv_type', cvFile.type);
      }
      
      // Submit to Google Sheets
      const response = await fetch(GOOGLE_SCRIPT_URL, {
        method: 'POST',
        body: formData
      });
      
      if (response.ok) {
        loadingSpinner.classList.add('hidden');
        successMessage.classList.remove('hidden');
        form.reset();
        
        // Scroll to success message
        successMessage.scrollIntoView({ behavior: 'smooth' });
      } else {
        throw new Error('Form submission failed');
      }
      
    } catch (error) {
      console.error('Error:', error);
      loadingSpinner.classList.add('hidden');
      errorMessage.classList.remove('hidden');
      
      // Scroll to error message
      errorMessage.scrollIntoView({ behavior: 'smooth' });
    } finally {
      submitBtn.disabled = false;
    }
  });
  
  // Helper function to convert file to base64
  function fileToBase64(file) {
    return new Promise((resolve, reject) => {
      const reader = new FileReader();
      reader.readAsDataURL(file);
      reader.onload = () => resolve(reader.result.split(',')[1]);
      reader.onerror = error => reject(error);
    });
  }
});
</script>
