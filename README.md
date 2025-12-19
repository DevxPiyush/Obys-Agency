# Obys Agency — Interactive Landing Page

Recreation of the award‑winning Obys Agency site as a single‑page experience. It blends smooth scrolling, video reveals, gooey image transitions, custom cursor interactions, and a loader sequence using modern front‑end animation libraries.

## What’s inside
- Custom hero, projects gallery, about, marquee, and footer sections styled in [style.css](style.css)
- Loader/countdown intro and text animations driven by GSAP timelines in [script.js](script.js)
- Smooth scrolling via Locomotive Scroll + ScrollTrigger proxy setup
- Shery.js image gooey effect and custom mouse follower with magnetic nav hover
- Video hero with play/pause cursor toggle and inline showreel source
- Hosted assets for imagery, SVGs, and local web fonts under `assets/` and `fonts/`

## Tech stack
- HTML/CSS/JS (no build step)
- GSAP + ScrollTrigger
- Locomotive Scroll
- Shery.js (+ three.js/controlkit dependencies)
- Textillate.js + Lettering.js + animate.css
- Remix Icons

## Quick start
1) Clone/download the repo.
2) Open `index.html` directly in a modern browser, or serve locally (recommended for smooth scrolling):

```bash
npx serve .
# or
python -m http.server 5173
```

Then visit the printed localhost URL (e.g., `http://localhost:5173`).

## Notes
- External CDNs are referenced in `index.html`; an internet connection is required for dependencies.
- Custom fonts are loaded from `fonts/` and expect the provided file names in [style.css](style.css).
- Cursor hiding (`cursor: none`) and Shery’s follower are enabled globally; disable in CSS if needed for accessibility testing.
- Video autoplay is click‑triggered; toggle via the orange circular cursor inside the video frame.

## Tweaks
- Update image sources in `assets/` and the `#page3` gallery markup to swap projects.
- Adjust animation timings inside `LoadingAnimation()` and `cursoranimation()` in [script.js](script.js).
- Edit the smooth scroll behavior in `locomotiveanimation()` by changing the `smooth` option or scroll container.
