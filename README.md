# MILAURE — static site

Ready-to-deploy static files. No build step required.

## Structure
- `index.html` — home (Water / element selector, sneak strip, showcase, launch)
- `About.dc.html` — about page
- `Elements.dc.html` — elements page
- `support.js` — runtime (must sit next to the HTML files)
- `assets/` — images, video, logos

## Deploy
Upload the entire folder to any static host (Netlify, Vercel, GitHub Pages, S3, nginx).
`index.html` is the entry point. Everything is served as plain static files — open
`index.html` over HTTP (not file://) so the videos and fonts load.

Quick local check:
```
npx serve .
```
