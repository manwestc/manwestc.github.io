---
layout: single
title: "GeoGebra en el Aula. Aplicaciones Matemáticas aplicadas al aula con GeoGebra"
excerpt: "Libro práctico para aplicar GeoGebra en el aula con módulos de geometría, estadística, álgebra y análisis. Incluye acceso gratuito a un curso de Udemy y materiales descargables."
collection: libros-software
category: "Books"
image: "/images/geogebra.png"
permalink: /libros-software/libro-curso-GeoGebra-Aula/
author_profile: true
show_date: false
read_time: false
share: false
related: false
---

{% include base_path %}

<!-- ✅ SEO básico -->
<link rel="canonical" href="{{ site.url }}{{ page.permalink }}">
<meta name="robots" content="index,follow">
<meta name="description" content="Libro 'GeoGebra en el Aula' con módulos de geometría, álgebra, estadística, análisis y 3D. Incluye curso Udemy gratuito y materiales descargables.">

<!-- ✅ Open Graph / Twitter -->
<meta property="og:title" content="Libro: GeoGebra en el Aula — Aplicaciones Matemáticas">
<meta property="og:description" content="Libro práctico para aplicar GeoGebra en el aula. Incluye curso Udemy gratuito y recursos descargables.">
<meta property="og:type" content="book">
<meta property="og:url" content="{{ site.url }}{{ page.permalink }}">
<meta property="og:image" content="{{ site.url }}{{ page.image }}">
<meta property="og:image:width" content="1200"><meta property="og:image:height" content="630">

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Libro: GeoGebra en el Aula — Aplicaciones Matemáticas">
<meta name="twitter:description" content="Módulos de geometría, álgebra, estadística, análisis y 3D. Con curso Udemy gratuito.">
<meta name="twitter:image" content="{{ site.url }}{{ page.image }}">

<!-- ✅ JSON-LD (Book + Offer) -->
<script type="application/ld+json">
{
  "@context":"https://schema.org",
  "@type":"Book",
  "name":"GeoGebra en el Aula. Aplicaciones Matemáticas aplicadas al aula con GeoGebra",
  "author":{"@type":"Person","name":"Manuel Castillo-Cara","url":"https://www.manuelcastillo.eu/"},
  "description":"Libro educativo para el uso práctico de GeoGebra en el aula. Incluye módulos sobre geometría, álgebra, estadística, análisis y geometría 3D, además de recursos descargables y acceso a curso online.",
  "image":"{{ site.url }}{{ page.image }}",
  "url":"{{ site.url }}{{ page.permalink }}",
  "publisher":{"@type":"Organization","name":"Autoedición"},
  "inLanguage":"es",
  "offers":{
    "@type":"Offer",
    "price":"20.00",
    "priceCurrency":"EUR",
    "availability":"https://schema.org/InStock",
    "url":"{{ site.url }}{{ page.permalink }}"
  }
}
</script>

<!-- 🎨 Estilos unificados -->
<style>
  :root{
    --ink:#1f2937; --muted:#6b7280; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8;
    --cta:#2563eb; --cta-hover:#1d4ed8; --cta-soft:#eaf1ff;
  }
  .book-wrap{max-width:1050px;margin:0 auto;padding:0 1rem}

  /* HERO */
  .book-hero{
    display:flex; gap:1rem; align-items:center; flex-wrap:wrap;
    background:linear-gradient(135deg,#1d4ed8 0%, #9333ea 100%);
    color:#fff; border-radius:14px; padding:1rem 1.25rem; margin:1.25rem 0 1rem;
    box-shadow:0 8px 24px rgba(0,0,0,.08);
  }
  .book-hero img{
    width:120px; height:120px; object-fit:cover; border-radius:12px;
    background:#fff; border:2px solid rgba(255,255,255,.7);
  }
  .book-hero h1{font-size:1.6rem; margin:.1rem 0 .3rem; line-height:1.2}
  .book-hero p{margin:0; opacity:.95}
  .hero-actions{display:flex; justify-content:center; align-items:center; gap:.6rem; flex-wrap:wrap; margin-top:.8rem; text-align:center}

  /* Botones */
  .btn{display:inline-block; padding:.65em 1.05em; border-radius:10px; font-weight:800; text-decoration:none; border:0; cursor:pointer; transition: transform .06s ease, box-shadow .15s ease, background-color .15s ease;}
  .btn:hover{ transform:translateY(-1px); box-shadow:0 6px 16px rgba(0,0,0,.18) }
  .btn-primary{ background:var(--cta); color:#fff !important; }
  .btn-primary:hover{ background:var(--cta-hover) !important; }
  .btn-ghost{ background:#1e40af; color:#fff !important; border:none; }
  .btn-ghost:hover{ background:#1e3a8a; }

  /* Secciones */
  .section-title{
    display:flex; align-items:center; gap:.5rem;
    font-size:1.25rem; font-weight:800; color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand);
    border-radius:12px; padding:.5rem .8rem; margin:1.3rem 0 .8rem;
  }
  .section-title::after{
    content:""; flex:1; height:3px; margin-left:.6rem;
    background:linear-gradient(to right,#4a90e2,#e91e63); border-radius:2px;
  }

  .card{ background:var(--card); border:1px solid var(--bd); border-radius:12px; padding:1rem; box-shadow:0 2px 10px rgba(0,0,0,.04); }
  .list{ margin:.35rem 0 0; padding-left:1.1rem }
  .list li{ margin:.28rem 0; line-height:1.55 }

  /* Bloque compra */
  .buy-card{
    display:flex; flex-direction:column; gap:.6rem; align-items:center; text-align:center;
    background:linear-gradient(180deg,#ffffff,#f7f9ff);
    border:1px solid var(--bd); border-radius:12px; padding:1rem;
    box-shadow:0 2px 10px rgba(0,0,0,.05);
  }
  .price{font-size:1.35rem; font-weight:900; color:#0b3e99}

  /* CTA inferior grande */
  .cta-center{ display:flex; justify-content:center; margin:2rem 0; }
  .cta-center .btn-primary{ padding:1em 2.5em; font-size:1.1rem; min-width:clamp(240px,40vw,420px); text-align:center; box-shadow:0 4px 12px rgba(0,0,0,.15); }

  /* Ocultar meta del theme */
  .page__meta, .page__meta-title, .page__taxonomy, .page__date{ display:none !important; }
</style>

<div class="book-wrap">

  <!-- HERO -->
  <section class="book-hero">
    <img src="{{ page.image }}" alt="Portada del libro GeoGebra en el Aula">
    <div style="flex:1">
      <h1>GeoGebra en el Aula — Libro práctico para docentes</h1>
      <p>Módulos de geometría, álgebra, estadística, análisis y 3D. Incluye materiales descargables y acceso gratuito a un curso en Udemy.</p>
      <div class="hero-actions">
        <a class="btn btn-primary" href="#resumen">Ver resumen</a>
        <a class="btn btn-ghost" href="#contenidos">Ver contenidos</a>
      </div>
    </div>
  </section>

  <!-- RESUMEN -->
  <div id="resumen" class="card">
    <h2 class="section-title">📘 Resumen</h2>
    <p>Este recurso didáctico fomenta el uso de <strong>GeoGebra</strong> en el aula para facilitar y enriquecer la labor docente. El libro <strong>“GeoGebra en el Aula. Aplicaciones Matemáticas aplicadas al aula con GeoGebra”</strong> ofrece un aprendizaje práctico y progresivo para el alumnado.</p>
    <p>GeoGebra permite crear <em>construcciones dinámicas</em> exportables a la web, manipulando expresiones geométricas, numéricas, algebraicas o tabulares para comprender relaciones y propiedades matemáticas.</p>
    <p>Los materiales están pensados como herramientas útiles para la <strong>adquisición de conceptos</strong> y la <strong>participación activa</strong> del alumnado.</p>
  </div>

  <!-- CONTENIDOS -->
  <div id="contenidos" class="card">
    <h2 class="section-title">📚 Contenidos del Libro</h2>
    <ul class="list">
      <li>Introducción e <strong>Iniciación a GeoGebra</strong></li>
      <li><strong>Movimientos en el plano</strong></li>
      <li><strong>Estadística y Probabilidad</strong></li>
      <li><strong>Álgebra</strong> con GeoGebra</li>
      <li><strong>Aplicaciones al Análisis</strong></li>
      <li><strong>Geometría Espacial</strong> (GeoGebra 3D)</li>
    </ul>
  </div>

  <!-- QUÉ INCLUYE -->
  <div class="card">
    <h2 class="section-title">🎁 ¿Qué incluye la compra?</h2>
    <ul class="list">
      <li>📕 <strong>Libro en PDF</strong></li>
      <li>🎥 <strong>Vídeos tutoriales</strong></li>
      <li>📂 <strong>Archivos fuente de GeoGebra</strong></li>
      <li>🎓 Acceso <strong>gratuito</strong> al <a href="https://www.udemy.com/course/matematicas-geogebra/?couponCode=AGO_2025" target="_blank" rel="noopener">curso en Udemy</a></li>
    </ul>
  </div>

  <!-- PRECIO & COMPRA -->
  <div class="buy-card">
    <div class="price">💰 Precio: <strong>20€</strong></div>
    <p style="margin:.1rem 0 .6rem; color:var(--muted)">Puedes comprarlo con PayPal o escribirme si prefieres otra forma de pago.</p>

    <!-- Botón PayPal (tu mismo ID, integrado) -->
    <div id="paypal-container-UX7UBGJ8TCPTW"></div>

    <div style="margin-top:.4rem">
      <a class="btn btn-primary" href="mailto:manwest.c@gmail.com">📩 Solicitar factura o info</a>
    </div>
  </div>

  <!-- CTA inferior -->
  <div class="cta-center">
    <a class="btn btn-primary" href="https://www.udemy.com/course/matematicas-geogebra/?couponCode=AGO_2025" target="_blank" rel="noopener">🎓 Acceder al curso gratis en Udemy</a>
  </div>
</div>

<!-- SDK PayPal + Render -->
<script 
  src="https://www.paypal.com/sdk/js?client-id=BAAFLtzEbhR-v2Nk6YVEdhvWJzPrGcmQm4dOmmv6DDKyXomXKpToxESEA_da2HErs94WB2HVZrH396-SUg&components=hosted-buttons&disable-funding=venmo&currency=EUR">
</script>
<script>
  paypal.HostedButtons({ hostedButtonId: "UX7UBGJ8TCPTW" })
        .render("#paypal-container-UX7UBGJ8TCPTW");
</script>