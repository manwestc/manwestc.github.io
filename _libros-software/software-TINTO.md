---
layout: single
title: "TINTO — Transform Tabular Data into Synthetic Images for Deep Neural Networks"
excerpt: "Open-source framework to convert tidy tabular data into synthetic images (PCA, t-SNE, blurring) for CNN-based classification."
collection: libros-software
category: "Software"
permalink: /libros-software/software-TINTO/
image: "/images/tinto-logo.svg"
author_profile: true
show_date: false
read_time: false
share: false
related: false
description: "TINTO is an open-source Python framework that converts tidy tabular data into synthetic images using PCA, t-SNE and blurring to enable CNN-based classification."
---

{% include base_path %}

<!-- ✅ Canonical + basic SEO -->
<link rel="canonical" href="{{ site.url }}{{ page.permalink }}">
<meta name="robots" content="index,follow">
<meta name="description" content="TINTO is an open-source framework to transform tidy tabular data into synthetic images (PCA, t-SNE, blurring) for deep learning with CNNs.">
<meta name="keywords" content="TINTO, TINTOlib, tabular to image, tidy data, synthetic images, PCA, t-SNE, blurring, deep learning, CNN">

<!-- ✅ Open Graph / Twitter -->
<meta property="og:title" content="TINTO — Tabular Data → Synthetic Images for Deep Learning">
<meta property="og:description" content="Convert tidy tabular data into synthetic images with PCA, t-SNE and blurring. Open-source, Python, CNN-ready.">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}{{ page.permalink }}">
<meta property="og:image" content="{{ site.url }}{{ page.image }}">
<meta property="og:image:width" content="1200"><meta property="og:image:height" content="630">

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="TINTO — Tabular Data → Synthetic Images">
<meta name="twitter:description" content="Open-source Python framework to turn tidy data into images for CNNs.">
<meta name="twitter:image" content="{{ site.url }}{{ page.image }}">

<!-- 🎨 Styles (coherentes con cursos) -->
<style>
  :root{
    --ink:#1f2937; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8;
    --cta:#2563eb; --cta-hover:#1d4ed8; --cta-soft:#eaf1ff;
  }
  .wrap{max-width:1050px;margin:0 auto;padding:0 1rem}
  /* Ocultar meta del theme */
  .page__meta, .page__meta-title, .page__taxonomy, .page__date{display:none !important;}

  /* HERO */
  .hero{
    display:flex; gap:1rem; align-items:center; flex-wrap:wrap;
    background:linear-gradient(135deg,#1d4ed8 0%, #9333ea 100%);
    color:#fff; border-radius:14px; padding:1rem 1.25rem; margin:1.25rem 0 1rem;
    box-shadow:0 8px 24px rgba(0,0,0,.08);
  }
  .hero img{width:84px;height:84px;border-radius:12px;background:#fff;padding:.35rem;border:2px solid rgba(255,255,255,.6)}
  .hero h1{font-size:1.65rem;line-height:1.2;margin:.1rem 0 .25rem}
  .hero p{margin:0;opacity:.95}
  .hero-actions{display:flex;justify-content:center;gap:.6rem;flex-wrap:wrap;margin-top:.7rem}

  /* Botones */
  .btn{display:inline-block;padding:.65em 1.05em;border-radius:10px;font-weight:800;text-decoration:none;border:0;cursor:pointer;transition:transform .06s ease,box-shadow .15s ease,background-color .15s ease}
  .btn:hover{transform:translateY(-1px);box-shadow:0 6px 16px rgba(0,0,0,.18)}
  .btn-primary{background:var(--cta);color:#fff !important}
  .btn-primary:hover{background:var(--cta-hover)}
  .btn-ghost{background:#1e40af;color:#fff !important}
  .btn-ghost:hover{background:#1e3a8a}

  /* Secciones */
  .card{background:var(--card);border:1px solid var(--bd);border-radius:12px;padding:1rem;box-shadow:0 2px 10px rgba(0,0,0,.04);margin:1rem 0}
  .section-title{
    display:flex;align-items:center;gap:.5rem;font-size:1.25rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);border-left:6px solid var(--brand);
    border-radius:12px;padding:.5rem .8rem;margin:1.3rem 0 .8rem;
  }
  .section-title::after{content:"";flex:1;height:3px;margin-left:.6rem;background:linear-gradient(to right,#4a90e2,#e91e63);border-radius:2px}
  .list{margin:.35rem 0 0;padding-left:1.1rem}
  .list li{margin:.28rem 0;line-height:1.55}

  /* Tabla simple */
  table{width:100%;border-collapse:collapse;margin:.6rem 0 1rem}
  th,td{border:1px solid #e6e8eb;padding:.55rem .65rem}
  th{background:#f3f6fb;text-align:left}

  /* CTA inferior grande */
  .cta-center{display:flex;justify-content:center;margin:2rem 0}
  .cta-center .btn-primary{padding:1em 2.5em;font-size:1.15rem;min-width:clamp(240px,48vw,420px)}
  /* === Callout / Aviso importante === */
  .callout{
    display:flex; gap:.8rem; align-items:flex-start;
    border:1px solid #f2e8c6;               /* borde suave ámbar */
    border-left:6px solid #d97706;          /* acento ámbar oscuro */
    background:linear-gradient(180deg,#fffef8,#fff7e6);
    border-radius:12px; padding:1rem 1.1rem; 
    box-shadow:0 2px 10px rgba(0,0,0,.04); margin:1rem 0;
  }
  .callout .ico{
    flex:0 0 34px; width:34px; height:34px; border-radius:8px;
    display:inline-flex; align-items:center; justify-content:center;
    background:#fff3cd; color:#92400e; font-size:18px;
    border:1px solid #fde68a;
  }
  .callout h3{
    margin:.1rem 0 .35rem; font-size:1.05rem; font-weight:800; color:var(--ink);
  }
  .callout p{ margin:.25rem 0; color:#1f2937 }
  .callout ul{ margin:.4rem 0 .2rem .95rem }
  .callout li{ margin:.2rem 0; line-height:1.5 }
  .callout a{ color:#0b67b8; font-weight:800; text-decoration:none }
  .callout a:hover{ text-decoration:underline }
</style>

<div class="wrap">
  <!-- HERO -->
  <section class="callout" role="note" aria-label="Important notice about TINTO">
    <span class="ico" aria-hidden="true">⚠️</span>
    <div>
      <h3>Important Notice</h3>
      <p>
        This repository contains the original implementation of <strong>TINTO</strong>, an engine for converting tidy tabular data into synthetic images using dimensionality reduction and convolution techniques.
      </p>
      <p>
        📦 <strong>We strongly recommend using the updated library 
        <a href="https://github.com/oeg-upm/TINTOlib" target="_blank" rel="noopener">TINTOlib</a></strong>, which includes:
      </p>
      <ul>
        <li>The original <strong>TINTO</strong> method</li>
        <li>Additional methods: <strong>IGTD</strong>, <strong>REFINED</strong>, <strong>BarGraph</strong>, <strong>DistanceMatrix</strong>, <strong>Combination</strong>, <strong>FeatureWrap</strong>, <strong>SuperTML</strong>, and <strong>BIE</strong></li>
        <li>A more user-friendly and flexible interface</li>
        <li>Complete and regularly updated documentation</li>
        <li>A free course with examples, notebooks, and video tutorials</li>
      </ul>
      <p>🔄 <strong>TINTOlib</strong> is under active development and continues to receive improvements.</p>
      <p>👉 For new projects, we highly recommend switching to 
        <a href="https://github.com/oeg-upm/TINTOlib" target="_blank" rel="noopener">TINTOlib</a>.
      </p>
    </div>
  </section>

  <section class="hero">
    <img src="/images/tinto-logo.svg" alt="TINTO logo" loading="lazy">
    <div style="flex:1">
      <h1>TINTO — Tabular Data → Synthetic Images</h1>
      <p>Open-source Python framework that turns tidy tabular data into images using PCA, t-SNE and blurring — ready for CNN pipelines.</p>
      <div class="hero-actions">
        <a class="btn btn-primary" href="https://github.com/oeg-upm/TINTO" target="_blank" rel="noopener">⭐ GitHub</a>
        <a class="btn btn-ghost" href="#features">Ver características</a>
        <a class="btn btn-primary" href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" target="_blank" rel="noopener">🎓 Curso gratuito (Udemy)</a>
      </div>
    </div>
  </section>

  <!-- Aviso curso -->
  <section class="card" style="text-align:center">
    <h2 class="section-title" style="justify-content:center">🎉 Free Course: TINTOlib & Hybrid Neural Networks</h2>
    <p>Learn how to convert tabular data into images and train CNNs, ViTs and hybrid architectures.</p>
    <a class="btn btn-primary" href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" target="_blank" rel="noopener">👉 Access on Udemy</a>
  </section>

  <!-- Abstract -->
  <section class="card">
    <h2 class="section-title">🔎 Abstract</h2>
    <p><strong>TINTO</strong> is an open-source, user-extendable framework to convert <em>tidy data</em> into images via 2-D projection (PCA, t-SNE) and a <em>blurring</em> technique that adds ordered information, often improving CNN classification.</p>
    <p style="text-align:center">
      <img src="/images/tinto-framework.png" alt="TINTO framework diagram" style="max-width:680px;width:100%;border:1px solid var(--bd);border-radius:10px">
    </p>
  </section>

  <!-- VideoTutorial en GitHub -->
  <section class="card">
    <h2 class="section-title">📺 VideoTutorial Course (English/Spanish)</h2>
    <p>Prefer GitHub over Udemy? Follow the full bilingual course with notebooks:</p>
    <p style="text-align:center">
      <a href="./5_TINTOlib%20Videotutorial%20course/README.md" target="_blank" rel="noopener">
        <img src="https://img.shields.io/badge/GitHub-VideoTutorial%20Course-black?style=for-the-badge&logo=GitHub&logoColor=white" alt="Access the Course on GitHub">
      </a>
    </p>
  </section>

  <!-- Docs -->
  <section class="card">
    <h2 class="section-title">📄 Documentation</h2>
    <p>All documentation and source code are available in the <a href="https://github.com/oeg-upm/TINTO" target="_blank" rel="noopener">OEG GitHub repository</a>.</p>
  </section>

  <!-- Video -->
  <section class="card">
    <h2 class="section-title">🎬 Video Example</h2>
    <div style="text-align:center">
      <video width="500" controls>
        <source src="https://user-images.githubusercontent.com/102165947/212918739-89fca790-3360-4a8c-89b7-443f294fba6f.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
  </section>

  <!-- Features -->
  <section id="features" class="card">
    <h2 class="section-title">🔍 Main Features</h2>
    <ul class="list">
      <li>Works with CSV files in <strong>Tidy Data</strong> format.</li>
      <li>Input: numeric features; target in the last column.</li>
      <li>Projection methods: <strong>PCA</strong> and <strong>t-SNE</strong>.</li>
      <li>Output: black-and-white synthetic images.</li>
      <li><em>Blurring</em> technique for pixel blending.</li>
      <li>Python 3.7+, Linux/Windows/macOS.</li>
    </ul>
  </section>

  <!-- Input -->
  <section class="card">
    <h2 class="section-title">📥 Input</h2>
    <p>Example (IRIS dataset format):</p>
    <table>
      <thead><tr><th>sepal length</th><th>sepal width</th><th>petal length</th><th>petal width</th><th>target</th></tr></thead>
      <tbody>
        <tr><td>4.9</td><td>3.0</td><td>1.4</td><td>0.2</td><td>1</td></tr>
        <tr><td>7.0</td><td>3.2</td><td>4.7</td><td>1.4</td><td>2</td></tr>
        <tr><td>6.3</td><td>3.3</td><td>6.0</td><td>2.5</td><td>3</td></tr>
      </tbody>
    </table>
  </section>

  <!-- Output -->
  <section class="card">
    <h2 class="section-title">🖼️ Output</h2>
    <p style="text-align:center">
      <img src="/images/tinto1.png" alt="TINTO output example" width="280" style="border:1px solid var(--bd);border-radius:10px">
    </p>
  </section>

  <!-- Citations -->
  <section class="card">
    <h2 class="section-title">📖 Citation</h2>
    <p>If you used <strong>TINTOlib with Hybrid Neural Networks</strong>, cite the IEEE JSTSP paper:</p>
<pre><code>@ARTICLE{10946146,
  author={Castillo-Cara, Manuel and Martínez-Gómez, Jesus and Ballesteros-Jerez, Javier and García-Varea, Ismael and García-Castro, Raúl and Orozco-Barbosa, Luis},
  journal={IEEE Journal of Selected Topics in Signal Processing},
  title={MIMO-Based Indoor Localisation with Hybrid Neural Networks: Leveraging Synthetic Images from Tidy Data for Enhanced Deep Learning},
  year={2025},
  pages={1-13},
  doi={10.1109/JSTSP.2025.3555067}
}</code></pre>

    <p>If you used <strong>TINTO</strong>, cite the Information Fusion paper:</p>
<pre><code>@article{inffus_TINTO,
  title   = {A novel deep learning approach using blurring image techniques for Bluetooth-based indoor localisation},
  journal = {Information Fusion},
  author  = {Reewos Talla-Chumpitaz and Manuel Castillo-Cara and Luis Orozco-Barbosa and Raúl García-Castro},
  volume  = {91},
  pages   = {173-186},
  year    = {2023},
  issn    = {1566-2535},
  doi     = {10.1016/j.inffus.2022.10.011}
}</code></pre>

    <p>And the <strong>SoftwareX</strong> paper:</p>
<pre><code>@article{softwarex_TINTO,
  title   = {TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks},
  journal = {SoftwareX},
  author  = {Manuel Castillo-Cara and Reewos Talla-Chumpitaz and Raúl García-Castro and Luis Orozco-Barbosa},
  year    = {2023},
  volume  = {22},
  pages   = {101391},
  issn    = {2352-7110},
  doi     = {10.1016/j.softx.2023.101391}
}</code></pre>
  </section>

  <!-- CTA inferior -->
  <div class="cta-center">
    <a class="btn btn-primary" href="https://github.com/oeg-upm/TINTO" target="_blank" rel="noopener">⭐ Ver repositorio en GitHub</a>
  </div>
</div>

<!-- ✅ JSON-LD Software -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "TINTO",
  "operatingSystem": "Linux, macOS, Windows",
  "applicationCategory": "Machine Learning Library",
  "description": "TINTO is an open-source Python framework that transforms tidy tabular data into black-and-white images using PCA, t-SNE and blurring techniques for CNN-based classification.",
  "url": "{{ site.url }}{{ page.permalink }}",
  "image": "{{ site.url }}{{ page.image }}",
  "softwareVersion": "1.0",
  "author": { "@type": "Person", "name": "Manuel Castillo-Cara" },
  "publisher": { "@type": "Organization", "name": "Ontology Engineering Group, UPM" },
  "license": "https://github.com/oeg-upm/TINTO/blob/main/LICENSE",
  "codeRepository": "https://github.com/oeg-upm/TINTO",
  "programmingLanguage": "Python",
  "offers": { "@type": "Offer", "price": "0.00", "priceCurrency": "EUR" }
}
</script>