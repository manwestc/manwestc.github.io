---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
description: "University teaching, thesis supervision, and technical training by Manuel Castillo-Cara at undergraduate, master’s and doctoral levels."
---

{% include base_path %}

<!-- ✅ SEO Structured Data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Manuel Castillo-Cara",
  "jobTitle": "Professor & Researcher",
  "affiliation": { "@type": "EducationalOrganization", "name": "Universidad Nacional de Educación a Distancia (UNED)" },
  "url": "{{ site.url }}{{ page.url }}",
  "hasCredential": "PhD in Computer Science",
  "description": "University teaching and thesis supervision at doctoral, master’s, and undergraduate levels, along with technical workshops in artificial intelligence, data science, and deep learning."
}
</script>

<style>
  :root{
    --ink:#1f2937; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8; --pill:#eef2ff;
  }

  .teach-wrap{max-width:1050px;margin:0 auto;padding:0 1rem;}

  /* === Section headers (igual que Publications) === */
  .section{margin:1.6rem 0}
  .section h2{
    display:flex;align-items:center;gap:.5rem;
    font-size:1.3rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand);
    border-radius:12px;padding:.5rem .8rem;margin:.25rem 0 .9rem;
  }
  .section h2::after{
    content:"";flex:1;height:3px;
    background:linear-gradient(to right,#4a90e2,#e91e63);
    border-radius:2px;margin-left:.6rem;
  }

  /* === Layouts (como Publications) === */
  .list-cards{display:grid;grid-template-columns:1fr;gap:.75rem}
  .list-grid{display:grid;grid-template-columns:1fr 1fr;gap:.75rem}
  @media (max-width:820px){ .list-grid{grid-template-columns:1fr} }

  /* === Cards === */
  .teach-card{
    background:var(--card);border:1px solid var(--bd);border-radius:12px;
    padding:.85rem 1rem; box-shadow:0 1px 8px rgba(0,0,0,.03)
  }
  .teach-title{margin:0 0 .35rem;line-height:1.35;font-weight:800}
  .teach-meta{font-size:.95rem;color:var(--muted);margin:.15rem 0 .35rem}
  .badges{display:flex;flex-wrap:wrap;gap:.35rem;margin:.2rem 0 .5rem}
  .badge{
    display:inline-block;border:1px solid var(--bd);border-radius:999px;
    padding:.12rem .55rem;font-size:.78rem;color:#334155;background:#f1f5f9;
    font-weight:700
  }
  .btn{
    display:inline-block;background:var(--brand);color:#fff;text-decoration:none;
    padding:.45rem .7rem;border-radius:8px;font-weight:700;font-size:.9rem
  }
  .btn:hover{background:var(--brand2)}
  .btn-row{display:flex;flex-wrap:wrap;gap:.5rem;margin-top:.35rem}
  /* separadores suaves (ocultos para uniformizar como pediste) */
  hr.soft{display:none}
</style>

<div class="teach-wrap">

  <!-- Doctoral -->
  <div class="section">
    <h2>🔍 Doctoral Courses</h2>
    <div class="list-grid">

      <article class="teach-card">
        <p class="teach-title">Improving Deep Learning by Exploiting Synthetic Images</p>
        <p class="teach-meta"><strong>Universidad de Almería (UAL)</strong>, Spain · 2024</p>
        <div class="badges">
          <span class="badge">Doctoral</span><span class="badge">Deep Learning</span>
        </div>
        <div class="btn-row">
          <a class="btn" href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">Materials</a>
        </div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Research Methodology</p>
        <p class="teach-meta"><strong>Universidad de Castilla-La Mancha (UCLM)</strong>, Spain · 2022</p>
        <div class="badges"><span class="badge">Doctoral</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Artificial Neural Networks and Deep Learning</p>
        <p class="teach-meta"><strong>Universidad de Almería (UAL)</strong>, Spain · 2022</p>
        <div class="badges"><span class="badge">Doctoral</span><span class="badge">DL</span></div>
        <div class="btn-row">
          <a class="btn" href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">Materials</a>
        </div>
      </article>

    </div>
  </div>

  <!-- Master -->
  <div class="section">
    <h2>📖 Master Courses</h2>
    <div class="list-grid">

      <article class="teach-card">
        <p class="teach-title">Data Mining & Deep Learning</p>
        <p class="teach-meta"><strong>MSc in AI, UNED</strong>, Spain · 2023–Current</p>
        <div class="badges"><span class="badge">Master</span><span class="badge">UNED</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Machine Learning II & Deep Learning</p>
        <p class="teach-meta"><strong>MSc in Engineering & Data Science, UNED</strong>, Spain · 2023–Current</p>
        <div class="badges"><span class="badge">Master</span><span class="badge">UNED</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">International Seminar I – Artificial Intelligence</p>
        <p class="teach-meta"><strong>MSc in Strategic Content Management, ULima</strong>, Peru · 2020–2022</p>
        <div class="badges"><span class="badge">Seminar</span><span class="badge">ULima</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Machine Learning & Data Mining</p>
        <p class="teach-meta"><strong>MSc in Computer Science, UNI</strong>, Peru · 2019–2020</p>
        <div class="badges"><span class="badge">Master</span><span class="badge">UNI</span></div>
      </article>

    </div>
  </div>

  <!-- Seminars -->
  <div class="section">
    <h2>🎤 Seminars & Technical Courses</h2>
    <div class="list-grid">

      <article class="teach-card">
        <p class="teach-title">Improving DL by Exploiting Synthetic Images</p>
        <p class="teach-meta"><strong>MSc in AI, UPM</strong>, Spain · 2024</p>
        <div class="badges"><span class="badge">Seminar</span><span class="badge">UPM</span></div>
        <div class="btn-row">
          <a class="btn" href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">Materials</a>
        </div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Deep Learning con Python</p>
        <p class="teach-meta"><strong>UNAM</strong>, México · 2024</p>
        <div class="badges"><span class="badge">Course</span><span class="badge">UNAM</span></div>
        <div class="btn-row">
          <a class="btn" href="https://github.com/manwestc/UNAM-Curso-ML-y-DL" target="_blank" rel="noopener">Materials</a>
        </div>
      </article>

    </div>
  </div>

  <!-- Undergraduate -->
  <div class="section">
    <h2>📚 Undergraduate Courses</h2>
    <div class="list-grid">

      <article class="teach-card">
        <p class="teach-title">Intelligent Systems</p>
        <p class="teach-meta"><strong>BSc in Computer Science, UNED</strong>, Spain · 2024–Current</p>
        <div class="badges"><span class="badge">Undergrad</span><span class="badge">UNED</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Data Mining</p>
        <p class="teach-meta"><strong>BSc in Computer Science, UNED</strong>, Spain · 2023–Current</p>
        <div class="badges"><span class="badge">Undergrad</span><span class="badge">UNED</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Probability & Statistics I</p>
        <p class="teach-meta"><strong>BSc in Computer Science, UPM</strong>, Spain · 2022–2023</p>
        <div class="badges"><span class="badge">Undergrad</span><span class="badge">UPM</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Other courses (UNI)</p>
        <p class="teach-meta"><strong>UNI</strong>, Peru · 2014–2020 — Network Management, Thesis Seminar, Fundamentals of Programming, Mobile Devices, Algorithms</p>
        <div class="badges"><span class="badge">Undergrad</span><span class="badge">UNI</span></div>
      </article>

    </div>
  </div>

  <!-- MSc Thesis -->
  <div class="section">
    <h2>🎓 M.Sc. Thesis Supervision</h2>
    <div class="list-cards">

      <article class="teach-card">
        <p class="teach-title">Interpretable Hybrid Models for Tabular Data (KAN + CNN via Synthetic Images)</p>
        <p class="teach-meta"><strong>Victor G. Mondragón Ruiz</strong> · UPM, Spain · 2025</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UPM</span></div>
        <div class="btn-row"><a class="btn" href="https://oa.upm.es" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Transformación de Datos Tabulares a Imágenes Sintéticas: Optimización y Evaluación de TINTOlib</p>
        <p class="teach-meta"><strong>David González</strong> · UPM, Spain · 2024</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UPM</span></div>
        <div class="btn-row"><a class="btn" href="https://oa.upm.es/82830/" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">TINTOlib: Librería en Python para Imágenes de Datos Tabulares</p>
        <p class="teach-meta"><strong>Borja Reinoso</strong> · UPM, Spain · 2023</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UPM</span></div>
        <div class="btn-row"><a class="btn" href="https://oa.upm.es/75351/" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Recommender System for Journals (GNN + Semantic Methods)</p>
        <p class="teach-meta"><strong>Jiayun Liu</strong> · UPM, Spain · 2023</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UPM</span></div>
        <div class="btn-row"><a class="btn" href="https://oa.upm.es/75794/" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">GANs para Text-to-Image en Español</p>
        <p class="teach-meta"><strong>Eduardo Yauri</strong> · UNI, Peru · 2023</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/26927" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Optimización de Campañas de Marketing con ML</p>
        <p class="teach-meta"><strong>Edmundo de Elvira Mori Orrillo</strong> · UNI, Peru · 2022</p>
        <div class="badges"><span class="badge">M.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/26917" target="_blank" rel="noopener">Link</a></div>
      </article>

    </div>
  </div>

  <!-- BSc Thesis -->
  <div class="section">
    <h2>🎓 B.Sc. Thesis Supervision</h2>
    <div class="list-cards">

      <article class="teach-card">
        <p class="teach-title">App web para tratar datos de sensores</p>
        <p class="teach-meta"><strong>Javier Pérez Tárraga</strong> · UCLM, Spain · 2023</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UCLM</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Optimización Energética en Edge/Fog Computing</p>
        <p class="teach-meta"><strong>Edgar Jesús Huaranga Junco</strong> · UNI, Peru · 2021</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/22835" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Evaluación de arquitecturas fog para IoT</p>
        <p class="teach-meta"><strong>Victor G. Mondragón Ruiz</strong> · UNI, Peru · 2019</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/18948" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Rutas inteligentes para personas ciegas (BLE)</p>
        <p class="teach-meta"><strong>Javier E. Villegas Herrera</strong> · UNI, Peru · 2018</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/18443" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Localización en interiores con Bluetooth + IA</p>
        <p class="teach-meta"><strong>Jesús E. Lovón Melgarejo</strong> · UNI, Peru · 2018</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/15999" target="_blank" rel="noopener">Link</a></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">SnorUNI: IDS móvil basado en Snort</p>
        <p class="teach-meta"><strong>Eduardo Yauri Lozano</strong> · UNI, Peru · 2017</p>
        <div class="badges"><span class="badge">B.Sc.</span><span class="badge">UNI</span></div>
        <div class="btn-row"><a class="btn" href="http://hdl.handle.net/20.500.14076/5651" target="_blank" rel="noopener">Link</a></div>
      </article>

    </div>
  </div>

  <!-- Other training -->
  <div class="section">
    <h2>📚 Courses, Workshops & Tutorials</h2>
    <div class="list-grid">

      <article class="teach-card">
        <p class="teach-title">Advanced Techniques in Deep Learning</p>
        <p class="teach-meta"><strong>Universidad Diego Portales</strong>, Chile · 2021–2022</p>
        <div class="badges"><span class="badge">Workshop</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Big Data, ML, DL for Business Engineering</p>
        <p class="teach-meta"><strong>UNJBG</strong>, Peru · 2021–2022</p>
        <div class="badges"><span class="badge">Workshop</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Deep Learning for Computer Vision</p>
        <p class="teach-meta"><strong>UNC</strong>, Peru · 2020–2021</p>
        <div class="badges"><span class="badge">Workshop</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">ML with Python & DL with Python</p>
        <p class="teach-meta"><strong>UPCH</strong>, Peru · 2018–2020</p>
        <div class="badges"><span class="badge">Course</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Data Analytics with R</p>
        <p class="teach-meta"><strong>UPCH</strong>, Peru · 2018–2020</p>
        <div class="badges"><span class="badge">Course</span></div>
      </article>

      <article class="teach-card">
        <p class="teach-title">Scientific Texts with LaTeX</p>
        <p class="teach-meta"><strong>UPCH</strong>, Peru · 2018–2019</p>
        <div class="badges"><span class="badge">Course</span></div>
      </article>

    </div>
  </div>

</div>