---
permalink: /
title: "About Me"
excerpt: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<!-- ✅ Structured Data for About Page -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Manuel Castillo-Cara",
  "image": "https://www.manuelcastillo.eu/images/profile.jpg",
  "url": "https://www.manuelcastillo.eu",
  "sameAs": [
    "https://scholar.google.es/citations?user=r0JytwIAAAAJ",
    "https://www.scopus.com/authid/detail.uri?authorId=57200871251",
    "https://www.webofscience.com/wos/author/record/O-9762-2017",
    "https://www.uned.es/universidad/docentes/informatica/jose-manuel-castillo-cara.html",
    "https://portalcientifico.uned.es/investigadores/818430/detalle",
    "https://www.udemy.com/user/manuel-castillo-cara/",
    "https://www.linkedin.com/in/manuelcastillocara/",
    "https://orcid.org/0000-0002-2990-7090"
  ],
  "jobTitle": "Professor and Researcher in Artificial Intelligence",
  "worksFor": {
    "@type": "Organization",
    "name": "Universidad Nacional de Educación a Distancia (UNED)",
    "url": "https://www.uned.es"
  },
  "memberOf": {
    "@type": "Organization",
    "name": "CISIAD – Intelligent Decision-Support Systems",
    "url": "https://portalcientifico.uned.es/grupos/17475/detalle"
  },
  "alumniOf": {
    "@type": "EducationalOrganization",
    "name": "Universidad de Castilla-La Mancha (UCLM)"
  },
  "knowsAbout": [
    "Artificial Intelligence","Machine Learning","Deep Learning","Computer Vision",
    "Natural Language Processing","Data Science","Data Analytics","Tabular Data",
    "Synthetic Data","Synthetic Images","TINTO","TINTOlib","Hybrid Neural Networks",
    "Python","R","Scikit-learn","Keras","TensorFlow","PyTorch","GeoGebra","LaTeX",
    "Educational Technology","Online Teaching","Scientific Writing","Open Science",
    "Higher Education","Research Methodology"
  ]
}
</script>

<!-- ===== Styles (ligeros y reutilizables) ===== -->
<style>
  :root{
    --ink:#37474f; --accent:#1565c0; --soft:#f5f8fa; --bd:#d0d7de;
  }
  .about-wrap{max-width:980px;margin:0 auto;padding:0 1rem;}
  .hero{
    display:flex;align-items:center;gap:1.2rem;background:linear-gradient(135deg,#0e4a7f,#1565c0);
    color:#fff;border-radius:14px;padding:1.1rem 1.3rem;margin:1.2rem 0 1.4rem;box-shadow:0 8px 24px rgba(0,0,0,.08)
  }
  .hero img{width:84px;height:84px;border-radius:50%;object-fit:cover;border:3px solid rgba(255,255,255,.6)}
  .hero h1{font-size:1.8rem;line-height:1.2;margin:.1rem 0 .3rem}
  .card{border:1px solid var(--bd);border-radius:10px;background:#fff;padding:1rem;box-shadow:0 2px 8px rgba(0,0,0,.04);margin:1rem 0}
  .card.soft{background:var(--soft)}
  .section-title{font-weight:800;color:#223;margin:1.1rem 0 .6rem}
  .cta-row{display:flex;gap:1.2rem;flex-wrap:wrap;justify-content:center}
  .btn{display:inline-block;padding:.6em 1em;border-radius:8px;text-decoration:none!important;font-weight:700}
  .btn-primary{background:#1976d2;color:#fff}
  .grid-2{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
  @media (max-width:720px){.hero{flex-direction:column;text-align:center}.grid-2{grid-template-columns:1fr}}
  table.about{width:100%;border-collapse:collapse}
  table.about th,table.about td{border:1px solid #e6e8eb;padding:.55rem .7rem;vertical-align:top}
  table.about th{background:#f3f6fb;text-align:left}
</style>

<div class="about-wrap">

  <!-- HERO -->
  <section class="hero">
    <img src="https://www.manuelcastillo.eu/images/profile.jpg" alt="Manuel Castillo-Cara">
    <div>
      <h1>Manuel Castillo-Cara, Ph.D.</h1>
      <p style="margin:0;opacity:.95">Professor & Researcher in Artificial Intelligence (UNED). Lead developer of <strong>TINTOlib</strong> and creator of the <strong>TINTO</strong> method.</p>
      <div style="margin-top:.6rem;display:flex;gap:.6rem;flex-wrap:wrap">
        <a class="btn btn-primary" href="https://www.manuelcastillo.eu/udemy/" target="_blank" rel="noopener">Udemy Courses</a>
        <a class="btn" style="border:1px solid #fff;color:#fff" href="/TINTOlib.html">TINTOlib Page</a>
      </div>
    </div>
  </section>

  <!-- Udemy + GitHub mini cards -->
  <section class="card soft">
    <h2 class="section-title" style="color:#1565c0">🎉 Learn TINTOlib for Free</h2>
    <div class="cta-row">
      <div class="card" style="flex:1 1 280px;max-width:420px;text-align:center">
        <h3 style="margin-top:0">📚 Udemy</h3>
        <p style="margin:.25rem 0 .75rem">Free course with videos and practical examples.</p>
        <a class="btn btn-primary" href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" target="_blank" rel="noopener">Access Udemy</a>
      </div>
      <div class="card" style="flex:1 1 280px;max-width:420px;text-align:center">
        <h3 style="margin-top:0">📺 GitHub</h3>
        <p style="margin:.25rem 0 .75rem">Bilingual video tutorials + notebooks.</p>
        <a href="https://github.com/oeg-upm/TINTOlib-Crash_Course" target="_blank" rel="noopener">
          <img src="https://img.shields.io/badge/GitHub-VideoTutorial%20Course-black?style=for-the-badge&logo=GitHub&logoColor=white" alt="Access GitHub Course" loading="lazy">
        </a>
      </div>
    </div>
  </section>

  <!-- Udemy intro (conserva tu texto) -->
  <section class="card">
    <h2 class="section-title">📚 My Courses on <a href="/udemy/" target="_blank">Udemy</a></h2>
    <p>I am passionate about <strong>Artificial Intelligence and Data Science</strong>, with a practical focus on training new generations. I have developed multiple Spanish-language courses on <strong>Udemy</strong>, available in the <a href="/udemy/" target="_blank"><strong>Udemy</strong></a> section with discount coupons.</p>
  </section>

  <!-- Biography -->
  <section>
    <h2 class="section-title">👨‍🎓 Biography</h2>
    <p>I am Manuel Castillo-Cara, PhD in Computer Science, specialized in <strong>Artificial Intelligence</strong>, from Universidad de Castilla-La Mancha (UCLM), where I received the Cum Laude distinction in 2018.</p>
    <div class="card soft">
      <div class="grid-2" style="align-items:start">
        <div>
          <table class="about">
            <thead>
              <tr><th>Period</th><th>Position</th><th>Institution</th><th>Research Group</th></tr>
            </thead>
            <tbody>
              <tr>
                <td><strong>2014 – 2020</strong></td>
                <td>Professor/Researcher in Peru</td>
                <td>Universidad Nacional de Ingeniería (UNI) <br> Universidad de Lima (ULima)</td>
                <td>IUT-SCi</td>
              </tr>
              <tr>
                <td><strong>2021 – 2023</strong></td>
                <td>Postdoctoral Contract (María Zambrano)</td>
                <td>Universidad Politécnica de Madrid (UPM)</td>
                <td><a href="https://oeg.fi.upm.es/" target="_blank">OEG</a></td>
              </tr>
              <tr>
                <td><strong>Since 2023</strong></td>
                <td>Professor/Researcher</td>
                <td><a href="https://www.uned.es/universidad/docentes/informatica/jose-manuel-castillo-cara.html" target="_blank">UNED</a></td>
                <td><a href="https://portalcientifico.uned.es/grupos/17475/detalle" target="_blank">CISIAD</a></td>
              </tr>
            </tbody>
          </table>
        </div>
        <div>
          <h3 style="margin:.2rem 0 .6rem">🎓 Research Interests & Projects</h3>
          <p>Throughout my career, I have participated in <strong>15+ research projects</strong>, leading two as PI. I also contributed to a social development project in Peru, bringing educational robotics and Scratch to more than <strong>2,000 children</strong> in vulnerable areas.</p>
          <ul style="margin:.6rem 0 0 1rem">
            <li>Main area: <strong>Synthetic Images & Hybrid Neural Networks</strong>.</li>
            <li>Lead developer of <a href="/libros-software/software-TINTOlib/" target="_blank"><strong>TINTOlib</strong></a>.</li>
            <li>Creator of the <a href="/libros-software/software-TINTO/" target="_blank"><strong>TINTO</strong></a> method.</li>
            <li>Talks and seminars in Spain and the Americas — see the <a href="/TINTOlib.html" target="_blank">TINTOlib page</a>.</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Scientific Production -->
  <section class="card">
    <h2 class="section-title">🔬 Scientific Production</h2>
    <ul>
      <li>25 journal articles (peer-reviewed)</li>
      <li>7 conference presentations (4 indexed in Scopus) and 1 tutorial</li>
      <li>2 IEEE international robotics competitions (3rd place)</li>
      <li>1 utility model patent</li>
      <li>2 software copyright registrations</li>
      <li>1 academic book and 1 book chapter</li>
      <li>6 Master’s theses and 6 Bachelor’s theses supervised</li>
    </ul>

    <h3 class="section-title" style="margin-top:1rem">📊 Impact in the Scientific Community</h3>
    <table class="about">
      <thead><tr><th>Source</th><th>Citations</th><th>#Q1</th><th>#Q2</th><th>H-Index</th></tr></thead>
      <tbody>
        <tr>
          <td><a href="https://www.webofscience.com/wos/author/record/O-9762-2017" target="_blank">Web Of Science (JCR)</a></td>
          <td>210</td><td>9</td><td>10</td><td>9</td>
        </tr>
        <tr>
          <td><a href="https://www.scopus.com/authid/detail.uri?authorId=57200871251" target="_blank">Scopus (SJR)</a></td>
          <td>344</td><td>15</td><td>8</td><td>11</td>
        </tr>
        <tr>
          <td><a href="https://scholar.google.es/citations?hl=es&authuser=2&user=r0JytwIAAAAJ" target="_blank">Google Scholar</a></td>
          <td>548</td><td>–</td><td>–</td><td>13</td>
        </tr>
      </tbody>
    </table>
  </section>

</div>