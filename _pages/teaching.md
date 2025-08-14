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
  "affiliation": {
    "@type": "EducationalOrganization",
    "name": "Universidad Nacional de Educación a Distancia (UNED)"
  },
  "url": "{{ site.url }}{{ page.url }}",
  "hasCredential": "PhD in Computer Science",
  "description": "University teaching and thesis supervision at doctoral, master’s, and undergraduate levels, along with technical workshops in artificial intelligence, data science, and deep learning."
}
</script>

<style>
  /* === Teaching: estilos unificados (scope por clase .teach-page) === */
  .teach-page{max-width:980px;margin:0 auto;padding:0 1rem}

  :root{
    --ink: #37474f;
    --brand: #1565c0;
    --card-bd:#d0d7de;
    --surface:#ffffff;
    --surface-soft:#f5f8fa;
  }

  /* Título de sección con barra (igual que About/Publications/TINTOlib) */
  .teach-page .section-title{
    display:flex;align-items:center;gap:.5rem;
    font-size:1.3rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand);
    border-radius:12px;
    padding:.5rem .8rem;
    width:100%;
    box-shadow:0 1px 6px rgba(0,0,0,.04);
    margin:1.2rem 0 .6rem;
  }
  .teach-page .section-title::after{
    content:"";flex:1;height:3px;
    background:linear-gradient(to right,#4a90e2,#e91e63);
    border-radius:2px;margin-left:.8rem;
  }

  /* Listas un poco más aireadas y legibles */
  .teach-page ul{margin:.4rem 0 1rem}
  .teach-page li{margin:.25rem 0;line-height:1.5}

  /* Separadores markdown '---' ya no necesitan línea */
  .teach-page hr{border:0;height:0;margin:.8rem 0}
</style>

<div class="teach-page">

## 🔍 **Doctoral Courses** {: .section-title}
- **Improving Deep Learning by Exploiting Synthetic Images**. Universidad de Almería (UAL), Spain. 2024. [📂 Materials](https://github.com/oeg-upm/TINTOlib-Crash_Course){:target="_blank"}.
- **Research Methodology**. Universidad de Castilla-La Mancha (UCLM), Spain. 2022.  
- **Artificial Neural Networks and Deep Learning**. Universidad de Almería (UAL), Spain. 2022. [📂 Materials](https://github.com/oeg-upm/TINTOlib-Crash_Course){:target="_blank"}.

---

## 📖 **Master Courses** {: .section-title}
- **Data Mining** & **Deep Learning**. MSc in Artificial Intelligence, Universidad Nacional de Educación a Distancia (UNED), Spain. 2023-Current.
- **Machine Learning II** & **Deep Learning**. MSc in Engineering and Data Science, UNED, Spain. 2023-Current. 
- **International Seminar I - Artificial Intelligence**. MSc in Strategic Content Management, Universidad de Lima (ULima), Peru. 2020-2022.  
- **Machine Learning & Data Mining**.  MSc in Computer Science, Universidad Nacional de Ingeniería (UNI), Peru. 2019-2020.  

---

## 🎤 **Seminars and Technical Courses** {: .section-title}
- **Improving Deep Learning by Exploiting Synthetic Images**. MSc in Artificial Intelligence, UPM, Spain. 2024. [📂 Materials](https://github.com/oeg-upm/TINTOlib-Crash_Course){:target="_blank"}.
- **Deep Learning con Python**. UNAM, México. 2024. [📂 Materials](https://github.com/manwestc/UNAM-Curso-ML-y-DL){:target="_blank"}.  

---

## 📚 **Undergraduate Courses** {: .section-title}
- **Inteligent Systems**. BSc in Computer Science, UNED, Spain. 2024-Current.
- **Data Mining**. BSc in Computer Science, UNED, Spain. 2023-Current.
- **Probability and Statistics I**. BSc in Computer Science, UPM, Spain. 2022-2023.
- **Workshop on Research Proposal**. BSc in Computer Science, ULima, Peru. 2021.
- **Network Management**, **Thesis Seminar**, **Fundamentals of Programming**, **Programming on Mobile Devices** & **Algorithms**. BSc in Computer Science, UNI, Peru. 2014-2020.

---

## 🎓 **M.Sc. Thesis Supervision** {: .section-title}
- Victor Giovanny Mondragón Ruiz. "Interpretable Hybrid Models for Tabular Data: Integrating Kolmogorov–Arnold and Convolutional Networks via Synthetic Images". UPM, Spain. 2025. [📂 Link](https://oa.upm.es){:target="_blank"}.  
- David González. "Transformación de Datos Tabulares a Imágenes Sintéticas…". UPM, Spain. 2024. [📂 Link](https://oa.upm.es/82830/){:target="_blank"}.  
- Borja Reinoso. "TINTOlib: Librería en Python…" UPM, Spain. 2023. [📂 Link](https://oa.upm.es/75351/){:target="_blank"}.  
- Jiayun Liu. "Sistema de recomendación de revistas…" UPM, Spain. 2023. [📂 Link](https://oa.upm.es/75794/){:target="_blank"}.  
- Eduardo Yauri. "Redes generativas antagónicas…" UNI, Peru. 2023. [📂 Link](http://hdl.handle.net/20.500.14076/26927){:target="_blank"}.  
- Edmundo de Elvira Mori Orrillo. "Optimización de las campañas de marketing…" UNI, Peru. 2022. [📂 Link](http://hdl.handle.net/20.500.14076/26917){:target="_blank"}.  

---

## 🎓 **B.Sc. Thesis Supervision** {: .section-title}
- Javier Pérez Tárraga. "Desarrollo de una aplicación web…" UCLM, Spain. 2023. 📖 [📂 Link](){:target="_blank"}.  
- Edgar Jesús Huaranga Junco. "Optimización del Consumo de Energía…" UNI, Peru. 2021. [📂 Link](http://hdl.handle.net/20.500.14076/22835){:target="_blank"}.  
- Victor Giovanny Mondragón Ruiz. "Evaluación y optimización…" UNI, Peru. 2019. [📂 Link](http://hdl.handle.net/20.500.14076/18948){:target="_blank"}.  
- Javier Enrique Villegas Herrera. “Desarrollo de un sistema IoT…” UNI, Perú. 2018. [📂 Link](http://hdl.handle.net/20.500.14076/18443){:target="_blank"}. 
- Jesús Enrique Lovón Melgarejo. “Técnicas para la localización en interiores…” UNI, Perú. 2018. [📂 Link](http://hdl.handle.net/20.500.14076/15999){:target="_blank"}.
- Eduardo Yauri Lozano. “SnorUNI: Aplicación móvil…” UNI, Perú. 2017. [📂 Link](http://hdl.handle.net/20.500.14076/5651){:target="_blank"}.

---

## 📚 **Courses, Workshops & Tutorials** {: .section-title}
- Advanced Techniques in Deep Learning. Universidad Diego Portales, Chile. 2021-2022.  
- Big Data, Machine Learning, Deep Learning for Business Engineering. UNJBG, Peru. 2021-2022.  
- Deep Learning for Computer Vision. Universidad Nacional de Cajamarca, Peru. 2020-2021.  
- Machine Learning with Python & Deep Learning with Python. UPCH, Peru. 2018-2020.  
- Data Analytics with R. UPCH, Peru. 2018-2020.  
- Scientific Texts with LaTeX. UPCH, Peru. 2018-2019.  

</div>