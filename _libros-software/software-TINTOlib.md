---
layout: single
title: "TINTOlib — Python library for transforming tabular data into synthetic images"
collection: libros-software
category: "Software"
permalink: /libros-software/software-TINTOlib/
image: "/images/tinto-logo.svg"
description: "TINTOlib is an open-source, user-extendable framework that converts tidy tabular data into synthetic images for deep learning with CNNs, ViTs, and hybrid models."
show_date: false
read_time: false
share: false
related: false
---

{% include base_path %}

<!-- ✅ SEO básico -->
<link rel="canonical" href="{{ site.url }}{{ page.permalink }}">
<meta name="robots" content="index,follow">
<meta name="description" content="TINTOlib is a Python library that converts tidy data into synthetic images for deep learning models like CNNs and Vision Transformers.">

<!-- ✅ Open Graph / Twitter -->
<meta property="og:title" content="TINTOlib — Tabular Data to Synthetic Images">
<meta property="og:description" content="Convert tidy tabular data into synthetic images for deep learning with CNNs, ViTs, and hybrid models.">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}{{ page.permalink }}">
<meta property="og:image" content="{{ site.url }}{{ page.image }}">
<meta property="og:image:width" content="1200"><meta property="og:image:height" content="630">

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="TINTOlib — Tabular Data to Synthetic Images">
<meta name="twitter:description" content="Open-source Python library to transform tabular data into synthetic images for advanced deep learning.">
<meta name="twitter:image" content="{{ site.url }}{{ page.image }}">

<!-- ✅ JSON-LD -->
<script type="application/ld+json">
{
  "@context":"https://schema.org",
  "@type":"SoftwareApplication",
  "name":"TINTOlib",
  "operatingSystem":"Linux, macOS, Windows",
  "applicationCategory":"Machine Learning Library",
  "description":"TINTOlib converts tidy tabular data into synthetic images, enabling the use of CNNs, ViTs, and hybrid deep learning models.",
  "url":"{{ site.url }}{{ page.url }}",
  "image":"{{ site.url }}{{ page.image }}",
  "softwareVersion":"1.0",
  "author":{"@type":"Person","name":"Manuel Castillo-Cara"},
  "publisher":{"@type":"Organization","name":"Ontology Engineering Group, UPM"},
  "license":"https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE",
  "downloadUrl":"https://pypi.org/project/TINTOlib/",
  "codeRepository":"https://github.com/oeg-upm/TINTOlib",
  "programmingLanguage":"Python",
  "offers":{"@type":"Offer","price":"0.00","priceCurrency":"EUR"}
}
</script>

<!-- 🎨 Estilos -->
<style>
  .hero {display:flex;gap:1rem;align-items:center;flex-wrap:wrap;background:linear-gradient(135deg,#1d4ed8 0%,#9333ea 100%);color:#fff;border-radius:14px;padding:1rem 1.25rem;margin:1.25rem 0 1rem;box-shadow:0 8px 24px rgba(0,0,0,.08);}
  .hero img{width:120px;height:120px;object-fit:contain;background:#fff;border-radius:12px;padding:.4rem;}
  .hero h1{font-size:1.6rem;margin:.1rem 0 .3rem;}
  .hero-actions{display:flex;gap:.6rem;flex-wrap:wrap;margin-top:.8rem;}
  .btn{display:inline-block;padding:.65em 1.05em;border-radius:10px;font-weight:800;text-decoration:none;transition:transform .06s ease,box-shadow .15s ease;background:#2563eb;color:#fff;}
  .btn:hover{background:#1d4ed8;transform:translateY(-1px);}
  .btn-secondary{background:#1e40af;}
  .btn-secondary:hover{background:#1e3a8a;}
  .section-title{font-size:1.25rem;font-weight:800;margin:1.3rem 0 .8rem;border-left:6px solid #1565c0;padding-left:.8rem;}
  .card{background:#fff;border:1px solid #e5e7eb;border-radius:12px;padding:1rem;box-shadow:0 2px 10px rgba(0,0,0,.04);}
</style>

<!-- HERO -->
<section class="hero">
  <img src="{{ page.image }}" alt="TINTOlib Logo">
  <div style="flex:1">
    <h1>TINTOlib — Python library for transforming tabular data into synthetic images</h1>
    <p>Convert tidy data into synthetic images for CNNs, ViTs, and hybrid deep learning models.</p>
    <div class="hero-actions">
      <a href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" target="_blank" class="btn">🚀 Access Free Udemy Course</a>
      <a href="https://github.com/oeg-upm/TINTOlib" target="_blank" class="btn btn-secondary">View on GitHub</a>
    </div>
  </div>
</section>

<!-- OVERVIEW -->
<div class="card">
  <h2 class="section-title">🧠 Overview</h2>
  <p><strong>TINTOlib</strong> is an open-source Python library that transforms <em>tidy tabular data</em> into <em>synthetic images</em>, enabling the use of deep learning models like <strong>CNNs</strong> and <strong>Vision Transformers</strong>. Ideal for tasks such as classification and regression.</p>
</div>

<!-- FEATURES -->
<div class="card">
  <h2 class="section-title">🔧 Features</h2>
  <ul>
    <li>Input formats: CSV or Pandas DataFrame</li>
    <li>Designed for tidy data (target column last)</li>
    <li>Output: grayscale synthetic images from multiple algorithms</li>
    <li>Cross-platform: Linux, Windows, macOS</li>
    <li>Requires Python 3.7+</li>
  </ul>
</div>

<!-- GETTING STARTED -->
<div class="card">
  <h2 class="section-title">🚀 Getting Started</h2>
  <pre><code>pip install TINTOlib</code></pre>
  <p>Use <code>requirements.txt</code> for the base environment or <code>requirements-example.txt</code> for deep learning workflows.</p>
</div>

<!-- CITE -->
<div class="card">
  <h2 class="section-title">📚 Citation</h2>
  <p>If you use TINTOlib, please cite our papers:</p>
  <ul>
    <li><a href="https://doi.org/10.1109/JSTSP.2025.3555067" target="_blank">IEEE Journal of Selected Topics in Signal Processing (2025)</a></li>
    <li><a href="https://doi.org/10.1016/j.softx.2023.101391" target="_blank">SoftwareX (2023)</a></li>
    <li><a href="https://doi.org/10.1016/j.inffus.2022.10.011" target="_blank">Information Fusion (2023)</a></li>
  </ul>
</div>