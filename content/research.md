---
title: "Research"
date: 2025-06-05
layout: "simple"
description: "Fatih Kansoy | Research"
slug: "research"
tags: ["research", "publications"]
---

<!-- Font Awesome CDN -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<!-- Tailwind CSS CDN -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Hidden Settings - Set to true/false to control default expansion -->
<script>
    const ALWAYS_OPEN_DEFAULT = false; // Change this to true to keep all abstracts and bibtex expanded by default
</script>

<style>
/* Clean, simple styling for standard page layout */
.paper-section {
    margin-bottom: 2rem;
    background-color: #f2f2f2;
    padding: 1.5rem;
    border-radius: 0.5rem;
    border: 1px solid #e5e7eb;
}

.paper-title {
    font-size: 1.25rem;
    font-weight: 600;
    color: #111827;
    margin-bottom: 0.5rem;
}

.paper-meta {
    font-size: 0.875rem;
    color: #6b7280;
    margin-bottom: 0.5rem;
}

.paper-journal {
    font-size: 0.875rem;
    color: #9ca3af;
    margin-bottom: 1rem;
}

.button-group {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-bottom: 1rem;
}

/* Hide abstract and bibtex by default */
.abstract-section, .bibtex-section {
    display: none;
}

.abstract-section {
    background-color: #ffffff;
    padding: 1.5rem;
    border-radius: 0.5rem;
    margin: 1rem 0;
    border: 1px solid #e5e7eb;
}

.bibtex-section {
    background-color: #111827;
    color: #f3f4f6;
    padding: 1.5rem;
    border-radius: 0.5rem;
    margin: 1rem 0;
    font-family: monospace;
    font-size: 0.75rem;
}

/* Show when toggled */
.abstract-section.show, .bibtex-section.show {
    display: block;
}

.section-divider {
    margin: 3rem 0;
    border-color: #e5e7eb;
}

/* Mobile-friendly responsive design */
@media (max-width: 768px) {
    .paper-section {
        padding: 1rem;
        margin-left: -0.5rem;
        margin-right: -0.5rem;
    }
    
    .button-group {
        gap: 0.5rem;
    }
    
    .button-group a,
    .button-group button {
        font-size: 0.75rem;
        padding: 0.375rem 0.75rem;
    }
}

/* Copy button styling */
.copy-button {
    background-color: #4b5563;
    color: #d1d5db;
    padding: 0.25rem 0.5rem;
    border-radius: 0.25rem;
    font-size: 0.75rem;
    border: none;
    cursor: pointer;
    transition: background-color 0.2s;
}

.copy-button:hover {
    background-color: #6b7280;
}

.copy-button.copied {
    background-color: #059669;
}
</style>

## Research Interests

<div class="bg-gray-50 rounded-lg shadow-sm p-6 mb-8">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div class="flex items-start gap-3">
            <i class="fas fa-chart-line text-blue-600 mt-1"></i>
            <span>Central Banking: Policies, Tools, & Implications</span>
        </div>
        <div class="flex items-start gap-3">
            <i class="fas fa-robot text-blue-600 mt-1"></i>
            <span>Text Mining in Economics and Finance</span>
        </div>
        <div class="flex items-start gap-3">
            <i class="fas fa-leaf text-green-600 mt-1"></i>
            <span>Climate Change and Finance</span>
        </div>
        <div class="flex items-start gap-3">
            <i class="fas fa-history text-purple-600 mt-1"></i>
            <span>Quantitative Economic and Financial History</span>
        </div>
    </div>
</div>

## Working in Progress

<!-- Paper 1: Green Shields -->
<div class="paper-section">
    <h3 class="paper-title">Green Shields: The Role of ESG in Uncertain Times</h3>
    <div class="paper-meta">
        with Dominykas Stasiulaitis 
        <span class="inline-block bg-orange-100 text-orange-800 text-xs px-2 py-1 rounded ml-2">Working Paper</span>
    </div>
    <div class="paper-journal">
        Journal: Department of Economics Discussion Paper Series, University of Oxford
    </div>
    
  <div class="button-group">
        <a href="http://fatih.ai/esg.pdf" class="inline-flex items-center gap-2 text-blue-600 hover:text-blue-800 text-sm bg-blue-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-pdf"></i> View PDF
        </a>
        <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5278853" target="_blank" class="inline-flex items-center gap-2 text-blue-700 hover:text-blue-900 text-sm bg-blue-100 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> SSRN
        </a>
        <a href="https://arxiv.org/abs/2506.02143" target="_blank" class="inline-flex items-center gap-2 text-red-700 hover:text-red-900 text-sm bg-red-100 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-archive"></i> arXiv
        </a>
        <!-- <a href="http://fatih.ai/esg.pdf" download class="inline-flex items-center gap-2 text-green-600 hover:text-green-800 text-sm bg-green-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-download"></i> Download
        </a> -->
        <button onclick="toggleAbstract('paper1')" class="inline-flex items-center gap-2 text-gray-600 hover:text-gray-800 text-sm bg-gray-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> Abstract
        </button>
        <button onclick="toggleBibtex('paper1')" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-quote-left"></i> BibTeX
        </button>
        <a href="https://x.com/kansoy/status/1929638410358346063" target="_blank" class="inline-flex items-center gap-2 text-gray-800 hover:text-gray-900 text-sm bg-gray-100 px-3 py-1.5 rounded-md transition-colors">
            <i class="fab fa-x-twitter"></i> X Thread
        </a>
        <a href="https://bsky.app/profile/fatih.ai/post/3lqno6dfwok24" target="_blank" class="inline-flex items-center gap-2 text-sky-600 hover:text-sky-800 text-sm bg-sky-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-cloud"></i> Bluesky
        </a>
    </div>
    
  <div class="abstract-section" id="paper1-abstract">
        <h4 class="font-semibold mb-2 text-gray-700">Abstract</h4>
        <p class="text-sm text-gray-600 leading-relaxed">
            The rapid growth of sustainable investing, now exceeding 35 trillion USD globally, has transformed financial markets, yet the implications for monetary policy transmission remain underexplored. While existing literature documents heterogeneous firm responses to monetary policy through traditional channels such as size and leverage, it remains unknown whether environmental, social, and governance (ESG) characteristics create distinct transmission mechanisms. Using high-frequency identification around 160 Federal Reserve announcements from 2005 to 2025, we uncover an asymmetric pattern: high-ESG firms gain 1.6 basis points of protection from contractionary target surprises, yet suffer 2.6 basis points greater sensitivity to forward guidance shocks. This asymmetry persists within industries and intensifies with investor climate awareness. Remarkably, the Paris Agreement inverted these relationships: before December 2015, high-ESG firms were more vulnerable to contractionary policy within industries; afterward, they gained protection, representing a 186 basis point reversal. We develop a two-period model featuring heterogeneous investors with sustainability preferences that quantitatively matches these patterns. The model reveals how ESG investors' non-pecuniary utility creates differential demand elasticities, simultaneously protecting green firms from immediate rate changes while amplifying forward guidance vulnerability through their longer investment horizons. These findings establish environmental characteristics as a new dimension of monetary policy non-neutrality, with important implications as sustainable finance continues expanding.
        </p>
    </div>
    
  <div class="bibtex-section" id="paper1-bibtex">
        <div class="flex justify-between items-start mb-2">
            <h4 class="font-sans font-semibold text-gray-300">BibTeX</h4>
            <button onclick="copyBibtex('paper1')" class="copy-button">
                <i class="fas fa-copy mr-1"></i> Copy
            </button>
        </div>
        <pre class="whitespace-pre-wrap" id="paper1-bibtex-content">@article{kansoy2025green,
  title={Green Shields: The Role of ESG in Uncertain Times},
  author={Kansoy, Fatih and Stasiulaitis, Dominykas},
  journal={Department of Economics Discussion Paper Series, University of Oxford},
  volume={June 2025},
  year={2025},
  institution={University of Oxford}
}</pre>
    </div>
</div>

<!-- Paper 2: Central Bank Communication -->
<div class="paper-section">
    <h3 class="paper-title">Central Bank Communication with Public: Bank of England and Twitter (X)</h3>
    <div class="paper-meta">
        with Joel Mundy (Bank of England) 
        <span class="inline-block bg-orange-100 text-orange-800 text-xs px-2 py-1 rounded ml-2">Working Paper</span>
    </div>
    <div class="paper-journal">
        Journal: Department of Economics Discussion Paper Series, University of Oxford
    </div>
    
  <div class="button-group">
        <a href="http://fatih.ai/boe.pdf" class="inline-flex items-center gap-2 text-blue-600 hover:text-blue-800 text-sm bg-blue-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-pdf"></i> View PDF
        </a>
        <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5279225" target="_blank" class="inline-flex items-center gap-2 text-blue-700 hover:text-blue-900 text-sm bg-blue-100 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> SSRN
        </a>
        <a href="https://arxiv.org/abs/2506.02559" target="_blank" class="inline-flex items-center gap-2 text-red-700 hover:text-red-900 text-sm bg-red-100 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-archive"></i> arXiv
        </a>
        <!-- <a href="http://fatih.ai/boe.pdf" download class="inline-flex items-center gap-2 text-green-600 hover:text-green-800 text-sm bg-green-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-download"></i> Download
        </a> -->
        <button onclick="toggleAbstract('paper2')" class="inline-flex items-center gap-2 text-gray-600 hover:text-gray-800 text-sm bg-gray-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> Abstract
        </button>
        <button onclick="toggleBibtex('paper2')" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-quote-left"></i> BibTeX
        </button>
    </div>
    
  <div class="abstract-section" id="paper2-abstract">
        <h4 class="font-semibold mb-2 text-gray-700">Abstract</h4>
        <p class="text-sm text-gray-600 leading-relaxed">
            Central banks increasingly use social media to communicate beyond financial markets, yet evidence on public engagement effectiveness remains limited. Despite 113 central banks joining Twitter between 2008 and 2018, we lack understanding of what drives audience interaction with their content. To examine engagement determinants, we analyzed 3.13 million tweets mentioning the Bank of England from 2007 to 2022, including 9,810 official posts. We investigate posting patterns, measure engagement elasticity, and identify content characteristics predicting higher interaction. The Bank's posting schedule misaligns with peak audience engagement times, with evening hours generating the highest interaction despite minimal posting. Cultural content, such as the Alan Turing 50 pound note, achieved 1,300 times higher engagement than routine policy communications. Engagement elasticity averaged 1.095 with substantial volatility during events like Brexit, contrasting with the Federal Reserve's stability. Media content dramatically increased engagement: videos by 1,700 percent, photos by 126 percent, while monetary policy announcements and readability significantly enhanced all metrics. Content quality and timing matter more than posting frequency for effective central bank communication. These findings suggest central banks should prioritize accessible, media-rich content during high-attention periods rather than increasing volume, with implications for digital communication strategies in fulfilling public transparency mandates.
        </p>
    </div>
    
  <div class="bibtex-section" id="paper2-bibtex">
        <div class="flex justify-between items-start mb-2">
            <h4 class="font-sans font-semibold text-gray-300">BibTeX</h4>
            <button onclick="copyBibtex('paper2')" class="copy-button">
                <i class="fas fa-copy mr-1"></i> Copy
            </button>
        </div>
        <pre class="whitespace-pre-wrap" id="paper2-bibtex-content">@article{kansoy2025central,
  title={Central Bank Communication with Public: Bank of England and Twitter (X)},
  author={Kansoy, Fatih and Mundy, Joel},
  journal={Department of Economics Discussion Paper Series, University of Oxford},
  volume={July 2025},
  year={2025},
  institution={University of Oxford and Bank of England}
}</pre>
    </div>
</div>

<hr class="section-divider">

## Published Papers

<!-- Paper 3: NIM -->
<div class="paper-section">
    <h3 class="paper-title">The Determinants of Net Interest Margin in the Turkish Banking Sector: Does Bank Ownership Matter?</h3>
    <div class="paper-meta">
        <span class="inline-block bg-indigo-100 text-indigo-800 text-xs px-2 py-1 rounded">Journal Article</span>
    </div>
    <div class="paper-journal">
        Journal of BRSA Banking and Financial Markets
    </div>
    
  <div class="button-group">
        <a href="http://fatih.ai/nim.pdf" class="inline-flex items-center gap-2 text-blue-600 hover:text-blue-800 text-sm bg-blue-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-pdf"></i> View PDF
        </a>
        <a href="https://dergipark.org.tr/tr/pub/bddkdergisi/issue/57356/874957" target="_blank" class="inline-flex items-center gap-2 text-violet-600 hover:text-violet-800 text-sm bg-violet-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-journal-whills"></i> Journal
        </a>
        <a href="http://fatih.ai/nim.pdf" download class="inline-flex items-center gap-2 text-green-600 hover:text-green-800 text-sm bg-green-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-download"></i> Download
        </a>
        <button onclick="toggleAbstract('nim')" class="inline-flex items-center gap-2 text-gray-600 hover:text-gray-800 text-sm bg-gray-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> Abstract
        </button>
        <button onclick="toggleBibtex('nim')" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-quote-left"></i> BibTeX
        </button>
    </div>
    
  <div class="abstract-section" id="nim-abstract">
        <h4 class="font-semibold mb-2 text-gray-700">Abstract</h4>
        <p class="text-sm text-gray-600 leading-relaxed">
            This research presented an empirical investigation of the determinants of the net interest margin in Turkish Banking sector with a particular emphasis on the bank ownership structure. This study employed a unique bank-level dataset covering Turkey's commercial banking sector for the 2001-2012. Our main results are as follows. Operation diversity, credit risk and operating costs are important determinants of margin in Turkey. More efficient banks exhibit lower margin and also price stability contributes to lower margin. The effect of principal determinants such as credit risk, bank size, market concentration and inflation vary across foreign-owned, state-controlled and private banks. At the same time, the impacts of implicit interest payment, operation diversity and operating cost are homogeneous across all banks.
        </p>
    </div>
    
  <div class="bibtex-section" id="nim-bibtex">
        <div class="flex justify-between items-start mb-2">
            <h4 class="font-sans font-semibold text-gray-300">BibTeX</h4>
            <button onclick="copyBibtex('nim')" class="copy-button">
                <i class="fas fa-copy mr-1"></i> Copy
            </button>
        </div>
        <pre class="whitespace-pre-wrap" id="nim-bibtex-content">@article{kansoy2012determinants,
  title={The determinants of net interest margin in the Turkish banking sector: does bank ownership matter},
  author={Kansoy, Fatih},
  journal={Journal of BRSA Banking and Financial Markets},
  volume={6},
  number={2},
  pages={13--49},
  year={2012},
  publisher={Banking Regulation and Supervision Agency}
}</pre>
    </div>
</div>

<!-- Paper 4: Istanbul -->
<div class="paper-section">
    <h3 class="paper-title">Islamic Finance as a Means to Make Istanbul an International Financial Centre</h3>
    <div class="paper-meta">
        with H Karlioglu 
        <span class="inline-block bg-indigo-100 text-indigo-800 text-xs px-2 py-1 rounded ml-2">Journal Article</span>
    </div>
    <div class="paper-journal">
        Afro Eurasian Studies
    </div>
    
  <div class="button-group">
        <a href="http://fatih.ai/istanbul.pdf" class="inline-flex items-center gap-2 text-blue-600 hover:text-blue-800 text-sm bg-blue-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-pdf"></i> View PDF
        </a>
        <a href="https://dergipark.org.tr/en/pub/afes/issue/44783/557024" target="_blank" class="inline-flex items-center gap-2 text-violet-600 hover:text-violet-800 text-sm bg-violet-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-journal-whills"></i> Journal
        </a>
        <a href="http://fatih.ai/istanbul.pdf" download class="inline-flex items-center gap-2 text-green-600 hover:text-green-800 text-sm bg-green-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-download"></i> Download
        </a>
        <button onclick="toggleAbstract('istanbul')" class="inline-flex items-center gap-2 text-gray-600 hover:text-gray-800 text-sm bg-gray-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-file-alt"></i> Abstract
        </button>
        <button onclick="toggleBibtex('istanbul')" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
            <i class="fas fa-quote-left"></i> BibTeX
        </button>
    </div>
    
  <div class="abstract-section" id="istanbul-abstract">
        <h4 class="font-semibold mb-2 text-gray-700">Abstract</h4>
        <p class="text-sm text-gray-600 leading-relaxed">
            This paper discusses and assesses Istanbul as an international finance centre within the context of its position in the sector of of Islamic finance. No doubt, Istanbul is a centre of business and culture of Turkey and the Turkish government is at present endeavouring to turn Istanbul into a regional finance centre in ten years and ,furthermore, into one of the top international financial centre in thirty years. In this context we evaluate Istanbul's potential and position to assume the role of a hub for Islamic finance. Our main conclusions are as follows; the current image, legal and regulatory infrastructure and human capacity of Istanbul do not presently allow it to become an international finance centre. In contrast, if we consider its strategic location standing between the Middle East, Eurasia and Africa as well as its strong relations with Muslim countries, and ,last but not least, its strong banking system, Istanbul has the potential to serve as a centre for Islamic finance provided that the government's ambitions remain focused in this direction.
        </p>
    </div>
    
  <div class="bibtex-section" id="istanbul-bibtex">
        <div class="flex justify-between items-start mb-2">
            <h4 class="font-sans font-semibold text-gray-300">BibTeX</h4>
            <button onclick="copyBibtex('istanbul')" class="copy-button">
                <i class="fas fa-copy mr-1"></i> Copy
            </button>
        </div>
        <pre class="whitespace-pre-wrap" id="istanbul-bibtex-content">@article{kansoy2013islamic,
  title={Islamic Finance as a Means to Make Istanbul an International Financial Centre},
  author={Kansoy, Fatih and Karlioglu, Hasan Huseyin},
  journal={Afro Eurasian Studies},
  volume={2},
  number={1-2},
  pages={126--143},
  year={2013},
  publisher={Musiad (Independent Industrialists and Businessmen's Association)}
}</pre>
    </div>
</div>

<script>
// Toggle abstract visibility
function toggleAbstract(paperId) {
    const abstractBox = document.getElementById(paperId + '-abstract');
    const bibtexBox = document.getElementById(paperId + '-bibtex');
    
    // Hide bibtex if shown
    if (bibtexBox && bibtexBox.classList.contains('show')) {
        bibtexBox.classList.remove('show');
    }
    
    abstractBox.classList.toggle('show');
}

// Toggle bibtex visibility
function toggleBibtex(paperId) {
    const bibtexBox = document.getElementById(paperId + '-bibtex');
    const abstractBox = document.getElementById(paperId + '-abstract');
    
    // Hide abstract if shown
    if (abstractBox && abstractBox.classList.contains('show')) {
        abstractBox.classList.remove('show');
    }
    
    bibtexBox.classList.toggle('show');
}

// Copy BibTeX to clipboard
function copyBibtex(paperId) {
    const bibtexContent = document.getElementById(paperId + '-bibtex-content').textContent;
    navigator.clipboard.writeText(bibtexContent).then(function() {
        // Change button text temporarily
        const button = event.target.closest('button');
        const originalHTML = button.innerHTML;
        button.innerHTML = '<i class="fas fa-check mr-1"></i> Copied!';
        button.classList.add('copied');
        
        setTimeout(() => {
            button.innerHTML = originalHTML;
            button.classList.remove('copied');
        }, 2000);
    }).catch(function(err) {
        console.error('Could not copy text: ', err);
    });
}

// Apply default expansion setting on load
window.onload = function() {
    if (ALWAYS_OPEN_DEFAULT) {
        // Show all abstracts and bibtex sections
        const allAbstracts = document.querySelectorAll('.abstract-section');
        const allBibtex = document.querySelectorAll('.bibtex-section');
        
        allAbstracts.forEach(abstract => {
            abstract.classList.add('show');
        });
        allBibtex.forEach(bibtex => {
            bibtex.classList.add('show');
        });
    }
}
</script>
<!-- 
==========================
BUTTON LIBRARY - Copy and paste these buttons as needed
==========================

PDF Button:
<a href="#" class="inline-flex items-center gap-2 text-blue-600 hover:text-blue-800 text-sm bg-blue-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-file-pdf"></i> View PDF
</a>

Download Button:
<a href="#" download class="inline-flex items-center gap-2 text-green-600 hover:text-green-800 text-sm bg-green-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-download"></i> Download
</a>

Abstract Button:
<button onclick="toggleAbstract(event, 'PAPER_ID')" class="inline-flex items-center gap-2 text-gray-600 hover:text-gray-800 text-sm bg-gray-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-file-alt"></i> Abstract
</button>

BibTeX Button:
<button onclick="toggleBibtex(event, 'PAPER_ID')" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-quote-left"></i> BibTeX
</button>

External Link Button:
<a href="https://example.com" target="_blank" class="inline-flex items-center gap-2 text-indigo-600 hover:text-indigo-800 text-sm bg-indigo-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-external-link-alt"></i> External Link
</a>

Code Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-orange-600 hover:text-orange-800 text-sm bg-orange-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-code"></i> Code
</a>

Dataset Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-pink-600 hover:text-pink-800 text-sm bg-pink-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-database"></i> Dataset
</a>

Slides Button:
<a href="#" class="inline-flex items-center gap-2 text-teal-600 hover:text-teal-800 text-sm bg-teal-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-presentation-screen"></i> Slides
</a>

Video Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-red-600 hover:text-red-800 text-sm bg-red-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-video"></i> Video
</a>

Poster Button:
<a href="#" class="inline-flex items-center gap-2 text-yellow-600 hover:text-yellow-800 text-sm bg-yellow-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-image"></i> Poster
</a>

X (Twitter) Thread Button:
<a href="https://twitter.com/intent/tweet?text=YOUR_TEXT_HERE&url=YOUR_URL_HERE" target="_blank" class="inline-flex items-center gap-2 text-gray-800 hover:text-gray-900 text-sm bg-gray-100 px-3 py-1.5 rounded-md transition-colors">
    <i class="fab fa-x-twitter"></i> X Thread
</a>

Bluesky Button:
<a href="https://bsky.app/intent/compose?text=YOUR_TEXT_HERE" target="_blank" class="inline-flex items-center gap-2 text-sky-600 hover:text-sky-800 text-sm bg-sky-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-cloud"></i> Bluesky
</a>

LinkedIn Button:
<a href="https://www.linkedin.com/sharing/share-offsite/?url=YOUR_URL_HERE" target="_blank" class="inline-flex items-center gap-2 text-blue-700 hover:text-blue-900 text-sm bg-blue-100 px-3 py-1.5 rounded-md transition-colors">
    <i class="fab fa-linkedin"></i> LinkedIn
</a>

GitHub Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-gray-900 hover:text-black text-sm bg-gray-200 px-3 py-1.5 rounded-md transition-colors">
    <i class="fab fa-github"></i> GitHub
</a>

Preprint Button:
<a href="#" class="inline-flex items-center gap-2 text-emerald-600 hover:text-emerald-800 text-sm bg-emerald-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-file-lines"></i> Preprint
</a>

Journal Link Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-violet-600 hover:text-violet-800 text-sm bg-violet-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-journal-whills"></i> Journal
</a>

DOI Button:
<a href="https://doi.org/YOUR_DOI_HERE" target="_blank" class="inline-flex items-center gap-2 text-cyan-600 hover:text-cyan-800 text-sm bg-cyan-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-fingerprint"></i> DOI
</a>

Cite Button:
<button onclick="toggleCitation(event, 'PAPER_ID')" class="inline-flex items-center gap-2 text-rose-600 hover:text-rose-800 text-sm bg-rose-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-quote-right"></i> Cite
</button>

Blog Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-orange-600 hover:text-orange-800 text-sm bg-orange-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-blog"></i> Blog
</a>

YouTube Button:
<a href="https://youtube.com/watch?v=YOUR_VIDEO_ID" target="_blank" class="inline-flex items-center gap-2 text-red-600 hover:text-red-800 text-sm bg-red-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fab fa-youtube"></i> YouTube
</a>

Media Button:
<a href="#" target="_blank" class="inline-flex items-center gap-2 text-purple-600 hover:text-purple-800 text-sm bg-purple-50 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-newspaper"></i> Media
</a>


SSRN Button:
<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=YOUR_SSRN_ID" target="_blank" class="inline-flex items-center gap-2 text-blue-700 hover:text-blue-900 text-sm bg-blue-100 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-file-alt"></i> SSRN
</a>

ArXiv Button:
<a href="https://arxiv.org/abs/YOUR_ARXIV_ID" target="_blank" class="inline-flex items-center gap-2 text-red-700 hover:text-red-900 text-sm bg-red-100 px-3 py-1.5 rounded-md transition-colors">
    <i class="fas fa-archive"></i> arXiv
</a>
==========================
STATUS BADGES
==========================

Draft Ready Badge (Subtle Style):
<a href="YOUR_LINK" target="_blank" class="draft-badge inline-flex items-center gap-1 text-gray-600 hover:text-gray-800 text-xs bg-gray-50 px-2 py-1 rounded-md transition-colors">Draft Ready →</a>

Published Badge:
<span class="inline-block bg-green-100 text-green-800 text-xs px-2 py-1 rounded">Published</span>

Under Review Badge:
<span class="inline-block bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Under Review</span>

Working Paper Badge:
<span class="inline-block bg-orange-100 text-orange-800 text-xs px-2 py-1 rounded">Working Paper</span>

Book Badge:
<span class="inline-block bg-purple-100 text-purple-800 text-xs px-2 py-1 rounded">Book</span>

Journal Article Badge:
<span class="inline-block bg-indigo-100 text-indigo-800 text-xs px-2 py-1 rounded">Journal Article</span>

Conference Paper Badge:
<span class="inline-block bg-teal-100 text-teal-800 text-xs px-2 py-1 rounded">Conference Paper</span>

Forthcoming Badge:
<span class="inline-block bg-pink-100 text-pink-800 text-xs px-2 py-1 rounded">Forthcoming</span>

-->