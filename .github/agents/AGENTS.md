# Agent instructions for manuelcastillo.eu

This repository contains a Jekyll / GitHub Pages academic website for Manuel Castillo-Cara.

## Canonical domain

Use:

https://www.manuelcastillo.eu

Never use:

https://academicpages.github.io

## Deployment

The website is deployed through GitHub Pages.

Important consequence:

- Do not suggest `.htaccess`.
- Do not suggest Apache headers.
- Do not suggest server-side redirects unless explicitly discussing DNS or GitHub Pages settings.

## Main files

- `_config.yml`: global Jekyll configuration
- `_data/navigation.yml`: navigation menu
- `_pages/`: main pages
- `_talks/`: Udemy/course pages
- `_libros-software/`: books/software pages
- `_includes/`: reusable components
- `_layouts/`: layouts
- `assets/`: CSS/JS/assets
- `images/`: images
- `files/`: PDFs and downloadable files
- `video/`: videos

## Preferred practices

- Preserve existing permalinks.
- Preserve existing visual identity.
- Keep SEO metadata synchronized with visible content.
- Keep JSON-LD valid.
- Use relative URLs for internal links.
- Use DOI URLs for publications.
- Avoid duplicate pages and obsolete AcademicPages generator files.
- Do not reintroduce `markdown_generator/`.