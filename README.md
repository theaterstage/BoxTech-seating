# BoxTech seating — static GitHub Pages mirror

مرآة ثابتة لموقع **بوكس تيك** (كراسي ومسارح وملاعب وقاعات).

Static mirror of https://playground-grandstand.grok.me built for the `/BoxTech-seating/` sub-path.

**Live:** https://theaterstage.github.io/BoxTech-seating/

## Contents

- Arabic (`/ar/…`) and English (`/en/…`) HTML routes from the source sitemap (~1226 pages), each as `…/index.html`
- `/assets/*` (JS/CSS), `/media/*` (product & project images), favicon, OG images, `.nojekyll`, `404.html`
- TanStack Router `basepath` set to `/BoxTech-seating` so client navigation works under GitHub Pages

## Gaps / known limits

- This is a **static** export: any live server APIs, quote/form backends, or WebSocket features from the original host will not run here.
- Google Fonts still load from `fonts.googleapis.com` (requires network).
- The original grok.app-builder extension script was removed from HTML.

## Fix notes (2026-10-05)

- Restored 20 missing Vite route chunks under `assets/` (products, systems, journal, news, …).
- Corrected Vite asset URL helper `Mv` so dynamic imports resolve under `/BoxTech-seating/` (was `/assets/…` at site root).
- Added `media/plates/*.svg` (~1600) referenced by journal/news/atlas pages.

## Source

- Origin: https://playground-grandstand.grok.me (`/` → `/ar`)
- Repo description: BoxTech seating / playground-grandstand static GitHub Pages mirror
