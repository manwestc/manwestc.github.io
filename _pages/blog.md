---
layout: archive
title: "Blog & Tutorials"
permalink: /blog/
author_profile: true
description: "Technical tutorials and research notes on TINTOlib, tabular-to-image transformation, synthetic image generation from tabular data, deep learning, PyTorch, explainable AI and applied machine learning."
excerpt: "Tutorials on TINTOlib, tabular-to-image transformation, synthetic images, deep learning, PyTorch and applied machine learning."
---

{% include base_path %}

<!-- SEO metadata -->
<link rel="canonical" href="{{ site.url }}{{ page.url }}">
<meta name="robots" content="index,follow,max-image-preview:large">
<meta name="description" content="{{ page.description }}">

<!-- Open Graph metadata -->
<meta property="og:title" content="{{ page.title }} · Manuel Castillo-Cara">
<meta property="og:description" content="{{ page.description }}">
<meta property="og:type" content="website">
<meta property="og:url" content="{{ site.url }}{{ page.url }}">
<meta property="og:image" content="{{ site.url }}/images/profile.jpg">

<!-- Twitter Card metadata -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="{{ page.title }} · Manuel Castillo-Cara">
<meta name="twitter:description" content="{{ page.description }}">
<meta name="twitter:image" content="{{ site.url }}/images/profile.jpg">

<!-- JSON-LD structured data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "CollectionPage",
  "name": {{ page.title | append: " — Manuel Castillo-Cara" | jsonify }},
  "url": "{{ site.url }}{{ page.url }}",
  "description": {{ page.description | jsonify }},
  "author": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "url": "{{ site.url }}"
  },
  "publisher": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "url": "{{ site.url }}"
  },
  "about": [
    "TINTOlib",
    "TINTO",
    "tabular-to-image transformation",
    "synthetic image generation",
    "tabular data",
    "spatial feature encoding",
    "deep learning",
    "computer vision",
    "convolutional neural networks",
    "hybrid neural networks",
    "PyTorch",
    "Scikit-Learn",
    "explainable artificial intelligence"
  ],
  "keywords": "TINTOlib, TINTO, tabular-to-image, synthetic images, tabular data, spatial encoding, CNN, PyTorch, deep learning, hybrid neural networks, explainable AI",
  "mainEntity": [
    {% assign published_posts = site.posts | where_exp: "p", "p.published != false" %}
    {% for post in published_posts %}
    {
      "@type": "BlogPosting",
      "headline": {{ post.title | jsonify }},
      "url": "{{ site.url }}{{ post.url }}",
      "datePublished": "{{ post.date | date_to_xmlschema }}",
      "description": {{ post.description | default: post.excerpt | strip_html | jsonify }}
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

  /* Hide layout-rendered title (hero replaces it) */
  .page__title {
    display: none !important;
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
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
  }

  .blog-hero-icon {
    font-size: 2.8rem;
    line-height: 1;
  }

  .blog-hero h1 {
    margin: 0 0 0.2rem;
    font-size: 1.7rem;
    line-height: 1.2;
  }

  .blog-hero p {
    margin: 0;
    opacity: 0.9;
    font-size: 0.95rem;
  }

  /* ===== Search ===== */
  .blog-search-wrap {
    position: relative;
    margin-bottom: 1rem;
  }

  .blog-search-icon {
    position: absolute;
    left: 0.85rem;
    top: 50%;
    transform: translateY(-50%);
    color: var(--muted);
    pointer-events: none;
    font-size: 1rem;
  }

  .blog-search {
    width: 100%;
    box-sizing: border-box;
    padding: 0.6rem 1rem 0.6rem 2.4rem;
    border: 1px solid var(--bd);
    border-radius: 999px;
    font-size: 0.95rem;
    color: var(--ink);
    background: #fff;
    outline: none;
    transition: border-color 0.15s, box-shadow 0.15s;
  }

  .blog-search:focus {
    border-color: var(--brand);
    box-shadow: 0 0 0 3px rgba(25, 118, 210, 0.15);
  }

  /* ===== Filters ===== */
  .blog-filters {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-bottom: 1.4rem;
    padding: 0;
    list-style: none;
  }

  .blog-filter-btn {
    background: #f0f4f8;
    border: 1px solid var(--bd);
    border-radius: 999px;
    padding: 0.4rem 1rem;
    font-size: 0.9rem;
    font-weight: 700;
    color: var(--ink);
    cursor: pointer;
    transition: background 0.15s, color 0.15s, border-color 0.15s;
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

  /* ===== Card grid ===== */
  .blog-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1.1rem;
    align-items: stretch;
  }

  @media (max-width: 900px) {
    .blog-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }
  }

  @media (max-width: 560px) {
    .blog-grid {
      grid-template-columns: 1fr;
    }
  }

  /* ===== Card ===== */
  .blog-card {
    background: var(--card-bg);
    border: 1px solid var(--bd);
    border-radius: 12px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
    transition: box-shadow 0.15s, transform 0.12s;
  }

  .blog-card:hover {
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
    transform: translateY(-2px);
  }

  .blog-card[hidden] {
    display: none !important;
  }

  .blog-card-thumb {
    width: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
    display: block;
    background: #e8edf5;
  }

  .blog-card-body {
    padding: 0.85rem 0.9rem 1rem;
    display: flex;
    flex-direction: column;
    flex: 1;
  }

  .blog-card-meta {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.8rem;
    color: var(--muted);
    margin-bottom: 0.4rem;
    flex-wrap: wrap;
  }

  .blog-card-cat {
    background: #e0ecff;
    color: #0f3d8a;
    font-weight: 700;
    font-size: 0.75rem;
    padding: 0.15rem 0.5rem;
    border-radius: 999px;
  }

  .blog-card-title {
    font-size: 1rem;
    font-weight: 800;
    color: var(--grad-a);
    line-height: 1.3;
    margin: 0 0 0.45rem;
  }

  .blog-card-title a {
    color: inherit;
    text-decoration: none;
  }

  .blog-card-title a:hover {
    text-decoration: underline;
  }

  .blog-card-excerpt {
    font-size: 0.88rem;
    color: var(--ink);
    line-height: 1.5;
    flex: 1;
    margin-bottom: 0.6rem;
  }

  .blog-card-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.3rem;
    margin-bottom: 0.75rem;
  }

  .blog-tag {
    background: #f1f5f9;
    border: 1px solid #cbd5e1;
    color: var(--muted);
    font-size: 0.75rem;
    padding: 0.12rem 0.45rem;
    border-radius: 999px;
  }

  .blog-btn {
    display: inline-block;
    background: var(--brand);
    color: #fff !important;
    text-decoration: none !important;
    padding: 0.45rem 0.9rem;
    border-radius: 10px;
    font-weight: 800;
    font-size: 0.88rem;
    text-align: center;
    transition: background 0.15s, transform 0.06s, box-shadow 0.15s;
    align-self: flex-start;
  }

  .blog-btn:hover {
    background: var(--brand-2);
    transform: translateY(-1px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.12);
  }

  /* ===== Empty state ===== */
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
    margin-bottom: 0.6rem;
  }

  .blog-empty h3 {
    margin: 0 0 0.5rem;
    color: var(--ink);
    font-size: 1.1rem;
  }

  .blog-empty p {
    margin: 0 auto;
    font-size: 0.95rem;
    max-width: 480px;
  }

  /* ===== No search results ===== */
  .blog-no-results {
    display: none;
    text-align: center;
    padding: 2rem 1rem;
    color: var(--muted);
    font-size: 0.95rem;
  }
</style>

{% assign published_posts = site.posts | where_exp: "p", "p.published != false" %}

<!-- Hero -->
<div class="blog-hero">
  <div class="blog-hero-icon">✍️</div>

  <div>
    <h1>Blog &amp; Tutorials</h1>

    <p>
      Technical tutorials, research notes and reproducible examples on
      TINTOlib, tabular-to-image transformation, synthetic image generation
      from tabular data, hybrid neural networks, explainable AI and applied
      deep learning.
    </p>

    <p style="margin: 0.35rem 0 0; font-size: 0.82rem; opacity: 0.8;">
      By Manuel Castillo-Cara, PhD — Researcher and Professor at UNED,
      developer of TINTO and TINTOlib.
    </p>
  </div>
</div>

{% if published_posts.size == 0 %}

  <!-- Empty state: no published posts -->
  <div class="blog-empty" style="display: block;">
    <div class="blog-empty-icon">📝</div>

    <h3>Content coming soon</h3>

    <p>
      Articles about TINTOlib, artificial intelligence, Python, R,
      deep learning and teaching will be published soon.
    </p>
  </div>

{% else %}

  <!-- Search -->
  <div class="blog-search-wrap">
    <span class="blog-search-icon" aria-hidden="true">🔍</span>

    <input
      type="search"
      id="blog-search"
      class="blog-search"
      placeholder="Search articles…"
      aria-label="Search articles"
      autocomplete="off"
    >
  </div>

  <!-- Filters -->
  <div
    role="tablist"
    aria-label="Filter articles by topic"
    class="blog-filters"
  >
    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="true"
      data-filter=""
    >
      All
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="tintolib"
    >
      TINTOlib
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="clusters"
    >
      Clusters()
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="tabular-to-image"
    >
      Tabular-to-Image
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="synthetic images"
    >
      Synthetic Images
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="artificial intelligence"
    >
      Artificial Intelligence
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="python"
    >
      Python
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="deep learning"
    >
      Deep Learning
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="teaching"
    >
      Teaching
    </button>

    <button
      type="button"
      role="tab"
      class="blog-filter-btn"
      aria-selected="false"
      data-filter="research"
    >
      Research
    </button>
  </div>

  <!-- Card grid -->
  <div class="blog-grid" id="blog-grid">
    {% for post in published_posts %}
      {% assign post_image = post.image | default: post.header.teaser %}
      {% assign post_category = post.categories | first | default: post.category %}
      {% assign post_tags_str = post.tags | join: " " | downcase %}
      {% assign post_cats_str = post.categories | join: " " | downcase | append: " " | append: post.category | downcase %}

      {% capture search_blob %}
        {{ post.title }}
        {{ post.tags | join: " " }}
        {{ post.categories | join: " " }}
        {{ post.category }}
        {{ post.description }}
        {{ post.excerpt | strip_html }}
      {% endcapture %}

      <article
        class="blog-card"
        data-search="{{ search_blob | strip_newlines | downcase | escape }}"
        data-tags="{{ post_tags_str }} {{ post_cats_str }}"
      >
        {% if post_image %}
          <img
            class="blog-card-thumb"
            src="{{ post_image | relative_url }}"
            alt="{{ post.title | escape }}"
            loading="lazy"
          >
        {% endif %}

        <div class="blog-card-body">
          <div class="blog-card-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%d %b %Y" }}
            </time>

            {% if post_category %}
              <span class="blog-card-cat">
                {{ post_category }}
              </span>
            {% endif %}
          </div>

          <h2 class="blog-card-title">
            <a href="{{ post.url | relative_url }}">
              {{ post.title }}
            </a>
          </h2>

          {% assign excerpt_text = post.description | default: post.excerpt | strip_html | truncate: 130 %}

          {% if excerpt_text %}
            <p class="blog-card-excerpt">
              {{ excerpt_text }}
            </p>
          {% endif %}

          {% if post.tags.size > 0 %}
            <div class="blog-card-tags">
              {% for tag in post.tags limit: 4 %}
                <span class="blog-tag">
                  {{ tag }}
                </span>
              {% endfor %}
            </div>
          {% endif %}

          <a
            class="blog-btn"
            href="{{ post.url | relative_url }}"
          >
            Read article →
          </a>
        </div>
      </article>
    {% endfor %}
  </div>

  <div
    class="blog-no-results"
    id="blog-no-results"
    role="status"
    aria-live="polite"
  >
    No articles found for the selected criteria.
  </div>

  <script>
  (function () {
    "use strict";

    function initializeBlogFilters() {
      var searchInput = document.getElementById("blog-search");

      var filterButtons = Array.prototype.slice.call(
        document.querySelectorAll(".blog-filter-btn")
      );

      var cards = Array.prototype.slice.call(
        document.querySelectorAll("#blog-grid .blog-card")
      );

      var noResults = document.getElementById("blog-no-results");
      var activeFilter = "";

      if (
        !searchInput ||
        filterButtons.length === 0 ||
        cards.length === 0
      ) {
        console.warn("Blog filters could not be initialized.", {
          searchInput: Boolean(searchInput),
          filterButtons: filterButtons.length,
          cards: cards.length
        });

        return;
      }

      function normalizeText(value) {
        var text = String(value || "").toLowerCase();

        if (typeof text.normalize === "function") {
          text = text
            .normalize("NFD")
            .replace(/[\u0300-\u036f]/g, "");
        }

        return text.trim();
      }

      function applyFilters() {
        var query = normalizeText(searchInput.value);
        var visibleCards = 0;

        cards.forEach(function (card) {
          var searchableText = normalizeText(
            card.getAttribute("data-search")
          );

          var tags = normalizeText(
            card.getAttribute("data-tags")
          );

          var matchesSearch =
            query === "" ||
            searchableText.indexOf(query) !== -1;

          var matchesFilter =
            activeFilter === "" ||
            tags.indexOf(activeFilter) !== -1;

          var shouldShow =
            matchesSearch && matchesFilter;

          if (shouldShow) {
            card.removeAttribute("hidden");
            visibleCards += 1;
          } else {
            card.setAttribute("hidden", "");
          }
        });

        if (noResults) {
          noResults.style.display =
            visibleCards === 0 ? "block" : "none";
        }
      }

      function activateFilter(filterValue) {
        activeFilter = normalizeText(filterValue);
        var matched = false;

        filterButtons.forEach(function (button) {
          var buttonFilter = normalizeText(
            button.getAttribute("data-filter")
          );

          var isActive =
            buttonFilter === activeFilter;

          button.setAttribute(
            "aria-selected",
            isActive ? "true" : "false"
          );

          if (isActive) {
            matched = true;
          }
        });

        if (!matched) {
          activeFilter = "";

          filterButtons.forEach(function (button, index) {
            button.setAttribute(
              "aria-selected",
              index === 0 ? "true" : "false"
            );
          });
        }

        applyFilters();
      }

      searchInput.addEventListener(
        "input",
        applyFilters
      );

      searchInput.addEventListener(
        "search",
        applyFilters
      );

      filterButtons.forEach(function (button) {
        button.addEventListener("click", function () {
          var filterValue =
            button.getAttribute("data-filter") || "";

          activateFilter(filterValue);

          if (filterValue) {
            window.history.replaceState(
              null,
              "",
              window.location.pathname +
                window.location.search +
                "#" +
                encodeURIComponent(filterValue)
            );
          } else {
            window.history.replaceState(
              null,
              "",
              window.location.pathname +
                window.location.search
            );
          }
        });
      });

      var initialHash = decodeURIComponent(
        window.location.hash.replace(/^#/, "")
      );

      activateFilter(initialHash || "");

      console.info("Blog filters initialized.", {
        cards: cards.length,
        filters: filterButtons.length
      });
    }

    if (document.readyState === "loading") {
      document.addEventListener(
        "DOMContentLoaded",
        initializeBlogFilters
      );
    } else {
      initializeBlogFilters();
    }
  }());
  </script>

{% endif %}