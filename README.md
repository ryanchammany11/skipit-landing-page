# SkipIt — Landing Page

Marketing site for **SkipIt**, a nightlife app for buying line-skip passes, booking tables, and pre-ordering drinks.

> Skip the line. Own the night.

## What's here

A single self-contained `index.html`. All CSS, JavaScript, and imagery (app screenshots encoded as WebP data URIs) ship inside that one file, so there is no build step and no asset directory to keep in sync.

## Structure

| Section | Purpose |
| --- | --- |
| Hero | Headline, app store buttons, home-screen preview |
| Venue ticker | Scrolling marquee of partner venues |
| The problem | The 40-minutes-outside pitch |
| What you can do | Passes, tables, wallet, pre-ordered drinks |
| How it works | Three steps, venue to door |
| Venue partners | Partner wordmarks + venue signup link |
| Social proof | Chat-bubble testimonials |
| Closing CTA | Download buttons |

## Details

- Type: Anton (display) and Poppins (body), loaded from Google Fonts
- Accent: `#FF2D6E` on a `#0B0A12` ground — committed dark theme
- Motion: neon scroll-tracking scribble drawn on a `<canvas>`-free inline SVG, flicker/pulse keyframes, and `IntersectionObserver` section reveals — all disabled under `prefers-reduced-motion`

## Running locally

No dependencies. Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
```

## Deploying

Static — no build command, no output directory. Vercel serves the repository root as-is.
