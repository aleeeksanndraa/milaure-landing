# MILAURE — Woman as Elements

Brand-awareness landing page for **MILAURE**. A welcome "door" intro opens (click) into an editorial hero with an interactive element selector — **Water · Fire · Air · Earth** — that re-themes the Story, Mood and First Glimpse sections. Water is the first drop; the other elements show a *coming soon* state.

## Run locally

It's a static site — serve the folder with any static server (don't open via `file://`, the video and runtime need HTTP):

```bash
# Python
python3 -m http.server 8080

# or Node
npx serve .
```

Then open http://localhost:8080

## Deploy

Drop the whole folder onto any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages). No build step.

- **GitHub Pages:** push to a repo and enable Pages on the branch root. `index.html` is the entry point.

## Structure

```
index.html      — the page (markup + logic)
support.js      — lightweight runtime that renders the component
assets/
  hero.mp4      — hero background video
  door.mp4      — welcome "door" intro video
```

## Editing

- **Copy & per-element content** live in the `ELEMENTS` object inside the `<script data-dc-script>` block in `index.html`.
- **Palette / theming** are CSS custom properties in the `:root` and `html[data-element="…"]` rules at the top of the same file.
- Replace the placeholder mood/glimpse tiles with real campaign imagery when assets are ready.

© 2026 MILAURE — Woman as Elements
