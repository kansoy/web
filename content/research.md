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

<style>
/* Theme-compatible styles */
.research-container {
    max-width: 1200px;
    margin: 0 auto;
}

.research-interests {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1rem;
    margin: 2rem 0;
}

.interest-item {
    display: flex;
    align-items: start;
    gap: 0.75rem;
    padding: 1rem;
    background-color: var(--color-neutral-100);
    border-radius: 0.5rem;
}

.paper-card {
    background-color: var(--color-neutral-50);
    border: 1px solid var(--color-neutral-200);
    border-radius: 0.5rem;
    margin-bottom: 1.5rem;
    overflow: hidden;
}

.paper-header {
    padding: 1.5rem;
    cursor: pointer;
    position: relative;
}

.paper-header:hover {
    background-color: var(--color-neutral-100);
}

.paper-title {
    font-size: 1.25rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
    padding-right: 2rem;
}

.paper-meta {
    font-size: 0.875rem;
    color: var(--color-neutral-600);
    margin-bottom: 0.25rem;
}

.paper-journal {
    font-size: 0.875rem;
    font-style: italic;
    color: var(--color-neutral-500);
}

.expand-icon {
    position: absolute;
    top: 1.5rem;
    right: 1.5rem;
    transition: transform 0.3s ease;
}

.expand-icon.rotated {
    transform: rotate(180deg);
}

.paper-content {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease;
}

.paper-content.expanded {
    max-height: 2000px;
}

.paper-inner {
    padding: 0 1.5rem 1.5rem;
}

.button-group {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
}

.paper-button {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.5rem 1rem;
    background-color: var(--color-neutral-100);
    border: 1px solid var(--color-neutral-200);
    border-radius: 0.375rem;
    text-decoration: none;
    font-size: 0.875rem;
    transition: all 0.2s;
}

.paper-button:hover {
    background-color: var(--color-neutral-200);
}

.btn-pdf { color: #2563eb; }
.btn-ssrn { color: #1e40af; }
.btn-arxiv { color: #dc2626; }
.btn-download { color: #059669; }
.btn-journal { color: #7c3aed; }
.btn-twitter { color: var(--color-neutral-800); }
.btn-bluesky { color: #0ea5e9; }
.btn-bibtex { color: #8b5cf6; }

.content-section {
    background-color: var(--color-neutral-100);
    padding: 1rem;
    border-radius: 0.375rem;
    margin-bottom: 1rem;
}

.section-title {
    font-weight: 600;
    margin-bottom: 0.75rem;
    font-size: 0.875rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--color-neutral-600);
}

.bibtex-content {
    background-color: var(--color-neutral-800);
    color: var(--color-neutral-100);
    padding: 1rem;
    border-radius: 0.375rem;
    font-family: monospace;
    font-size: 0.8rem;
    overflow-x: auto;
    position: relative;
}

.copy-button {
    position: absolute;
    top: 0.5rem;
    right: 0.5rem;
    background-color: var(--color-neutral-700);
    color: var(--color-neutral-100);
    border: none;
    padding: 0.25rem 0.5rem;
    border-radius: 0.25rem;
    cursor: pointer;
    font-size: 0.75rem;
}

.copy-button:hover {
    background-color: var(--color-neutral-600);
}

.status-badge {
    display: inline-block;
    padding: 0.25rem 0.75rem;
    font-size: 0.75rem;
    font-weight: 500;
    border-radius: 9999px;
    margin-left: 0.5rem;
}

.badge-working {
    background-color: #fed7aa;
    color: #c2410c;
}

.badge-journal {
    background-color: #ddd6fe;
    color: #6d28d9;
}

.section-divider {
    margin: 3rem 0;
    border: 0;
    border-top: 2px solid var(--color-neutral-200);
}

/* Hide elements by default */
.hidden {
    display: none;
}

/* Mobile responsive */
@media (max-width: 768px) {
    .research-interests {
        grid-template-columns: 1fr;
    }
    
    .paper-title {
        font-size: 1.125rem;
    }
    
    .button-group {
        gap: 0.375rem;
    }
    
    .paper-button {
        font-size: 0.75rem;
        padding: 0.375rem 0.75rem;
    }
}

/* Dark mode compatibility */
@media (prefers-color-scheme: dark) {
    .paper-card {
        background-color: var(--color-neutral-800);
        border-color: var(--color-neutral-700);
    }
    
    .paper-header:hover {
        background-color: var(--color-neutral-700);
    }
    
    .content-section {
        background-color: var(--color-neutral-800);
    }
    
    .paper-button {
        background-color: var(--color-neutral-800);
        border-color: var(--color-neutral-700);
    }
    
    .paper-button:hover {
        background-color: var(--color-neutral-700);
    }
}
</style>

<div class="research-container">

## Research Interests

<div class="research-interests">
    <div class="interest-item">
        <i class="fas fa-chart-line" style="color: #2563eb;"></i>
        <span>Central Banking: Policies, Tools, & Implications</span>
    </div>
    <div class="interest-item">
        <i class="fas fa-robot" style="color: #2563eb;"></i>
        <span>Text Mining in Economics and Finance</span>
    </div>
    <div class="interest-item">
        <i class="fas fa-leaf" style="color: #10b981;"></i>
        <span>Climate Change and Finance</span>
    </div>
    <div class="interest-item">
        <i class="fas fa-history" style="color: #8b5cf6;"></i>
        <span>Quantitative Economic and Financial History</span>
    </div>
</div>

## Working Papers

<!-- Paper 1 -->
<div class="paper-card">
    <div class="paper-header" onclick="togglePaper('paper1')">
        <h3 class="paper-title">Green Shields: The Role of ESG in Uncertain Times</h3>
        <div class="paper-meta">
            with Dominykas Stasiulaitis
            <span class="status-badge badge-working">Working Paper</span>
        </div>
        <div class="paper-journal">
            Department of Economics Discussion Paper Series, University of Oxford
        </div>
        <i class="fas fa-chevron-down expand-icon" id="paper1-icon"></i>
    </div>
    
  <div class="paper-content" id="paper1-content">
        <div class="paper-inner">
            <div class="button-group">
                <a href="http://fatih.ai/esg.pdf" class="paper-button btn-pdf">
                    <i class="fas fa-file-pdf"></i> View PDF
                </a>
                <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5278853" target="_blank" class="paper-button btn-ssrn">
                    <i class="fas fa-file-alt"></i> SSRN
                </a>
                <a href="https://arxiv.org/abs/2506.02143" target="_blank" class="paper-button btn-arxiv">
                    <i class="fas fa-archive"></i> arXiv
                </a>
                <a href="http://fatih.ai/esg.pdf" download class="paper-button btn-download">
                    <i class="fas fa-download"></i> Download
                </a>
                <a href="https://x.com/kansoy/status/1929638410358346063" target="_blank" class="paper-button btn-twitter">
                    <i class="fab fa-x-twitter"></i> X Thread
                </a>
                <a href="https://bsky.app/profile/fatih.ai/post/3lqno6dfwok24" target="_blank" class="paper-button btn-bluesky">
                    <i class="fas fa-cloud"></i> Bluesky
                </a>
                <button onclick="toggleSection('paper1-abstract')" class="paper-button">
                    <i class="fas fa-file-alt"></i> Abstract
                </button>
                <button onclick="toggleSection('paper1-bibtex')" class="paper-button btn-bibtex">
                    <i class="fas fa-quote-left"></i> BibTeX
                </button>
            </div>
            
<div id="paper1-abstract" class="content-section hidden">
                <div class="section-title">Abstract</div>
                <div>
                    The rapid growth of sustainable investing, now exceeding 35 trillion USD globally, has transformed financial markets, yet the implications for monetary policy transmission remain underexplored. While existing literature documents heterogeneous firm responses to monetary policy through traditional channels such as size and leverage, it remains unknown whether environmental, social, and governance (ESG) characteristics create distinct transmission mechanisms. Using high-frequency identification around 160 Federal Reserve announcements from 2005 to 2025, we uncover an asymmetric pattern: high-ESG firms gain 1.6 basis points of protection from contractionary target surprises, yet suffer 2.6 basis points greater sensitivity to forward guidance shocks. This asymmetry persists within industries and intensifies with investor climate awareness. Remarkably, the Paris Agreement inverted these relationships: before December 2015, high-ESG firms were more vulnerable to contractionary policy within industries; afterward, they gained protection, representing a 186 basis point reversal. We develop a two-period model featuring heterogeneous investors with sustainability preferences that quantitatively matches these patterns. The model reveals how ESG investors' non-pecuniary utility creates differential demand elasticities, simultaneously protecting green firms from immediate rate changes while amplifying forward guidance vulnerability through their longer investment horizons. These findings establish environmental characteristics as a new dimension of monetary policy non-neutrality, with important implications as sustainable finance continues expanding.
                </div>
            </div>
            
   <div id="paper1-bibtex" class="content-section hidden">
                <div class="section-title">BibTeX</div>
                <div class="bibtex-content">
                    <button class="copy-button" onclick="copyBibtex('paper1-bib')">
                        <i class="fas fa-copy"></i> Copy
                    </button>
                    <pre id="paper1-bib">@article{kansoy2025green,
  title={Green Shields: The Role of ESG in Uncertain Times},
  author={Kansoy, Fatih and Stasiulaitis, Dominykas},
  journal={Department of Economics Discussion Paper Series, University of Oxford},
  volume={June 2025},
  year={2025},
  institution={University of Oxford}
}</pre>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- Paper 2 -->
<div class="paper-card">
    <div class="paper-header" onclick="togglePaper('paper2')">
        <h3 class="paper-title">Central Bank Communication with Public: Bank of England and Twitter (X)</h3>
        <div class="paper-meta">
            with Joel Mundy (Bank of England)
            <span class="status-badge badge-working">Working Paper</span>
        </div>
        <div class="paper-journal">
            Department of Economics Discussion Paper Series, University of Oxford
        </div>
        <i class="fas fa-chevron-down expand-icon" id="paper2-icon"></i>
    </div>
    
 <div class="paper-content" id="paper2-content">
        <div class="paper-inner">
            <div class="button-group">
                <a href="http://fatih.ai/boe.pdf" class="paper-button btn-pdf">
                    <i class="fas fa-file-pdf"></i> View PDF
                </a>
                <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5279225" target="_blank" class="paper-button btn-ssrn">
                    <i class="fas fa-file-alt"></i> SSRN
                </a>
                <a href="https://arxiv.org/abs/2506.02559" target="_blank" class="paper-button btn-arxiv">
                    <i class="fas fa-archive"></i> arXiv
                </a>
                <a href="http://fatih.ai/boe.pdf" download class="paper-button btn-download">
                    <i class="fas fa-download"></i> Download
                </a>
                <button onclick="toggleSection('paper2-abstract')" class="paper-button">
                    <i class="fas fa-file-alt"></i> Abstract
                </button>
                <button onclick="toggleSection('paper2-bibtex')" class="paper-button btn-bibtex">
                    <i class="fas fa-quote-left"></i> BibTeX
                </button>
            </div>
            
<div id="paper2-abstract" class="content-section hidden">
                <div class="section-title">Abstract</div>
                <div>
                    Central banks increasingly use social media to communicate beyond financial markets, yet evidence on public engagement effectiveness remains limited. Despite 113 central banks joining Twitter between 2008 and 2018, we lack understanding of what drives audience interaction with their content. To examine engagement determinants, we analyzed 3.13 million tweets mentioning the Bank of England from 2007 to 2022, including 9,810 official posts. We investigate posting patterns, measure engagement elasticity, and identify content characteristics predicting higher interaction. The Bank's posting schedule misaligns with peak audience engagement times, with evening hours generating the highest interaction despite minimal posting. Cultural content, such as the Alan Turing 50 pound note, achieved 1,300 times higher engagement than routine policy communications. Engagement elasticity averaged 1.095 with substantial volatility during events like Brexit, contrasting with the Federal Reserve's stability. Media content dramatically increased engagement: videos by 1,700 percent, photos by 126 percent, while monetary policy announcements and readability significantly enhanced all metrics. Content quality and timing matter more than posting frequency for effective central bank communication. These findings suggest central banks should prioritize accessible, media-rich content during high-attention periods rather than increasing volume, with implications for digital communication strategies in fulfilling public transparency mandates.
                </div>
            </div>
            
 <div id="paper2-bibtex" class="content-section hidden">
                <div class="section-title">BibTeX</div>
                <div class="bibtex-content">
                    <button class="copy-button" onclick="copyBibtex('paper2-bib')">
                        <i class="fas fa-copy"></i> Copy
                    </button>
                    <pre id="paper2-bib">@article{kansoy2025central,
  title={Central Bank Communication with Public: Bank of England and Twitter (X)},
  author={Kansoy, Fatih and Mundy, Joel},
  journal={Department of Economics Discussion Paper Series, University of Oxford},
  volume={July 2025},
  year={2025},
  institution={University of Oxford and Bank of England}
}</pre>
                </div>
            </div>
        </div>
    </div>
</div>

<hr class="section-divider">

## Published Papers

<!-- Paper 3 -->
<div class="paper-card">
    <div class="paper-header" onclick="togglePaper('paper3')">
        <h3 class="paper-title">The Determinants of Net Interest Margin in the Turkish Banking Sector: Does Bank Ownership Matter?</h3>
        <div class="paper-meta">
            <span class="status-badge badge-journal">Journal Article</span>
        </div>
        <div class="paper-journal">
            Journal of BRSA Banking and Financial Markets
        </div>
        <i class="fas fa-chevron-down expand-icon" id="paper3-icon"></i>
    </div>
    
    
<div class="paper-content" id="paper3-content">
        <div class="paper-inner">
            <div class="button-group">
                <a href="http://fatih.ai/nim.pdf" class="paper-button btn-pdf">
                    <i class="fas fa-file-pdf"></i> View PDF
                </a>
                <a href="https://dergipark.org.tr/tr/pub/bddkdergisi/issue/57356/874957" target="_blank" class="paper-button btn-journal">
                    <i class="fas fa-journal-whills"></i> Journal
                </a>
                <a href="http://fatih.ai/nim.pdf" download class="paper-button btn-download">
                    <i class="fas fa-download"></i> Download
                </a>
                <button onclick="toggleSection('paper3-abstract')" class="paper-button">
                    <i class="fas fa-file-alt"></i> Abstract
                </button>
                <button onclick="toggleSection('paper3-bibtex')" class="paper-button btn-bibtex">
                    <i class="fas fa-quote-left"></i> BibTeX
                </button>
            </div>
            
<div id="paper3-abstract" class="content-section hidden">
                <div class="section-title">Abstract</div>
                <div>
                    This research presented an empirical investigation of the determinants of the net interest margin in Turkish Banking sector with a particular emphasis on the bank ownership structure. This study employed a unique bank-level dataset covering Turkey's commercial banking sector for the 2001-2012. Our main results are as follows. Operation diversity, credit risk and operating costs are important determinants of margin in Turkey. More efficient banks exhibit lower margin and also price stability contributes to lower margin. The effect of principal determinants such as credit risk, bank size, market concentration and inflation vary across foreign-owned, state-controlled and private banks. At the same time, the impacts of implicit interest payment, operation diversity and operating cost are homogeneous across all banks.
                </div>
            </div>
            
   <div id="paper3-bibtex" class="content-section hidden">
                <div class="section-title">BibTeX</div>
                <div class="bibtex-content">
                    <button class="copy-button" onclick="copyBibtex('paper3-bib')">
                        <i class="fas fa-copy"></i> Copy
                    </button>
                    <pre id="paper3-bib">@article{kansoy2012determinants,
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
        </div>
    </div>
</div>

<!-- Paper 4 -->
<div class="paper-card">
    <div class="paper-header" onclick="togglePaper('paper4')">
        <h3 class="paper-title">Islamic Finance as a Means to Make Istanbul an International Financial Centre</h3>
        <div class="paper-meta">
            with H Karlioglu
            <span class="status-badge badge-journal">Journal Article</span>
        </div>
        <div class="paper-journal">
            Afro Eurasian Studies
        </div>
        <i class="fas fa-chevron-down expand-icon" id="paper4-icon"></i>
    </div>
    
 <div class="paper-content" id="paper4-content">
        <div class="paper-inner">
            <div class="button-group">
                <a href="http://fatih.ai/istanbul.pdf" class="paper-button btn-pdf">
                    <i class="fas fa-file-pdf"></i> View PDF
                </a>
                <a href="https://dergipark.org.tr/en/pub/afes/issue/44783/557024" target="_blank" class="paper-button btn-journal">
                    <i class="fas fa-journal-whills"></i> Journal
                </a>
                <a href="http://fatih.ai/istanbul.pdf" download class="paper-button btn-download">
                    <i class="fas fa-download"></i> Download
                </a>
                <button onclick="toggleSection('paper4-abstract')" class="paper-button">
                    <i class="fas fa-file-alt"></i> Abstract
                </button>
                <button onclick="toggleSection('paper4-bibtex')" class="paper-button btn-bibtex">
                    <i class="fas fa-quote-left"></i> BibTeX
                </button>
            </div>
            
  <div id="paper4-abstract" class="content-section hidden">
                <div class="section-title">Abstract</div>
                <div>
                    This paper discusses and assesses Istanbul as an international finance centre within the context of its position in the sector of Islamic finance. No doubt, Istanbul is a centre of business and culture of Turkey and the Turkish government is at present endeavouring to turn Istanbul into a regional finance centre in ten years and, furthermore, into one of the top international financial centres in thirty years. In this context we evaluate Istanbul's potential and position to assume the role of a hub for Islamic finance. Our main conclusions are as follows; the current image, legal and regulatory infrastructure and human capacity of Istanbul do not presently allow it to become an international finance centre. In contrast, if we consider its strategic location standing between the Middle East, Eurasia and Africa as well as its strong relations with Muslim countries, and, last but not least, its strong banking system, Istanbul has the potential to serve as a centre for Islamic finance provided that the government's ambitions remain focused in this direction.
                </div>
            </div>
            
 <div id="paper4-bibtex" class="content-section hidden">
                <div class="section-title">BibTeX</div>
                <div class="bibtex-content">
                    <button class="copy-button" onclick="copyBibtex('paper4-bib')">
                        <i class="fas fa-copy"></i> Copy
                    </button>
                    <pre id="paper4-bib">@article{kansoy2013islamic,
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
        </div>
    </div>
</div>

</div>

<script>
// Toggle paper expansion
function togglePaper(paperId) {
    const content = document.getElementById(paperId + '-content');
    const icon = document.getElementById(paperId + '-icon');
    
    content.classList.toggle('expanded');
    icon.classList.toggle('rotated');
}

// Toggle individual sections (abstract, bibtex)
function toggleSection(sectionId) {
    const section = document.getElementById(sectionId);
    section.classList.toggle('hidden');
    
    // Hide other sections in the same paper
    const paperId = sectionId.split('-')[0];
    const otherSection = sectionId.includes('abstract') ? 
        document.getElementById(paperId + '-bibtex') : 
        document.getElementById(paperId + '-abstract');
    
    if (otherSection && !section.classList.contains('hidden')) {
        otherSection.classList.add('hidden');
    }
}

// Copy BibTeX
function copyBibtex(id) {
    const text = document.getElementById(id).textContent;
    navigator.clipboard.writeText(text).then(function() {
        const button = event.target.closest('button');
        const originalHTML = button.innerHTML;
        button.innerHTML = '<i class="fas fa-check"></i> Copied!';
        setTimeout(() => {
            button.innerHTML = originalHTML;
        }, 2000);
    });
}
</script>