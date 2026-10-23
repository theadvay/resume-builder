# Resume Builder

> A free, fully responsive online resume builder with a live preview and one-click PDF export. No sign-up, no watermark, no server — everything runs in your browser.

**Live demo:** https://theadvay.github.io/resume-builder/

![Resume Builder — free resume builder with live preview](og-image.png)

---

## What it is

Resume Builder is a single-page web app that helps you build a clean, professional, print-ready A4 resume. You type your details into the editor on the left, the live preview on the right updates instantly, and when you are happy you export it as a PDF straight from the browser.

It is built with plain HTML, CSS and JavaScript — no frameworks, no build step, no dependencies. Drop it on any static host and it just works.

## Features

- **Live preview** — every keystroke is reflected on an A4 sheet in real time.
- **20 templates** — Classic, Modern, Minimal, Elegant, Compact, Bold, Timeline, Banner, Right Rail, Two Column, Academic, Creative, Corporate, Mono, Infographic, Swiss, Photo Left, Gradient, Dark Sidebar and Spotlight.
- **Profile photo upload** — optional, resized in the browser before it is stored.
- **Eight accent colours** and **three font styles** (Sans, Serif, Mono).
- **One-click PDF export** — a print stylesheet strips away the UI and prints only the resume.
- **Auto-save** — your work is stored in the browser's `localStorage`, so you can close the tab and come back later.
- **100% private** — nothing is ever uploaded; your data never leaves your device.
- **Fully responsive** — a two-pane workspace on desktop and tablet, and a clean Edit / Preview switch on phones.
- **Accessible** — semantic landmarks, a skip link, visible focus states, ARIA labels and `prefers-reduced-motion` support.
- **SEO ready** — meta tags, Open Graph, Twitter cards, canonical URL, JSON-LD structured data (`WebApplication` + `FAQPage`), `robots.txt` and an XML sitemap.

## How to use

1. Open the site (or `index.html`) in any modern browser.
2. Fill in your details — name, contact, summary, experience, education, projects, skills and certifications.
3. Pick one of the 20 templates, an accent colour and a font — and upload a photo if you like.
4. Click **Save as PDF**, then choose **Save as PDF** as the print destination.

> **Tip:** Keep it to one or two pages, start every bullet with an action verb, and quantify results wherever you can. Sections you leave empty never appear in the resume.

## Run it locally

No installation or build step is required. Because it is a static site, any of these work:

```bash
# Clone
git clone https://github.com/theadvay/resume-builder.git
cd resume-builder

# Open directly…
open index.html          # macOS
xdg-open index.html      # Linux

# …or serve it over HTTP (recommended, so the manifest and icons load)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

The site is plain static files, so it deploys anywhere:

- **GitHub Pages** — push to `main`, then enable Pages with the source set to the root of the `main` branch.
- **Netlify / Vercel / Cloudflare Pages** — connect the repo; no build command, publish directory is the project root.

## Project structure

```
resume-builder/
├── index.html            # The whole app — markup, styles and logic
├── manifest.webmanifest  # PWA metadata
├── favicon.svg           # Vector favicon
├── icon-192.png          # PWA icon
├── icon-512.png          # PWA icon
├── apple-touch-icon.png  # iOS home-screen icon
├── og-image.png          # Social share image (1200×630)
├── robots.txt            # Crawler rules + sitemap reference
├── sitemap.xml           # XML sitemap
├── LICENSE               # MIT
└── README.md
```

## Tech

Vanilla **HTML5**, **CSS3** (custom properties, Grid, Flexbox, container-free full-screen layout) and **JavaScript** (ES5-compatible, no dependencies). Fonts are [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans), [Azeret Mono](https://fonts.google.com/specimen/Azeret+Mono) and [Source Serif 4](https://fonts.google.com/specimen/Source+Serif+4) via Google Fonts, with system fallbacks.

## Browser support

Latest versions of Chrome, Edge, Firefox and Safari, on desktop and mobile. The layout adapts from small phones up to large desktop screens.

## License

Released under the [MIT License](LICENSE).

## Author

Built by **Advay** ([@theadvay](https://github.com/theadvay)).

If this saved you some time, a ⭐ on the repo is always appreciated.
