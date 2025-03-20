---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
📚 También puedes encontrar mis artículos en <a href="{{author.googlescholar}}" style="text-decoration: underline; font-weight: bold;">Google Scholar</a>.
{% endif %}

{% include base_path %}

## 📝 **Lista de Publicaciones**
{% for post in site.publications reversed %}
  <div style="padding: 1rem 0; border-bottom: 2px solid #ddd;">
    {% include archive-single.html %}
  </div>
{% endfor %}

---

## 📖 **Journals**  
### 🔍 Todas las publicaciones están disponibles en:
- 🔗 [**Google Scholar**](https://scholar.google.es/citations?hl=es&authuser=2&user=r0JytwIAAAAJ){:target="_blank"}  
- 🔗 [**Scopus**](https://www.scopus.com/authid/detail.uri?authorId=57200871251){:target="_blank"}  
- 🔗 [**Web of Science**](https://www.webofscience.com/wos/author/record/O-9762-2017){:target="_blank"}  
- 🔗 [**UNED Researcher**](https://portalcientifico.uned.es/investigadores/818430/detalle){:target="_blank"}  
- 🔗 [**UNED Professor**](https://www.uned.es/universidad/docentes/informatica/jose-manuel-castillo-cara.html){:target="_blank"}  

---

## 🏆 **Últimos 10 Artículos**
{% for paper in site.data.publications limit:10 %}
  <div style="padding: 1rem 0; border-bottom: 1px solid #ccc;">
    <b>{{ paper.authors }}</b>.  
    <i>{{ paper.title }}</i>.  
    <b>{{ paper.journal }}</b>, {{ paper.year }}.  
    📌 DOI: <a href="{{ paper.doi }}" target="_blank" style="color: blue;">{{ paper.doi }}</a>  
    (IF: {{ paper.if }}, {{ paper.rank }} – SJR: {{ paper.sjr }}, {{ paper.q }})  
  </div>
{% endfor %}

## 📚 **Libros y Capítulos**
- **Hancco _et al_**. Cost-Effective Advanced Remote Diagnostics of Sucker Rod Pumping Wells From Dynamometric Charts: A Deep Learning Approach. _IGI Global_, 2024. DOI: [10.4018/979-8-3693-0740-3.ch009](https://doi.org/10.4018/979-8-3693-0740-3.ch009){:target="_blank"}
- **Manuel Castillo-Cara.** GeoGebra en el Aula. Aplicaciones Matemáticas aplicadas al aula con GeoGebra.  
📖 ISBN: 9798379088873, Ed. Amazon. [📕 Ver libro](https://www.manuelcastillo.eu/portfolio/portfolio-1/){:target="_blank"}.

## 💻 **Software Registrado**
- **TINTORERA** – Manuel Castillo-Cara y Raúl García Castro. Registro Propiedad Intelectual: 16/2023/4624  
- **TINTORETTO** – Manuel Castillo-Cara y Raúl García Castro. Registro Propiedad Intelectual: 16/2023/5491  

## 🏅 **Patentes**
- **Dispositivo electrónico para seguimiento y localización de personas o animales**  
   Expediente: 002758-2016/DIN | Resolución: 000417-2019/DIN-INDECOPI | Título N.º: 1151, Perú, 2019.


## 🎓 **Tutoriales Internacionales**
- **Improving Deep Learning by Exploiting Synthetic Images**. *27th European Conference on Artificial Intelligence (ECAI)*, 2024  
   [Link al evento](https://www.ecai2024.eu/programme/tutorials) | [📂 Materiales](https://github.com/DCY1117/ECAI2024-Material){:target="_blank"}  

## 🏆 **Competiciones Internacionales**
- **3er lugar** – IEEE OPEN XVIII Latin American Robotics Competition (LARC/CBR). *Robot con navegación autónoma usando lógica difusa y visión inteligente*  
- **3er lugar** – IEEE OPEN XVII Latin American Robotics Competition (LARC/CBR). *Robot rápido y preciso para mover pequeños contenedores*  


## 📜 **Informes Técnicos**
- **Principles and recommendations to make data.europa.eu data more reusable**. *European Data Portal, Publications Office of the European Union*, 2022  
DOI: [10.2830/9342](https://doi.org/10.2830/9342){:target="_blank"}  


## 🌍 **Congresos Internacionales**
- **Rodrigo M. Carrillo-Larco _et al_**. Phenotypes of non-alcoholic fatty liver disease (NAFLD) and all-cause mortality. *2022 Annual Meeting of the American College of Epidemiology*, USA, 2022. DOI: [10.1016/j.annepidem.2022.08.036](https://doi.org/10.1016/j.annepidem.2022.08.036){:target="_blank"}  
- **Lovón-Melgarejo, J. _et al_**. *16Th International Multi-Conference for Engineering, Education, and Technology (LACCEI)*, Perú, 2018.  
DOI: [10.18687/laccei2018.1.1.413](https://doi.org/10.18687/laccei2018.1.1.413){:target="_blank"}  
- **Gusseppe Bravo Rocca _et al_**. *8th IEEE Latin-American Conference on Communications (LATINCOM)*, Colombia, 2016.  
DOI: [10.1109/LATINCOM.2016.7811562](https://doi.org/10.1109/LATINCOM.2016.7811562){:target="_blank"}  
