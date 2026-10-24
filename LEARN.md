# Learn More

This site is a single-page portfolio built on the [HTML5 UP Dimension](https://html5up.net/dimension) template. It covers Aryaman's experience, skills, education, and the projects he builds outside work.

## How it is built

- HTML5, CSS3, and JavaScript
- SCSS sources in `assets/sass/`, compiled to `assets/css/main.css` and `assets/css/custom.css`
- [jQuery](https://jquery.com) for section routing and transitions
- [Font Awesome 5](https://fontawesome.com) for icons
- Hosted on GitHub Pages

The site is intentionally static: there is no build server, framework runtime, or database. Sections are opened through URL hashes (`#intro`, `#experience`, and so on), so individual sections can be linked directly.

## Accessibility notes

- All sections are reachable by keyboard, and focus moves to the opened section heading and back to the navigation on close.
- The close control is a real button.
- Icon links have accessible names for screen readers.
- The contact form uses native validation and a honeypot field for spam filtering.

## Images

Project screenshots and the hero background are optimized WebP files. The favicon is generated from the profile photo. The template's unused demo images were removed.

## Running locally

```bash
python -m http.server 8000
```

Open http://localhost:8000.

## Editing styles

Site-specific rules live in `assets/sass/components/_custom.scss`. Rebuild with:

```bash
npx sass assets/sass/custom.scss assets/css/custom.css --no-source-map
```

Base template rules live in the other SCSS partials and compile to `assets/css/main.css`.

## Deployment

Every push to `main` triggers the GitHub Pages workflow in `.github/workflows/static.yml`.
