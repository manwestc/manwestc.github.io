---
layout: archive
title: "📄 Publications"
permalink: /publications/
author_profile: true
description: "Scientific publications, books, patents and software contributions by Manuel Castillo-Cara"
---

{% include base_path %}

<!-- ✅ SEO Structured Data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Manuel Castillo-Cara",
  "url": "https://www.manuelcastillo.eu/",
  "affiliation": { "@type": "Organization", "name": "Universidad Nacional de Educación a Distancia (UNED)" },
  "sameAs": [
    "https://scholar.google.es/citations?user=r0JytwIAAAAJ",
    "https://www.scopus.com/authid/detail.uri?authorId=57200871251",
    "https://www.webofscience.com/wos/author/record/O-9762-2017"
  ]
}
</script>

<style>
  :root{
    --ink:#0f172a; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8; --pill:#eef2ff;
  }
  .pub-wrap{max-width:1050px;margin:0 auto;padding:0 1rem;}

  /* Section headings */
  .section{margin:1.6rem 0}
  .section h2{
    font-weight:900; font-size:1.35rem; margin:.25rem 0 .75rem;
    color:#0f172a; letter-spacing:.2px
  }
  .section small{color:var(--muted)}

  /* Layouts */
  .list-cards{display:grid;grid-template-columns:1fr;gap:.8rem}      /* 1 column */
  .list-grid{display:grid;grid-template-columns:1fr 1fr;gap:.8rem}   /* 2 columns */
  @media (max-width:820px){ .list-grid{grid-template-columns:1fr} }

  /* Cards */
  .pub-card{
    background:var(--card);border:1px solid var(--bd);border-radius:12px;
    padding:1rem 1.05rem; box-shadow:0 1px 8px rgba(0,0,0,.03)
  }

  /* Title & inline badges (improved hierarchy) */
  .pub-title{
    margin:0; line-height:1.45;
    font-weight:800; font-size:1.06rem; color:var(--ink);
  }
  .pub-title em{
    font-style:italic; font-weight:700; color:#1e293b;
  }
  /* Badges inline justo tras el texto del paper */
  .pub-title .badge{
    display:inline-block; margin-left:.45rem; margin-top:.35rem;
    border:1px solid var(--bd); border-radius:999px;
    padding:.14rem .55rem; font-size:.78rem; color:#334155; background:#f1f5f9;
    font-weight:800;
  }

  /* DOI button */
  .btn-row{display:flex;justify-content:center;gap:.5rem;margin-top:.55rem}
  .btn-doi{
    display:inline-block;background:var(--brand);color:#fff;text-decoration:none;
    padding:.48rem .8rem;border-radius:8px;font-weight:800;font-size:.92rem
  }
  .btn-doi:hover{background:var(--brand2)}

  hr.soft{border:none;height:1px;background:var(--bd);margin:1.25rem 0}

  /* === Scientific databases cards === */
  .db-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(220px,1fr));
    gap:0.9rem;
    margin-top:0.6rem;
  }
  .db-card{
    display:flex; align-items:center; gap:.75rem;
    background: linear-gradient(180deg, #ffffff, #f7f9ff);
    border: 1px solid #e5e7eb; border-radius: 12px;
    padding:.85rem 1rem;
    box-shadow: 0 2px 10px rgba(0,0,0,.03);
    text-decoration:none; color:inherit;
    transition: transform .12s ease, box-shadow .12s ease, border-color .12s ease;
  }
  .db-card:hover{
    transform: translateY(-2px);
    box-shadow: 0 6px 18px rgba(0,0,0,.06);
    border-color:#d6d9e0;
  }
  .db-icon{
    width:38px; height:38px; border-radius:10px;
    display:inline-flex; align-items:center; justify-content:center;
    background:#eef2ff; color:#1f3a8a; flex:0 0 38px;
    box-shadow: inset 0 0 0 1px #dbe3ff;
  }
  .db-body{display:flex; flex-direction:column; gap:.15rem; min-width:0}
  .db-title{font-weight:900; color:#111827; line-height:1.2; white-space:nowrap; overflow:hidden; text-overflow:ellipsis}
  .db-sub{font-size:.9rem; color:#6b7280}
</style>

<div class="pub-wrap">

  <!-- Scientific databases -->
  <div class="section">
    <h2>🔎 Scientific Databases</h2>
    <div class="db-grid">

      <a class="db-card" href="https://scholar.google.es/citations?hl=es&authuser=2&user=r0JytwIAAAAJ" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- book icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M3 5a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v14a1 1 0 0 1-1.447.894L14 18.118l-3.553 1.776A1 1 0 0 1 9 19V5H5a2 2 0 0 0-2 2V5z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">Google Scholar</span>
          <span class="db-sub">Citations, h-index, co-authors</span>
        </span>
      </a>

      <a class="db-card" href="https://www.scopus.com/authid/detail.uri?authorId=57200871251" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- chart icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M3 3h2v18H3V3zm4 8h2v10H7V11zm4-5h2v15h-2V6zm4 8h2v7h-2v-7zm4-11h2v18h-2V3z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">Scopus</span>
          <span class="db-sub">SJR, citations and impact</span>
        </span>
      </a>

      <a class="db-card" href="https://www.webofscience.com/wos/author/record/O-9762-2017" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- globe icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2a10 10 0 100 20 10 10 0 000-20Zm7.93 9H16.9a15.3 15.3 0 00-.9-4.02A8.03 8.03 0 0119.93 11ZM8 11H4.07A8.03 8.03 0 017.1 6.98 15.3 15.3 0 008 11Zm0 2a13.4 13.4 0 01-.9 4.02A8.03 8.03 0 014.07 13H8Zm2 0h4a13.4 13.4 0 01-.9 4.02A13.4 13.4 0 0110 15Zm6 0h3.93A8.03 8.03 0 0116.9 17.02 15.3 15.3 0 0016 15Zm-2-2h-4a13.4 13.4 0 01.9-4.02A13.4 13.4 0 0114 13ZM12 4.07c.9.9 1.78 2.53 2.3 4.93h-4.6c.52-2.4 1.4-4.03 2.3-4.93ZM12 19.93c-.9-.9-1.78-2.53-2.3-4.93h4.6c-.52 2.4-1.4 4.03-2.3 4.93Z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">Web of Science</span>
          <span class="db-sub">JCR metrics and records</span>
        </span>
      </a>

      <a class="db-card" href="https://portalcientifico.uned.es/investigadores/818430/detalle" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- id card icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M3 5a2 2 0 012-2h14a2 2 0 012 2v12a2 2 0 01-2 2H5a2 2 0 01-2-2V5zm4 3h6v2H7V8zm0 4h10v2H7v-2z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">UNED Researcher</span>
          <span class="db-sub">Profile at UNED Portal</span>
        </span>
      </a>

      <a class="db-card" href="https://www.uned.es/universidad/docentes/informatica/jose-manuel-castillo-cara.html" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- university icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12 3L2 8l10 5 10-5-10-5zm-7 8v5l7 3 7-3v-5l-7 3-7-3z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">UNED Professor</span>
          <span class="db-sub">Teaching profile</span>
        </span>
      </a>

      <a class="db-card" href="https://portalcientifico.uned.es/grupos/17475/detalle" target="_blank" rel="noopener">
        <span class="db-icon" aria-hidden="true">
          <!-- users icon -->
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M12 12a5 5 0 100-10 5 5 0 000 10zm-7 9a7 7 0 0114 0H5zm15.5-7a3.5 3.5 0 10-3.001-5.4 6 6 0 011.35 3.9c0 1.06-.27 2.06-.75 2.95.71.36 1.5.55 2.401.55z"/></svg>
        </span>
        <span class="db-body">
          <span class="db-title">CISIAD Research Group</span>
          <span class="db-sub">Intelligent Decision Support Systems</span>
        </span>
      </a>

    </div>
  </div>

  <hr class="soft">

  <!-- Articles (1 column, badges inline justo tras el texto) -->
  <div class="section">
    <h2>🧠 Most Recent 10 Publications in AI</h2>
    <div class="list-cards">

      <article class="pub-card">
        <p class="pub-title">
          Manuel Castillo-Cara, et al. <em>MIMO-Based Indoor Localisation with Hybrid Neural Networks: Leveraging Synthetic Images from Tidy Data for Enhanced Deep Learning</em>. IEEE Journal of Selected Topics in Signal Processing.
          <span class="badge">IF: 13.7 (Q1)</span><span class="badge">SJR 4.12 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1109/JSTSP.2025.3555067" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Jiayun Liu, Manuel Castillo-Cara, et al. <em>On the Significance of Graph Neural Networks with Pretrained Transformers in Content-Based Recommender Systems for Academic Articles Classification</em>. Expert Systems.
          <span class="badge">IF: 2.3 (Q2)</span><span class="badge">SJR 0.74 (Q2)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1111/exsy.70073" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Eduardo Yauri-Lozano, Manuel Castillo-Cara, et al. <em>Generative Adversarial Networks for Text-to-Face Synthesis & Generation: A Quantitative-Qualitative Analysis of NLP Encoders for Spanish</em>. Information Processing & Management, 2024.
          <span class="badge">IF: 6.9 (Q1)</span><span class="badge">SJR 2.06 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.ipm.2024.103667" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Edgar Huaranga-Junco, Salvador González-Gerpe, Manuel Castillo-Cara, et al. <em>From cloud and fog computing to federated-fog computing: A comparative analysis…</em> Future Generation Computer Systems, 2024.
          <span class="badge">IF: 6.1 (Q1)</span><span class="badge">SJR 1.55 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.future.2024.05.001" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Michael Vera, Kewin Cuadros, Manuel Castillo-Cara, et al. <em>BeeGOns!: A Wireless Sensor Node for Fog-Computing based Smart City Platforms</em>. IEEE TCAD, 2024.
          <span class="badge">IF: 2.9 (Q2)</span><span class="badge">SJR 0.73 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1109/TCAD.2023.3305575" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Reewos Talla-Chumpitaz, Manuel Castillo-Cara, et al. <em>A Novel Deep Learning Approach using Blurring Image Techniques for Bluetooth-based Indoor Localisation</em>. Information Fusion, 2023.
          <span class="badge">IF: 14.7 (Q1)</span><span class="badge">SJR 5.65 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.inffus.2022.10.011" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Manuel Castillo-Cara, et al. <em>TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks</em>. SoftwareX, 2023.
          <span class="badge">IF: 2.4 (Q2)</span><span class="badge">SJR 0.54 (Q2)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.softx.2023.101391" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Alonso Tenorio-Trigoso, Manuel Castillo-Cara, et al. <em>An Analysis of Computational Resources of Event-Driven Streaming Data Flow for Internet of Things</em>. The Computer Journal, 2023.
          <span class="badge">IF: 1.5 (Q3)</span><span class="badge">SJR 0.48 (Q2)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1093/comjnl/bxab143" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Luis Vasquez-Espinoza, Manuel Castillo-Cara, Luis Orozco-Barbosa. <em>On the Relevance of the Metadata used in the Semantic Segmentation of Indoor Image Spaces</em>. Expert Systems with Applications, 2021.
          <span class="badge">IF: 8.67 (Q1)</span><span class="badge">SJR 2.07 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.eswa.2021.115486" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">
          Giovanny Mondragón-Ruiz, Alonso Tenorio-Trigoso, Manuel Castillo-Cara, et al. <em>An Experimental Study of Fog and Cloud Computing in CEP-based Real-Time IoT Applications</em>. Journal of Cloud Computing, 2021.
          <span class="badge">IF: 3.42 (Q2)</span><span class="badge">SJR 1.05 (Q1)</span>
        </p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1186/s13677-021-00245-7" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

    </div>
  </div>

  <hr class="soft">

  <!-- Books & Chapters (GeoGebra first full row; others two columns) -->
  <div class="section">
    <h2>📚 Books & Chapters</h2>
    <div class="list-grid">
      <!-- GeoGebra: full-width row -->
      <article class="pub-card" style="grid-column:1 / -1">
        <p class="pub-title">Book — Manuel Castillo-Cara. <em>GeoGebra en el Aula. Aplicaciones Matemáticas aplicadas al aula con GeoGebra</em>. ISBN: 9798379088873, Amazon.</p>
        <div class="btn-row"><a class="btn-doi" href="https://www.manuelcastillo.eu/libros-software/libro-curso-GeoGebra-Aula/" target="_blank" rel="noopener">View Book</a></div>
      </article>
      <!-- Two columns below -->
      <article class="pub-card">
        <p class="pub-title">Chapter — Hancco <em>et al.</em> <em>Cost-Effective Advanced Remote Diagnostics of Sucker Rod Pumping Wells From Dynamometric Charts: A Deep Learning Approach</em>. IGI Global, 2024.</p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.4018/979-8-3693-0740-3.ch009" target="_blank" rel="noopener">Open DOI</a></div>
      </article>
      <article class="pub-card">
        <p class="pub-title">Whitepaper — Manuel Castillo-Cara. <em>Combating Multipath Fading in Indoor Positioning with Asynchronous Power Transmission Techniques</em>. COST Action INTERACT WG2, 2024.</p>
        <div class="btn-row"><a class="btn-doi" href="https://interactca20120.org/work-in-progress/" target="_blank" rel="noopener">Document</a></div>
      </article>
    </div>
  </div>

  <hr class="soft">

  <!-- Software & Patents (merged) -->
  <div class="section">
    <h2>💻 Software & Patents</h2>
    <div class="list-grid">
      <article class="pub-card">
        <p class="pub-title">TINTORERA — Manuel Castillo-Cara & Raúl García-Castro. Registro PI: 16/2023/4624.</p>
        <div class="btn-row"><a class="btn-doi" href="https://www.manuelcastillo.eu/libros-software/software-TINTOlib/" target="_blank" rel="noopener">Project Page</a></div>
      </article>
      <article class="pub-card">
        <p class="pub-title">TINTORETTO — Manuel Castillo-Cara & Raúl García-Castro. Registro PI: 16/2023/5491.</p>
        <div class="btn-row"><a class="btn-doi" href="https://www.manuelcastillo.eu/libros-software/software-TINTO/" target="_blank" rel="noopener">Project Page</a></div>
      </article>
      <article class="pub-card">
        <p class="pub-title">Patent — Dispositivo electrónico para seguimiento y localización de personas o animales. Expediente: 002758-2016/DIN. Resolución: 000417-2019/DIN-INDECOPI. Título N.º: 1151, Perú, 2019.</p>
        <div class="btn-row"><a class="btn-doi" href="https://www.manuelcastillo.eu/libros-software/patente/" target="_blank" rel="noopener">Patent Page</a></div>
      </article>
    </div>
  </div>

  <hr class="soft">

  <!-- Conferences (includes the tutorial) -->
  <div class="section">
    <h2>🌍 Conferences</h2>
    <div class="list-grid">
      <article class="pub-card">
        <p class="pub-title">Improving Deep Learning by Exploiting Synthetic Images. 27th European Conference on Artificial Intelligence (ECAI), 2024. Tutorial.</p>
        <div class="btn-row">
          <a class="btn-doi" href="https://www.ecai2024.eu/programme/tutorials" target="_blank" rel="noopener">Event</a>
          <a class="btn-doi" style="background:#475569" href="https://github.com/DCY1117/ECAI2024-Material" target="_blank" rel="noopener">Materials</a>
        </div>
      </article>

      <article class="pub-card">
        <p class="pub-title">Hybrid Neural Network-Based Indoor Localisation System for Mobile Robots Using CSI Data in a Robotics Simulator. 5th International Conference on Robotics, Computer Vision and Intelligent Systems (ROBOVIS), Portugal, 2025.</p>
        <div class="btn-row"><a class="btn-doi" href="https://www.insticc.org/node/TechnicalProgram/robovis/2025/personDetails/1d6991cc-c792-4bba-990d-91aed2148de6" target="_blank" rel="noopener">Event</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">Phenotypes of non-alcoholic fatty liver disease (NAFLD) and all-cause mortality. 2022 Annual Meeting of the American College of Epidemiology, USA, 2022.</p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1016/j.annepidem.2022.08.036" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">Identification of risk zones for road safety through unsupervised learning algorithms. 16th LACCEI, Peru, 2018.</p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.18687/laccei2018.1.1.413" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">Supervised learning algorithms for indoor localization fingerprinting using BLE4.0 Beacons. 4th IEEE LA-CCI, Peru, 2017.</p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.1109/LA-CCI.2017.8285716" target="_blank" rel="noopener">Open DOI</a></div>
      </article>

      <article class="pub-card">
        <p class="pub-title">Citizen security using Machine Learning algorithms through Open Data. 8th IEEE LATINCOM, Colombia, 2016.</p>
        <div class="btn-row"><a class="btn-doi" href="https://doi.org/10.