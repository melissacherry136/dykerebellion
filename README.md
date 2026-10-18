# Dyke Rebellion™

Website for **Dyke Rebellion™** — a queer women & nonbinary motorcycle club in the Bay Area, California. Est. 2026.

Live site: https://dykerebellion.com

## How it works

This repo is a single, self-contained static site. `index.html` has all styles, scripts, and the club patch (embedded) inlined — no build step required.

- **`index.html`** — the whole site (hero, buttons, ride calendar, Merch, Founders, contact).
- **`logo.png`** — transparent club patch, used for social/link-preview images.
- **`og-image.jpg`** — 1200×630 link-preview image (Facebook, iMessage, etc.).
- **`favicon.ico`, `favicon-48.png`, `icon-192.png`, `apple-touch-icon.png`** — browser/search-result icons.
- **`robots.txt`, `sitemap.xml`** — search-engine crawling. Bump `<lastmod>` in the sitemap when the page changes.
- **`netlify.toml`** — Netlify deploy config (publishes the repo root).

The Rides section embeds the public **"Dyke Rebellion Rides & Events"** Google Calendar, so new rides added in Google Calendar appear on the site automatically.

## Deploying

Netlify is connected to this repo for continuous deployment. **Any commit pushed to the `main` branch is built and published to https://www.dykerebellion.com automatically** — usually within a few seconds. There is no build command; Netlify just serves the files.

## Editing

Edit `index.html` and commit to `main`. That's it — Netlify does the rest.

To work locally, clone this repo (for example with GitHub Desktop), edit, then commit & push. Every push auto-deploys.
