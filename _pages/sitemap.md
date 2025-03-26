---
layout: archive
title: "🗺️ Sitemap"
permalink: /sitemap/
author_profile: true
description: "Visual sitemap of all content on the website: pages, posts and collections."
---

{% include base_path %}

A list of all the posts, pages and collections on this site.  
For search engines, there's also an [**XML version**]({{ base_path }}/sitemap.xml).

---

## 📄 Pages
{% for page in site.pages %}
  {% unless page.title == nil or page.title == "" or page.exclude_from_nav == true %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}

---

## 📝 Blog Posts
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

---

## 📦 Collections

{% assign written_label = '' %}
{% for collection in site.collections %}
  {% unless collection.output == false or collection.label == "posts" %}
    {% capture label %}{{ collection.label | capitalize }}{% endcapture %}
    {% if label != written_label %}
      <h2 style="margin-top: 2rem;">📁 {{ label }}</h2>
      {% assign written_label = label %}
    {% endif %}
    {% for post in collection.docs %}
      {% include archive-single.html %}
    {% endfor %}
  {% endunless %}
{% endfor %}