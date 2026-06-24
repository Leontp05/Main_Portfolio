# Leon Punnoose — WebGL Portfolio

A single-file WebGL portfolio with a 3D geological terrain that responds to scroll, mouse, and touch.

## Quick Start

1. Open `portfolio-leon-v8.html` in any modern browser (Chrome, Firefox, Safari, Edge)
2. That's it. No build step, no dependencies to install.

## Deploy

Upload the single HTML file to any static host:
- **GitHub Pages**: Push to a repo, enable Pages in Settings
- **Vercel**: `vercel --prod` in this directory
- **Netlify**: Drag and drop the file at app.netlify.com/drop

## Before You Ship

1. **Replace the canonical URL** — search for `https://leontp05.github.io/` and replace with your real deploy URL
2. **Generate an OG image** — take a 1200×630 screenshot of the hero, save as `og-image.png` in the same folder
3. **Test** — run through Google's [Rich Results Test](https://search.google.com/test/rich-results) to validate SEO

## Features

- **3D geological terrain** rendered with custom GLSL shaders (Three.js r160)
- **CatmullRom spline camera** with dolly, FOV animation, and idle orbit
- **GPU-driven particles** — zero CPU cost per frame
- **Full accessibility** — skip-link, ARIA, keyboard nav, reduced-motion, mute toggle
- **Mobile touch** — two-finger tap = shockwave, long-press = breath, perf scaling
- **SEO** — Open Graph, Twitter Card, Person JSON-LD, noscript fallback

## Browser Support

- Chrome/Edge 90+ (WebGL 2.0)
- Firefox 88+
- Safari 14+
- Mobile: iOS Safari 14+, Chrome Android 90+
- Falls back to static gradient if WebGL is unavailable

## Tech Stack

- Three.js r160 (ESM via importmap)
- GSAP 3.12 + ScrollTrigger
- Custom GLSL vertex + fragment shaders
- Web Audio API for ambient audio
- Zero build tools — just one HTML file
