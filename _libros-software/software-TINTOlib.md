---
layout: archive
title: "TINTOlib - Python library for transforming tabular data into synthetic images"
excerpt: "TINTOlib is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through differents algorithmic methods.<br/><img src='/images/tinto-logo.svg' width='150' align='center' />"
collection: libros-software
category: "Software"
image: "/images/tinto-logo.svg"
permalink: /libros-software/software-TINTOlib/
author_profile: true
---

{% include base_path %}

<!-- ✅ SEO básico -->
<link rel="canonical" href="{{ site.url }}{{ page.permalink }}">
<meta name="robots" content="index,follow">
<meta name="description" content="TINTOlib is a Python library that converts tidy tabular data into synthetic images for Deep Learning with CNNs, ViTs and hybrid models.">
<meta name="keywords" content="TINTOlib, tabular to image, tidy data, synthetic images, deep learning, CNN, ViT, Vision Transformer, hybrid neural networks, Python, Data Science">
<meta name="author" content="Manuel Castillo-Cara">

<!-- ✅ Open Graph / Twitter -->
<meta property="og:title" content="TINTOlib — Tabular Data → Synthetic Images">
<meta property="og:description" content="Python library to transform tidy tabular data into synthetic images for Deep Learning (CNNs, ViTs, hybrid).">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}{{ page.permalink }}">
<meta property="og:image" content="{{ site.url }}{{ page.image }}">
<meta property="og:image:width" content="1200"><meta property="og:image:height" content="630">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="TINTOlib — Tabular Data → Synthetic Images">
<meta name="twitter:description" content="Convert tidy data into images and train CNNs/ViTs & hybrid models.">
<meta name="twitter:image" content="{{ site.url }}{{ page.image }}">

<!-- ✅ JSON-LD: Software -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "TINTOlib",
  "operatingSystem": "Linux, macOS, Windows",
  "applicationCategory": "Machine Learning Library",
  "description": "TINTOlib is a Python library that converts tabular (tidy) data into synthetic images using various algorithmic methods. It enables the use of CNNs, ViTs and hybrid models with tabular data.",
  "url": "{{ site.url }}{{ page.url }}",
  "image": "{{ site.url }}/images/tinto-logo.svg",
  "softwareVersion": "1.0",
  "author": { "@type": "Person", "name": "Manuel Castillo-Cara" },
  "publisher": { "@type": "Organization", "name": "Ontology Engineering Group, UPM" },
  "license": "https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE",
  "downloadUrl": "https://pypi.org/project/TINTOlib/",
  "codeRepository": "https://github.com/oeg-upm/TINTOlib",
  "programmingLanguage": "Python",
  "offers": { "@type": "Offer", "price": "0.00", "priceCurrency": "EUR" }
}
</script>

<!-- ✅ JSON-LD: FAQ -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    { "@type": "Question", "name": "What is TINTOlib?",
      "acceptedAnswer": { "@type": "Answer", "text": "A Python library that transforms tidy tabular data into synthetic images so you can use computer vision models (CNNs, Vision Transformers) on non-image data." } },
    { "@type": "Question", "name": "Which methods are supported?",
      "acceptedAnswer": { "@type": "Answer", "text": "TINTO, IGTD, REFINED, BarGraph, DistanceMatrix, Combination, SuperTML, FeatureWrap, BIE — each with specific hyperparameters." } },
    { "@type": "Question", "name": "Why convert tables into images?",
      "acceptedAnswer": { "@type": "Answer", "text": "It lets you leverage the advances of modern vision models on tabular problems, sometimes improving accuracy and generalization." } }
  ]
}
</script>

<!-- 🎨 Estilos (alineados con el resto del sitio) -->
<style>
  :root{
    --ink:#1f2937; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8;
    --cta:#2563eb; --cta-hover:#1d4ed8; --pill:#eef2ff;
  }
  .tinto-wrap{max-width:1050px;margin:0 auto;padding:0 1rem}
  .tinto-hero{
    display:flex; gap:1rem; align-items:center; flex-wrap:wrap;
    background:linear-gradient(135deg,#1d4ed8 0%, #9333ea 100%);
    color:#fff; border-radius:14px; padding:1rem 1.25rem; margin:1.25rem 0 1.2rem;
    box-shadow:0 8px 24px rgba(0,0,0,.08);
  }
  .tinto-hero img{width:90px;height:90px;background:#fff;border-radius:12px;padding:.35rem;border:2px solid rgba(255,255,255,.7);object-fit:contain}
  .tinto-hero h1{font-size:1.6rem;margin:.1rem 0 .25rem;line-height:1.2}
  .hero-actions{display:flex;justify-content:center;align-items:center;gap:.6rem;flex-wrap:wrap;margin-top:.6rem}
  .btn{display:inline-block;padding:.65em 1.05em;border-radius:10px;font-weight:800;text-decoration:none;border:0;cursor:pointer;transition:transform .06s ease, box-shadow .15s ease, background-color .15s ease}
  .btn:hover{transform:translateY(-1px);box-shadow:0 6px 16px rgba(0,0,0,.18)}
  .btn-primary{background:var(--cta);color:#fff !important}
  .btn-primary:hover{background:var(--cta-hover)}
  .btn-ghost{border:2px solid rgba(255,255,255,.85);color:#fff !important;background:transparent}
  .section-title{
    display:flex;align-items:center;gap:.5rem;font-size:1.25rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand); border-radius:12px; padding:.5rem .8rem; margin:1.2rem 0 .8rem;
  }
  .section-title::after{content:"";flex:1;height:3px;margin-left:.6rem;background:linear-gradient(to right,#4a90e2,#e91e63);border-radius:2px}
  .card{background:var(--card);border:1px solid var(--bd);border-radius:12px;padding:1rem;box-shadow:0 2px 10px rgba(0,0,0,.04)}
  .pillbar{display:flex;flex-wrap:wrap;gap:.5rem;margin:.6rem 0}
  .pill{display:inline-flex;align-items:center;gap:.35rem;font-weight:700;font-size:.88rem;background:var(--pill);border:1px solid var(--bd);color:#111827;border-radius:999px;padding:.2rem .6rem}
  .methods-table{width:100%;border-collapse:collapse;font-size:.95rem;margin:1rem 0}
  .methods-table th,.methods-table td{border:1px solid #e6e8eb;padding:.6rem .7rem;vertical-align:top}
  .methods-table th{background:#f3f6fb;text-align:left}
  .cta-center{display:flex;justify-content:center;margin:1.6rem 0}
  .cta-center .btn-primary{padding:1em 2.5em;font-size:1.1rem;min-width:clamp(240px,50vw,440px)}
  /* Aviso Udemy */
  .udemy-box{border:1px solid #cfd8dc;border-radius:12px;background:#f5f8fa;padding:1rem;margin:1rem 0 1.2rem}
  .udemy-box h2{color:#1565c0;margin:.2rem 0 .4rem;text-align:center}
  .udemy-box p{text-align:center;color:#37474f;margin:.25rem 0}
</style>

<div class="tinto-wrap">

  <!-- HERO -->
  <section class="tinto-hero">
    <img src="/images/tinto-logo.svg" alt="TINTOlib logo">
    <div style="flex:1">
      <h1>TINTOlib — Tabular Data → Synthetic Images</h1>
      <p>Open-source Python library to convert tidy tabular data into synthetic images and train CNNs, ViTs, and hybrid architectures.</p>
      <div class="hero-actions">
        <a class="btn btn-primary" href="https://github.com/oeg-upm/TINTOlib" target="_blank" rel="noopener">⭐ GitHub</a>
        <a class="btn btn-ghost" href="https://tintolib.readthedocs.io/en/latest/" target="_blank" rel="noopener">📘 Documentation</a>
      </div>
    </div>
  </section>

  <!-- Aviso Udemy (conservado) -->
  <div class="udemy-box">
    <h2>🎉 New Free Course on Udemy! 🎉</h2>
    <p>We’ve just launched a <strong>100% free course on Udemy</strong> about using <strong>TINTOlib</strong> and developing <strong>Hybrid Neural Networks</strong>.</p>
    <p>Learn how to turn tabular data into synthetic images and apply CNNs, ViTs, and hybrid architectures.</p>
    <p>
      <a class="btn btn-primary" href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" target="_blank" rel="noopener">
        👉 Access the Course on Udemy
      </a>
    </p>
  </div>

  <!-- Logo centrado adicional (conservado del original) -->
  <p style="text-align:center;margin:.6rem 0 1rem">
    <img src="/images/tinto-logo.svg" alt="TINTO Logo" width="170">
  </p>

  <!-- Overview -->
  <div class="card">
    <h2 class="section-title">🧠 Overview</h2>
    <p><strong>TINTOlib</strong> transforms <strong>tidy tabular data</strong> into <strong>synthetic images</strong>, enabling deep learning with <strong>CNNs</strong> and <strong>Vision Transformers (ViTs)</strong> for classification and regression. It bridges structured data and image-based learning, and supports hybrid models combining both worlds.</p>
    <div class="pillbar">
      <span class="pill">📦 pip install TINTOlib</span>
      <span class="pill">🖥️ Linux / Windows / macOS</span>
      <span class="pill">🐍 Python 3.7+</span>
      <span class="pill">🧪 CSV / Pandas DataFrame</span>
    </div>
  </div>

  <!-- ======== TINTOlib: Overview Video (ES/EN) ======== -->
<div class="card">
  <h2 class="section-title">🎬 TINTOlib — Overview Video</h2>

  <div class="video-toggle" role="tablist" aria-label="Select video language">
    <button class="vt-btn active" data-target="#video-es" role="tab" aria-selected="true">Español</button>
    <button class="vt-btn" data-target="#video-en" role="tab" aria-selected="false">English</button>
  </div>

  <div class="video-wrap">
    <video id="video-es" class="vpanel active"
           controls controlsList="nodownload"
           preload="metadata" playsinline
           aria-label="TINTOlib — Vídeo en español">
      <source src="/video/TINTOlib-video-Es.mp4" type="video/mp4">
      Tu navegador no soporta el vídeo.
      <a href="/video/TINTOlib-video-Es.mp4">Descargar (ES)</a>.
    </video>

    <video id="video-en" class="vpanel"
           controls controlsList="nodownload"
           preload="metadata" playsinline
           aria-label="TINTOlib — Video in English">
      <source src="/video/TINTOlib-video-En.mp4" type="video/mp4">
      Your browser does not support the video tag.
      <a href="/video/TINTOlib-video-En.mp4">Download (EN)</a>.
    </video>
  </div>

  <style>
    .video-toggle{display:flex;gap:.5rem;flex-wrap:wrap;margin:.6rem 0 1rem}
    .vt-btn{
      background:#eef2ff;border:1px solid #dbe3ff;color:#1f2937;
      font-weight:800;border-radius:999px;padding:.35rem .8rem;cursor:pointer
    }
    .vt-btn.active{background:#2563eb;color:#fff;border-color:#2563eb}
    .video-wrap{position:relative;width:100%;max-width:900px;margin:0 auto}
    .vpanel{display:none;width:100%;height:auto;border:1px solid #d0d7de;border-radius:12px;box-shadow:0 2px 8px rgba(0,0,0,.06);background:#000}
    .vpanel.active{display:block}
    .video-wrap video.vpanel{aspect-ratio:16/9;object-fit:cover}
  </style>

  <script>
    document.addEventListener('DOMContentLoaded', function(){
      const buttons = document.querySelectorAll('.video-toggle .vt-btn');
      const panels  = document.querySelectorAll('#video-es, #video-en');
      buttons.forEach(btn=>{
        btn.addEventListener('click', ()=>{
          buttons.forEach(b=>{ b.classList.remove('active'); b.setAttribute('aria-selected','false'); });
          btn.classList.add('active'); btn.setAttribute('aria-selected','true');
          const target = btn.getAttribute('data-target');
          panels.forEach(p=>{
            if(('#'+p.id) === target){
              p.classList.add('active');
            } else {
              if(p.tagName.toLowerCase()==='video'){ try{ p.pause(); }catch(e){} }
              p.classList.remove('active');
            }
          });
        });
      });
    });
  </script>
</div>

  <!-- Videotutorial GitHub (conservado) -->
  <div class="card">
    <h2 class="section-title">📺 VideoTutorial Course (English/Spanish)</h2>
    <p>Prefer not to register on Udemy or looking for the English version? Follow the full bilingual course on GitHub, with videos and practical notebooks covering CNNs, ViTs, and hybrid architectures.</p>
    <p style="text-align:center;margin:.4rem 0 0">
      <a href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">
        <img src="https://img.shields.io/badge/GitHub-VideoTutorial%20Course-black?style=for-the-badge&logo=GitHub&logoColor=white" alt="Access the Course on GitHub">
      </a>
    </p>
  </div>

    <!-- Benchmark Section -->
  <div class="card">
    <h2 class="section-title">📊 Benchmark of TINTOlib vs Classical Models</h2>
    <p>
      This benchmark compares <strong>TINTOlib</strong> transformation methods and neural architectures 
      against traditional and ensemble models on multiple datasets.  
      You can explore the interactive version directly on the official site.
    </p>

    <!-- 🔵 Botón centrado -->
    <div style="text-align:center; margin:20px 0;">
      <a href="https://oeg-upm.github.io/TINTOlib/" 
        target="_blank" 
        rel="noopener" 
        style="display:inline-block; background-color:#2563eb; color:#fff; font-weight:600; 
                padding:12px 24px; border-radius:8px; text-decoration:none; box-shadow:0 2px 6px rgba(0,0,0,.2);">
        🌐 Visit TINTOlib Benchmark Page
      </a>
    </div>

    <div style="position:relative; padding-bottom:65%; height:0; overflow:hidden; border-radius:12px; box-shadow:0 2px 10px rgba(0,0,0,.15); border:1px solid #e5e7eb;">
      <iframe 
        src="https://oeg-upm.github.io/TINTOlib/"
        style="position:absolute; top:0; left:0; width:100%; height:100%; border:0;"
        title="TINTOlib Benchmark"
        loading="lazy"
        allowfullscreen>
      </iframe>
    </div>
  </div>

  <!-- Features -->
  <div class="card">
    <h2 class="section-title">🔧 Features</h2>
    <ul style="margin:.35rem 0 0; padding-left:1.1rem">
      <li>Input formats: <strong>CSV</strong> or <strong>Pandas DataFrame</strong>.</li>
      <li>Designed for tidy data (<em>target</em> column at the end).</li>
      <li>Output: grayscale images produced by reduction/transformation methods.</li>
      <li>Compatible with <strong>Linux</strong>, <strong>Windows</strong>, <strong>macOS</strong>.</li>
      <li>Requires <strong>Python 3.7+</strong>.</li>
    </ul>
  </div>

  <!-- Supported Models (tabla conservada y mejorada) -->
  <div class="card">
    <h2 class="section-title">🧪 Supported Models</h2>
    <p>Supported image transformation models include:</p>
    <table class="methods-table">
      <thead>
        <tr><th style="width:26%">Models</th><th style="width:12%">Class</th><th style="width:62%">Hyperparameters</th></tr>
      </thead>
      <tbody>
        <tr><td><a href="https://github.com/oeg-upm/TINTO" target="_blank" rel="noopener">TINTO</a></td><td><code>TINTO()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>pixels</code> <code>algorithm</code> <code>blur</code> <code>submatrix</code> <code>amplification</code> <code>distance</code> <code>steps</code> <code>option</code> <code>times</code> <code>train_m</code> <code>zoom</code> <code>random_seed</code></td></tr>
        <tr><td><a href="https://github.com/zhuyitan/igtd" target="_blank" rel="noopener">IGTD</a></td><td><code>IGTD()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>scale</code> <code>fea_dist_method</code> <code>image_dist_method</code> <code>error</code> <code>max_step</code> <code>val_step</code> <code>switch_t</code> <code>min_gain</code> <code>zoom</code> <code>random_seed</code></td></tr>
        <tr><td><a href="https://github.com/omidbazgirTTU/REFINED" target="_blank" rel="noopener">REFINED</a></td><td><code>REFINED()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>hcIterations</code> <code>n_processors</code> <code>zoom</code> <code>random_seed</code></td></tr>
        <tr><td><a href="https://github.com/anuraganands/Non-image-data-classification-with-CNN/" target="_blank" rel="noopener">BarGraph</a></td><td><code>BarGraph()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>pixel_width</code> <code>gap</code> <code>zoom</code></td></tr>
        <tr><td><a href="https://github.com/anuraganands/Non-image-data-classification-with-CNN/" target="_blank" rel="noopener">DistanceMatrix</a></td><td><code>DistanceMatrix()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>zoom</code></td></tr>
        <tr><td><a href="https://github.com/anuraganands/Non-image-data-classification-with-CNN/" target="_blank" rel="noopener">Combination</a></td><td><code>Combination()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>zoom</code></td></tr>
        <tr><td><a href="https://github.com/GilesStrong/SuperTML_HiggsML_Test" target="_blank" rel="noopener">SuperTML</a></td><td><code>SuperTML()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>pixels</code> <code>feature_importance</code> <code>font_size</code> <code>random_seed</code></td></tr>
        <tr><td><a href="https://link.springer.com/chapter/10.1007/978-3-319-70139-4_87" target="_blank" rel="noopener">FeatureWrap</a></td><td><code>FeatureWrap()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>size</code> <code>bins</code> <code>zoom</code></td></tr>
        <tr><td><a href="https://ieeexplore.ieee.org/document/10278393" target="_blank" rel="noopener">BIE</a></td><td><code>BIE()</code></td><td><code>problem</code> <code>normalize</code> <code>verbose</code> <code>precision</code> <code>zoom</code></td></tr>
      </tbody>
    </table>
  </div>

  <!-- Getting Started -->
  <div class="card">
    <h2 class="section-title">🚀 Getting Started</h2>
    <p>Install via <code>pip</code>:</p>
<pre><code class="language-bash">pip install TINTOlib
</code></pre>
    <ul style="margin:.35rem 0 0; padding-left:1.1rem">
      <li>Use <code>requirements.txt</code> for the base environment.</li>
      <li>Use <code>requirements-example.txt</code> for full deep learning workflows.</li>
    </ul>

    <h3 style="margin:1rem 0 .4rem;font-weight:800">🧩 Example</h3>
<pre><code class="language-python">from TINTOlib.tinto import TINTO

# Create and run TINTO on your tidy DataFrame (target column last)
model = TINTO(problem="supervised", blur=True, pixels=64, random_seed=42)
model.fit_transform(data, folder="outputs")
</code></pre>

<!-- Recursos adicionales -->
<div class="card">
  <h2 class="section-title">📚 Additional Resources</h2>
  
  <div class="pillbar" style="display:flex; justify-content:center; gap:10px;">
    <a class="pill" href="https://tintolib.readthedocs.io/en/latest/" target="_blank" rel="noopener">📘 Documentation</a>
    <a class="pill" href="https://github.com/oeg-upm/TINTOlib" target="_blank" rel="noopener">🚀 GitHub</a>
    <a class="pill" href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">📹 Crash Course</a>
  </div>
  
</div>
  </div>

  <!-- Cite -->
  <div class="card">
    <h2 class="section-title">🧠 Research and Software Publications</h2>
      <h3 style="margin:.25rem 0">📄 Research Articles</h3>
      <ul class="pub-list">
        <li>Manuel Castillo-Cara et al. <strong>MIMO-Based Indoor Localisation with Hybrid Neural Networks</strong>. <em>IEEE JSTSP</em>. DOI: <a href="https://doi.org/10.1109/JSTSP.2025.3555067" target="_blank" rel="noopener">10.1109/JSTSP.2025.3555067</a></li>
        <li>Reewos Talla-Chumpitaz, Manuel Castillo-Cara et al. <strong>Blurring Image Techniques for Bluetooth-based Indoor Localisation</strong>. <em>Information Fusion</em>. DOI: <a href="https://doi.org/10.1016/j.inffus.2022.10.011" target="_blank" rel="noopener">10.1016/j.inffus.2022.10.011</a></li>
      </ul>
      <h3 style="margin:.5rem 0 0">💾 Software Articles</h3>
      <ul class="pub-list">
        <li>Jiayun Liu et al. <strong>TINTOlib: A Python library for transforming tabular data into synthetic images for deep neural networks</strong>. <em>SoftwareX</em>. DOI: <a href="https://doi.org/10.1016/j.softx.2025.102444" target="_blank" rel="noopener">10.1016/j.softx.2025.102444</a></li>
        <li>Manuel Castillo-Cara et al. <strong>TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks</strong>. <em>SoftwareX</em>. DOI: <a href="https://doi.org/10.1016/j.softx.2023.101391" target="_blank" rel="noopener">10.1016/j.softx.2023.101391</a></li>
      </ul>
  </div>

  <div class="card">
    <h2 class="section-title">🎓 License</h2>
    <p>TINTOlib is released under the <strong>Apache License 2.0</strong>.</p>
  </div>

  <div class="card">
    <h2 class="section-title">👥 Authors</h2>
    <ul style="margin:.35rem 0 0; padding-left:1.1rem">
      <li><a href="https://github.com/manwestc" target="_blank" rel="noopener">Manuel Castillo-Cara</a></li>
      <li><a href="https://github.com/rgcmme" target="_blank" rel="noopener">Raúl García-Castro</a></li>
      <li><a href="https://github.com/DavidGonzalezFernandez" target="_blank" rel="noopener">David González Fernández</a></li>
      <li><a href="https://github.com/DCY1117" target="_blank" rel="noopener">Jiayun Liu</a></li>
    </ul>
  </div>

    <div class="card">
    <h2 class="section-title">🏛️ Institutions</h2>
    <p style="text-align:center;margin:.4rem 0 0">
      <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-oeg.png" alt="Ontology Engineering Group" width="130" style="margin:.35rem">
      <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-upm.png" alt="UPM" width="130" style="margin:.35rem">
      <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uned-.jpg" alt="UNED" width="130" style="margin:.35rem">
      <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uclm.png" alt="UCLM" width="130" style="margin:.35rem">
    </p>
  </div>

    <div class="cta-center">
    <a class="btn btn-primary" href="https://pypi.org/project/TINTOlib/" target="_blank" rel="noopener">⬇️ Install from PyPI</a>
  </div>
</div>



