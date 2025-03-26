---
layout: archive
title: "My Curriculum Vitae"
permalink: /cv/
author_profile: true
description: "Curriculum Vitae of Manuel Castillo-Cara: academic background, research lines, Udemy courses, projects, and publications."
redirect_from:
  - /resume
---

{% include base_path %}

## 🎓 Education
- **M.S. in Computer Science**, Universidad de Castilla-La Mancha (Spain).
- **Ph.D. in Computer Science**, Universidad de Castilla-La Mancha (Spain).  
  Thesis: [*Contributions to the advancement of wireless indoor localization techniques: signal characterization and distributed computing*](https://ruidera.uclm.es/xmlui/handle/10578/19354){:target="_blank"}

## 💼 Work Experience
- **2023 – Present**: Professor & Researcher, AI Department, UNED, Spain.  
- **2021 – 2023**: Postdoctoral Fellow, Ontology Engineering Group, UPM, Spain.  
- **2020**: Professor, Universidad de Lima, Peru.  
- **2019 – 2020**: Head of Office, Technology Infrastructure, Ministry of Education, Peru.  
- **2014 – 2019**: Professor, Universidad Nacional de Ingeniería, Peru.  
- **2015 – 2019**: Head, Center of IT & Communication, Universidad Nacional de Ingeniería, Peru.

## 🔬 Research Lines
- **Wireless Sensor Networks**
  - Indoor Localization
  - Fog/Edge Computing
  - Internet of Things (IoT)
- **Artificial Intelligence**
  - Data Science
  - Pattern Recognition
  - Computer Vision

---

### 📚 Udemy Courses

### Inteligencia Artificial con Python
<ul>
{% assign cursos_python = site.talks | where: "category", "Inteligencia Artificial con Python:" %}
{% for post in cursos_python %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

### Inteligencia Artificial con R
<ul>
{% assign cursos_r = site.talks | where: "category", "Inteligencia Artificial con R:" %}
{% for post in cursos_r %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

### Otros cursos de formación avanzada
<ul>
{% assign cursos_otros = site.talks | where: "category", "Otros cursos de formación avanzada:" %}
{% for post in cursos_otros %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

---

## 💻 Books, Software & Patents

### Books
<ul>
{% assign books = site.portfolio | where: "category", "Books" %}
{% for post in books %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

### Software
<ul>
{% assign software = site.portfolio | where: "category", "Software" %}
{% for post in software %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

### Patents
<ul>
{% assign patents = site.portfolio | where: "category", "Patents" %}
{% for post in patents %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

---

## 📄 Publications
All publications are listed on:
- [Website](https://manuelcastillo.eu/publications/)
- [Google Scholar](https://scholar.google.es/citations?hl=es&authuser=2&user=r0JytwIAAAAJ)
- [Scopus](https://www.scopus.com/authid/detail.uri?authorId=57200871251)
- [Web of Science](https://www.webofscience.com/wos/author/record/O-9762-2017)

## 🧪 Competitive R&D&i Projects
- **Co-investigator**. "Cost-Effective Screening of Breast Cancer and Rheumatic Heart Disease Using AI", PID2023-150515OB-I00, Spain (2024–2027).
- **Co-investigator**. "Development of HPC and data center applications", PID2021-123627OB-C52, Spain (2022–2025).
- **Co-investigator**. "Supercapacitor-based charging system", 026-FONDECYT-BM-INC.INV, Peru (2020–2022).
- **Co-investigator**. "Energy storage from microbial fuel cells", 401-FONDECYT, Peru (2020–2023).
- **Co-investigator**. "AgIoT: Agricultural IoT and analytics", CYTED, International (2020–2022).
- **Principal Investigator**. "Ubiquitous Smart Technologies", 138-2017-FONDECYT, Peru (2017–2020).
- **Principal Investigator**. "Smart City for geolocation", PIAP-363, Peru (2014–2017).
- **Co-investigator**. "Optimization of multimedia content distribution", TIN2015-66972-C05-2-R, Spain (2017–2018).
- **Co-investigator**. "Genetic expression analysis in microgravity", PIAP-1-P-622-13, Peru (2013–2016).

---

## 👨‍🏫 Teaching Experience

### Doctoral
- **2021–2022**: *Research Methodology*, PhD CS, UCLM, Spain.
- **2021–2022**: *Artificial Neural Networks and Deep Learning*, PhD CS, Universidad de Almería, Spain.

### Master’s
- **2023–Present**: *Data Mining & Deep Learning*, MSc AI, UNED, Spain.
- **2023–Present**: *Machine Learning II & Deep Learning*, MSc Eng. & Data Science, UNED, Spain.
- **2020–2022**: *International Seminar I*, MSc Strategic Content Mgmt., Universidad de Lima, Peru.
- **2019–2020**: *Machine Learning & Data Mining*, MSc CS, Universidad Nacional de Ingeniería, Peru.

### Undergraduate
- **2022–2023**: *Probability and Statistics I*, BSc CS, UPM, Spain.
- **2021**: *Workshop on Research Proposal*, BSc CS, Universidad de Lima, Peru.
- **2014–2020**: *Network Management*, BSc CS, UNI, Peru.
- **2015–2020**: *Thesis Seminar*, BSc CS, UNI, Peru.
- **2013–2017**: *Programming Fundamentals*, BSc CS, UNI, Peru.
- **2015–2017**: *Mobile Programming*, BSc CS, UNI, Peru.
- **2013–2014**: *Algorithms*, BSc CS, UNI, Peru.