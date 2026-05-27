---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
description: "Blog de Manuel Castillo-Cara sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia."
---

{% include base_path %}

<!-- ✅ SEO básico -->
<link rel="canonical" href="{{ site.url }}/blog/">
<meta name="robots" content="index,follow">
<meta name="description" content="Blog de Manuel Castillo-Cara sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia.">

<!-- ✅ Open Graph -->
<meta property="og:title" content="Blog · Manuel Castillo-Cara">
<meta property="og:description" content="Artículos sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia.">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}/blog/">
<meta property="og:image" content="{{ site.url }}/images/profile.jpg">

<!-- ✅ Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Blog · Manuel Castillo-Cara">
<meta name="twitter:description" content="Artículos sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia.">
<meta name="twitter:image" content="{{ site.url }}/images/profile.jpg">

<!-- ✅ JSON-LD Blog -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Blog",
  "name": "Blog de Manuel Castillo-Cara",
  "url": "{{ site.url }}/blog/",
  "description": "Artículos sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia.",
  "author": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "url": "{{ site.url }}"
  },
  "blogPost": [
    {% assign published_posts = site.posts | where_exp: "p", "p.published != false" %}
    {% for post in published_posts %}
    {
      "@type": "BlogPosting",
      "headline": "{{ post.title | escape }}",
      "url": "{{ site.url }}{{ post.url }}",
      "datePublished": "{{ post.date | date_to_xmlschema }}"
    }{% unless forloop.last %},{% endunless %}
    {% endfor %}
  ]
}
</script>

<style>
  :root {
    --ink: #1f2937;
    --muted: #6b7280;
    --bd: #cfd8dc;
    --card-bg: #f4f7fb;
    --frame: #ffffff;
    --brand: #1976d2;
    --brand-2: #0f60b6;
    --grad-a: #1565c0;
    --grad-b: #ff0f5e;
  }

  /* ===== Hero ===== */
  .blog-hero {
    display: flex;
    align-items: center;
    gap: 1rem;
    background: linear-gradient(135deg, #1565c0 0%, #6d28d9 100%);
    color: #fff;
    border-radius: 14px;
    padding: 1.25rem 1.5rem;
    margin: 0 0 1.5rem;
    box-shadow: 0 8px 24px rgba(0,0,0,.1);
  }
  .blog-hero-icon {
    font-size: 2.8rem;
    line-height: 1;
  }
  .blog-hero h1 {
    margin: 0 0 .2rem;
    font-size: 1.7rem;
    line-height: 1.2;
  }
  .blog-hero p {
    margin: 0;
    opacity: .9;
    font-size: .95rem;
  }

  /* ===== Buscador ===== */
  .blog-search-wrap {
    position: relative;
    margin-bottom: 1rem;
  }
  .blog-search-icon {
    position: absolute;
    left: .85rem;
    top: 50%;
    transform: translateY(-50%);
    color: var(--muted);
    pointer-events: none;
    font-size: 1rem;
  }
  .blog-search {
    width: 100%;
    box-sizing: border-box;
    padding: .6rem 1rem .6rem 2.4rem;
    border: 1px solid var(--bd);
    border-radius: 999px;
    font-size: .95rem;
    color: var(--ink);
    background: #fff;
    outline: none;
    transition: border-color .15s, box-shadow .15s;
  }
  .blog-search:focus {
    border-color: var(--brand);
    box-shadow: 0 0 0 3px rgba(25,118,210,.15);
  }

  /* ===== Filtros ===== */
  .blog-filters {
    display: flex;
    flex-wrap: wrap;
    gap: .4rem;
    margin-bottom: 1.4rem;
    padding: 0;
    list-style: none;
  }
  .blog-filter-btn {
    background: #f0f4f8;
    border: 1px solid var(--bd);
    border-radius: 999px;
    padding: .4rem 1rem;
    font-size: .9rem;
    font-weight: 700;
    color: var(--ink);
    cursor: pointer;
    transition: background .15s, color .15s, border-color .15s;
  }
  .blog-filter-btn:hover {
    background: #e0ecff;
    border-color: var(--brand);
    color: var(--brand);
  }
  .blog-filter-btn[aria-selected="true"] {
    background: var(--brand);
    color: #fff;
    border-color: var(--brand);
  }

  /* ===== Grid de tarjetas ===== */
  .blog-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0,1fr));
    gap: 1.1rem;
    align-items: stretch;
  }
  @media (max-width: 900px) {
    .blog-grid { grid-template-columns: repeat(2, minmax(0,1fr)); }
  }
  @media (max-width: 560px) {
    .blog-grid { grid-template-columns: 1fr; }
  }

  /* ===== Tarjeta ===== */
  .blog-card {
    background: var(--card-bg);
    border: 1px solid var(--bd);
    border-radius: 12px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    box-shadow: 0 2px 8px rgba(0,0,0,.05);
    transition: box-shadow .15s, transform .12s;
  }
  .blog-card:hover {
    box-shadow: 0 6px 20px rgba(0,0,0,.1);
    transform: translateY(-2px);
  }
  .blog-card[hidden] {
    display: none !important;
  }
  .blog-card-thumb {
    width: 100%;
    aspect-ratio: 16/9;
    object-fit: cover;
    display: block;
    background: #e8edf5;
  }
  .blog-card-body {
    padding: .85rem .9rem 1rem;
    display: flex;
    flex-direction: column;
    flex: 1;
  }
  .blog-card-meta {
    display: flex;
    align-items: center;
    gap: .5rem;
    font-size: .8rem;
    color: var(--muted);
    margin-bottom: .4rem;
    flex-wrap: wrap;
  }
  .blog-card-cat {
    background: #e0ecff;
    color: #0f3d8a;
    font-weight: 700;
    font-size: .75rem;
    padding: .15rem .5rem;
    border-radius: 999px;
  }
  .blog-card-title {
    font-size: 1rem;
    font-weight: 800;
    color: var(--grad-a);
    line-height: 1.3;
    margin: 0 0 .45rem;
  }
  .blog-card-title a {
    color: inherit;
    text-decoration: none;
  }
  .blog-card-title a:hover { text-decoration: underline; }
  .blog-card-excerpt {
    font-size: .88rem;
    color: var(--ink);
    line-height: 1.5;
    flex: 1;
    margin-bottom: .6rem;
  }
  .blog-card-tags {
    display: flex;
    flex-wrap: wrap;
    gap: .3rem;
    margin-bottom: .75rem;
  }
  .blog-tag {
    background: #f1f5f9;
    border: 1px solid #cbd5e1;
    color: var(--muted);
    font-size: .75rem;
    padding: .12rem .45rem;
    border-radius: 999px;
  }
  .blog-btn {
    display: inline-block;
    background: var(--brand);
    color: #fff !important;
    text-decoration: none !important;
    padding: .45rem .9rem;
    border-radius: 10px;
    font-weight: 800;
    font-size: .88rem;
    text-align: center;
    transition: background .15s, transform .06s, box-shadow .15s;
    align-self: flex-start;
  }
  .blog-btn:hover {
    background: var(--brand-2);
    transform: translateY(-1px);
    box-shadow: 0 4px 12px rgba(0,0,0,.12);
  }

  /* ===== Estado vacío ===== */
  .blog-empty {
    display: none;
    text-align: center;
    padding: 2.5rem 1rem;
    background: var(--card-bg);
    border: 1px solid var(--bd);
    border-radius: 14px;
    color: var(--muted);
  }
  .blog-empty-icon {
    font-size: 2.5rem;
    margin-bottom: .6rem;
  }
  .blog-empty h3 {
    margin: 0 0 .5rem;
    color: var(--ink);
    font-size: 1.1rem;
  }
  .blog-empty p {
    margin: 0;
    font-size: .95rem;
    max-width: 480px;
    margin: 0 auto;
  }

  /* ===== Sin resultados de búsqueda ===== */
  .blog-no-results {
    display: none;
    text-align: center;
    padding: 2rem 1rem;
    color: var(--muted);
    font-size: .95rem;
  }
</style>

{% assign published_posts = site.posts | where_exp: "p", "p.published != false" %}

<!-- Hero -->
<div class="blog-hero">
  <div class="blog-hero-icon">✍️</div>
  <div>
    <h1>Blog</h1>
    <p>Artículos sobre inteligencia artificial, TINTOlib, Python, R, deep learning y docencia.</p>
  </div>
</div>

{% if published_posts.size == 0 %}

  <!-- Estado vacío: no hay posts publicados -->
  <div class="blog-empty" style="display:block">
    <div class="blog-empty-icon">📝</div>
    <h3>Contenido próximamente</h3>
    <p>Próximamente se publicarán artículos sobre TINTOlib, inteligencia artificial, Python, R, deep learning y docencia.</p>
  </div>

{% else %}

  <!-- Buscador -->
  <div class="blog-search-wrap">
    <span class="blog-search-icon" aria-hidden="true">🔍</span>
    <input type="search" id="blog-search" class="blog-search"
           placeholder="Buscar artículos…" aria-label="Buscar artículos">
  </div>

  <!-- Filtros -->
  <div role="tablist" aria-label="Filtrar por categoría" class="blog-filters">
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="true"  data-filter="">Todos</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="tintolib">TINTOlib</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="ia python">IA Python</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="ia r">IA R</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="deep learning">Deep Learning</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="teaching">Teaching</button>
    <button type="button" role="tab" class="blog-filter-btn" aria-selected="false" data-filter="research">Research</button>
  </div>

  <!-- Grid de tarjetas -->
  <div class="blog-grid" id="blog-grid">
    {% for post in published_posts %}
      {% assign post_image = post.image | default: post.header.teaser %}
      {% assign post_category = post.categories | first | default: post.category %}
      {% assign post_tags_str = post.tags | join: " " | downcase %}
      {% assign post_cats_str = post.categories | join: " " | downcase | append: " " | append: post.category | downcase %}
      {% assign search_blob = post.title | downcase
          | append: " "
          | append: post_tags_str
          | append: " "
          | append: post_cats_str
          | append: " "
          | append: post.description | downcase
          | append: " "
          | append: post.excerpt | downcase %}

      <article class="blog-card"
               data-search="{{ search_blob | escape }}"
               data-tags="{{ post_tags_str }} {{ post_cats_str }}">

        {% if post_image %}
          <img class="blog-card-thumb"
               src="{{ post_image }}"
               alt="{{ post.title | escape }}"
               loading="lazy">
        {% endif %}

        <div class="blog-card-body">
          <div class="blog-card-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d %b %Y" }}</time>
            {% if post_category %}
              <span class="blog-card-cat">{{ post_category }}</span>
            {% endif %}
          </div>

          <h2 class="blog-card-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>

          {% assign excerpt_text = post.description | default: post.excerpt | strip_html | truncate: 130 %}
          {% if excerpt_text %}
            <p class="blog-card-excerpt">{{ excerpt_text }}</p>
          {% endif %}

          {% if post.tags.size > 0 %}
            <div class="blog-card-tags">
              {% for tag in post.tags limit: 4 %}
                <span class="blog-tag">{{ tag }}</span>
              {% endfor %}
            </div>
          {% endif %}

          <a class="blog-btn" href="{{ post.url | relative_url }}">Leer artículo →</a>
        </div>
      </article>
    {% endfor %}
  </div>

  <div class="blog-no-results" id="blog-no-results">
    No se encontraron artículos con esos criterios.
  </div>

  <script>
  (function () {
    var searchInput = document.getElementById('blog-search');
    var filterBtns  = document.querySelectorAll('.blog-filter-btn');
    var cards       = document.querySelectorAll('.blog-card');
    var noResults   = document.getElementById('blog-no-results');
    var activeFilter = '';

    function applyFilters() {
      var query = searchInput.value.trim().toLowerCase();
      var visible = 0;

      cards.forEach(function (card) {
        var searchBlob = card.dataset.search || '';
        var tags       = card.dataset.tags   || '';

        var matchSearch = query === '' || searchBlob.indexOf(query) !== -1;
        var matchFilter = activeFilter === '' || tags.indexOf(activeFilter) !== -1;

        if (matchSearch && matchFilter) {
          card.removeAttribute('hidden');
          visible++;
        } else {
          card.setAttribute('hidden', '');
        }
      });

      noResults.style.display = visible === 0 ? 'block' : 'none';
    }

    searchInput.addEventListener('input', applyFilters);

    filterBtns.forEach(function (btn) {
      btn.addEventListener('click', function () {
        filterBtns.forEach(function (b) { b.setAttribute('aria-selected', 'false'); });
        this.setAttribute('aria-selected', 'true');
        activeFilter = this.dataset.filter;
        applyFilters();
      });
    });
  }());
  </script>

{% endif %}
