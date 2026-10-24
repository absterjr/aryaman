# Aryaman — Personal Website

Personal portfolio for Aryaman: data engineering, analytics products, and independent projects.

**Live:** https://absterjr.github.io/aryaman/

## Stack

- HTML5, CSS3, and JavaScript
- SCSS sources compiled to `assets/css/main.css` (base theme) and `assets/css/custom.css` (site styles)
- [jQuery](https://jquery.com)
- [Font Awesome 5](https://fontawesome.com)
- [HTML5 UP Dimension](https://html5up.net/dimension) template (CC BY 3.0)

## Structure

- `index.html` — single page with hash-routed sections
- `assets/css/main.css` — compiled Dimension theme
- `assets/css/custom.css` — compiled site-specific styles
- `assets/sass/` — SCSS sources for both stylesheets
- `assets/js/main.js` — section routing, focus handling, and transitions
- `images/` — optimized WebP project images and background, the source profile photo, and favicons
- `Aryaman_Resume.pdf` — downloadable CV

## Local development

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

To rebuild the custom styles after editing `assets/sass/components/_custom.scss`:

```bash
npx sass assets/sass/custom.scss assets/css/custom.css --no-source-map
```

To rebuild the base theme after editing the other SCSS partials:

```bash
npx sass assets/sass/main.scss assets/css/main.css --no-source-map
```

## Deployment

Pushes to `main` deploy to GitHub Pages through `.github/workflows/static.yml`.
