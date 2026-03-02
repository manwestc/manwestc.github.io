---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
description: "University teaching, thesis supervision, and technical training by Manuel Castillo-Cara at undergraduate, master’s and doctoral levels."
---

{% include base_path %}

<!-- ✅ Open Graph / Twitter Card -->
<meta property="og:title" content="Teaching – Manuel Castillo-Cara">
<meta property="og:description" content="University teaching, thesis supervision, and technical training at undergraduate, master's and doctoral levels by Manuel Castillo-Cara in AI, Data Science and Deep Learning.">
<meta property="og:image" content="https://www.manuelcastillo.eu/images/profile.jpg">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}{{ page.url }}">

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Teaching – Manuel Castillo-Cara">
<meta name="twitter:description" content="University teaching, thesis supervision, and technical training by Manuel Castillo-Cara in AI, Data Science and Deep Learning.">
<meta name="twitter:image" content="https://www.manuelcastillo.eu/images/profile.jpg">

<!-- ✅ SEO Structured Data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebPage",
  "name": "Teaching – Manuel Castillo-Cara",
  "description": "University teaching, thesis supervision, and technical training by Manuel Castillo-Cara at undergraduate, master's and doctoral levels in AI, Data Science and Deep Learning.",
  "url": "{{ site.url }}{{ page.url }}",
  "image": "https://www.manuelcastillo.eu/images/profile.jpg",
  "mainEntityOfPage": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "jobTitle": "Professor & Researcher",
    "image": "https://www.manuelcastillo.eu/images/profile.jpg",
    "hasCredential": "PhD in Computer Science",
    "affiliation": {
      "@type": "EducationalOrganization",
      "name": "Universidad Nacional de Educación a Distancia (UNED)"
    },
    "sameAs": [
      "https://www.manuelcastillo.eu/",
      "https://scholar.google.es/citations?user=r0JytwIAAAAJ",
      "https://www.scopus.com/authid/detail.uri?authorId=57200871251",
      "https://www.webofscience.com/wos/author/record/O-9762-2017",
      "https://www.linkedin.com/in/manuelcastillocara/"
    ]
  }
}
</script>

<style>
  /* ==== Teaching: estilos unificados (alineados con Publications) ==== */
  :root{
    --ink:#1f2937; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0;
  }
  .teach-page{max-width:1050px;margin:0 auto;padding:0 1rem}
  .teach-page h1, .teach-page h2, .teach-page h3 { color: var(--ink); }

  /* Título de sección con barrita */
  .section-title{
    display:flex;align-items:center;gap:.5rem;
    font-size:1.3rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand);
    border-radius:12px;
    padding:.5rem .8rem;
    width:100%;
    box-shadow:0 1px 6px rgba(0,0,0,.04);
    margin:1.25rem 0 .7rem;
  }
  .section-title::after{
    content:"";flex:1;height:3px;
    background:linear-gradient(to right,#4a90e2,#e91e63);
    border-radius:2px;margin-left:.8rem;
  }

  /* Listas limpias y legibles */
  .teach-list{margin:.3rem 0 1.1rem; padding-left:1.15rem;}
  .teach-list li{margin:.35rem 0; line-height:1.55;}
  .teach-note{color:var(--muted);}

  /* Separadores suaves entre bloques cuando quieras <hr> */
  .teach-sep{height:0;margin:.6rem 0;border:0}
</style>

<div class="teach-page">

  <h2 class="section-title">🔍 Doctoral Courses</h2>
  <ul class="teach-list">
    <li><strong>Improving Deep Learning by Exploiting Synthetic Images</strong>. Universidad de Almería (UAL), Spain. 2024. <a href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">📂 Materials</a>.</li>
    <li><strong>Research Methodology</strong>. Universidad de Castilla-La Mancha (UCLM), Spain. 2022.</li>
    <li><strong>Artificial Neural Networks and Deep Learning</strong>. Universidad de Almería (UAL), Spain. 2022. <a href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">📂 Materials</a>.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">📖 Master Courses</h2>
  <ul class="teach-list">
    <li><strong>Data Mining</strong> &amp; <strong>Deep Learning</strong>. MSc in Artificial Intelligence, Universidad Nacional de Educación a Distancia (UNED), Spain. 2023–Current.</li>
    <li><strong>Machine Learning II</strong> &amp; <strong>Deep Learning</strong>. MSc in Engineering and Data Science, UNED, Spain. 2023–Current.</li>
    <li><strong>International Seminar I – Artificial Intelligence</strong>. MSc in Strategic Content Management, Universidad de Lima (ULima), Peru. 2020–2022.</li>
    <li><strong>Machine Learning &amp; Data Mining</strong>. MSc in Computer Science, Universidad Nacional de Ingeniería (UNI), Peru. 2019–2020.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">🎤 Seminars and Technical Courses</h2>
  <ul class="teach-list">
    <li><strong>Improving Deep Learning by Exploiting Synthetic Images</strong>. MSc in Artificial Intelligence, UPM, Spain. 2024. <a href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">📂 Materials</a>.</li>
    <li><strong>Deep Learning con Python</strong>. UNAM, México. 2024. <a href="https://github.com/manwestc/UNAM-Curso-ML-y-DL" target="_blank" rel="noopener">📂 Materials</a>.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">📚 Undergraduate Courses</h2>
  <ul class="teach-list">
    <li><strong>Machine Learning</strong>. BSc in Computer Science, UNED, Spain. 2025–Current.</li>
    <li><strong>Inteligent Systems</strong>. BSc in Computer Science, UNED, Spain. 2024–Current.</li>
    <li><strong>Data Mining</strong>. BSc in Computer Science, UNED, Spain. 2023–Current.</li>
    <li><strong>Probability and Statistics I</strong>. BSc in Computer Science, UPM, Spain. 2022–2023.</li>
    <li><strong>Workshop on Research Proposal</strong>. BSc in Computer Science, ULima, Peru. 2021.</li>
    <li><strong>Network Management</strong>, <strong>Thesis Seminar</strong>, <strong>Fundamentals of Programming</strong>, <strong>Programming on Mobile Devices</strong> &amp; <strong>Algorithms</strong>. BSc in Computer Science, UNI, Peru. 2014–2020.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">🎓 M.Sc. Thesis Supervision</h2>
  <ul class="teach-list">
    <li>Joel Hancco. “Diagnóstico Concurrente de Unidades de Bombeo Mecánico a Partir de Cartas Dinamométricas Usando Técnicas de Aprendizaje Profundo”. UNI, Peru. 2026. <a href="https://" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Mario Lavado. “Generación y aumento de imágenes sintéticas a partir de datos tabulares mediante GAN: un estudio experimental con Vision Transformers”. UNI, Peru. 2026. <a href="https://" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Giovanny Mondragón Ruiz. “Interpretable Hybrid Models for Tabular Data: Integrating Kolmogorov–Arnold and Convolutional Networks via Synthetic Images”. UPM, Spain. 2025. <a href="https://oa.upm.es/90918/" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Felipe Escalera. “PermGrad: Interpretable Hybrid Neural Networks with Synthetic Images for Tabular Data”. UNED, Spain. 2025. <a href="https://hdl.handle.net/20.500.14468/31806" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Michael Vera. “BeeGOns!: Diseño y Evaluación de un Nodo Sensor Inalámbrico para Computación en la Niebla en Aplicaciones de Ciudades Inteligentes”. UCLM, Spain. 2025. <a href="https://hdl.handle.net/10578/46997" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>David González. “Transformación de Datos Tabulares a Imágenes Sintéticas: Optimización y Evaluación de la Librería TINTOlib en Python”. UPM, Spain. 2024. <a href="https://oa.upm.es/82830/" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Borja Reinoso. “TINTOlib: librería en Python de transformación de datos tabulares en imágenes para redes neuronales convolucionales de dos dimensiones”. UPM, Spain. 2023. <a href="https://oa.upm.es/75351/" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Jiayun Liu. “Sistema de recomendación de revistas para artículos académicos: Un enfoque léxico y semántico basado en redes neuronales por grafo”. UPM, Spain. 2023. <a href="https://oa.upm.es/75794/" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Eduardo Yauri. “Redes generativas antagónicas para la síntesis y generación de texto a imagen”. UNI, Peru. 2023. <a href="http://hdl.handle.net/20.500.14076/26927" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Edmundo Mori. “Optimización de las campañas de marketing en la Industria Financiera: Un enfoque basado en Machine Learning”. UNI, Peru. 2022. <a href="http://hdl.handle.net/20.500.14076/26917" target="_blank" rel="noopener">📂 Link</a>.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">🎓 B.Sc. Thesis Supervision</h2>
  <ul class="teach-list">
    <li>Javier Pérez Tárraga. “Desarrollo de una aplicación web…” UCLM, Spain. 2023. <span class="teach-note">📖</span> <a href="#" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Edgar Jesús Huaranga Junco. “Optimización del Consumo de Energía…” UNI, Peru. 2021. <a href="http://hdl.handle.net/20.500.14076/22835" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Victor Giovanny Mondragón Ruiz. “Evaluación y optimización…” UNI, Peru. 2019. <a href="http://hdl.handle.net/20.500.14076/18948" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Javier Enrique Villegas Herrera. “Desarrollo de un sistema IoT…” UNI, Peru. 2018. <a href="http://hdl.handle.net/20.500.14076/18443" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Jesús Enrique Lovón Melgarejo. “Técnicas para la localización en interiores…” UNI, Peru. 2018. <a href="http://hdl.handle.net/20.500.14076/15999" target="_blank" rel="noopener">📂 Link</a>.</li>
    <li>Eduardo Yauri Lozano. “SnorUNI: Aplicación móvil…” UNI, Peru. 2017. <a href="http://hdl.handle.net/20.500.14076/5651" target="_blank" rel="noopener">📂 Link</a>.</li>
  </ul>

  <hr class="teach-sep">

  <h2 class="section-title">📚 Courses, Workshops & Tutorials</h2>
  <ul class="teach-list">
    <li>Advanced Techniques in Deep Learning. Universidad Diego Portales, Chile. 2021–2022.</li>
    <li>Big Data, Machine Learning, Deep Learning for Business Engineering. UNJBG, Peru. 2021–2022.</li>
    <li>Deep Learning for Computer Vision. Universidad Nacional de Cajamarca, Peru. 2020–2021.</li>
    <li>Machine Learning with Python &amp; Deep Learning with Python. UPCH, Peru. 2018–2020.</li>
    <li>Data Analytics with R. UPCH, Peru. 2018–2020.</li>
    <li>Scientific Texts with LaTeX. UPCH, Peru. 2018–2019.</li>
  </ul>

</div>