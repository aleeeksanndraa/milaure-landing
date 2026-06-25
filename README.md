# MILAURE — Woman as Elements

Brand-awareness launch site for **MILAURE**. A welcome "door" intro opens (click) into an editorial hero with an interactive element selector — **Water · Fire · Air · Earth** — that re-themes the story, mood and first-glimpse sections (accent, gradient and hero glow shift per element). Water is the first drop; the others show a *coming soon* state.

## Pages

- `index.html` — home (door intro, hero element selector, story, mood, first glimpse, launch sign-up, footer)
- `Elements.dc.html` — the four elements, one section each
- `About.dc.html` — brand statement and the four elements

## Run locally

Static site — serve the folder over HTTP (don't open via `file://`, the video and runtime need a server):

```bash
python3 -m http.server 8080   # then open http://localhost:8080
# or: npx serve .
```

## Deploy

Drop the folder onto any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages). No build step. `index.html` is the entry point.

## Structure

```
index.html            — home page
Elements.dc.html      — Elements page
About.dc.html         — About page
support.js            — lightweight runtime that renders the components
assets/
  hero.mp4            — hero background video
  door.mp4            — welcome "door" intro video
  favicon.png         — shell favicon
  apple-touch-icon.png
```

## Editing

- **Copy & per-element content** live in the `ELEMENTS` object inside the `<script data-dc-script>` block in `index.html`.
- **Palette / element theming** are CSS custom properties in `:root` and the `html[data-element="…"]` rules at the top of each file.
- Replace the placeholder image/mood panels with real campaign photography when assets are ready.

© 2026 MILAURE — Woman as Elements
