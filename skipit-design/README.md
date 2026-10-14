# SkipIt mobile design prototype

A mobile-first guestlist experience for Mumbai nightclub promoters, door staff, and guests.

## Run locally

From this directory:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. No package installation or build step is needed.

## Review

- Use the experience selector to explore Promoter, Door staff, Guest, and Design system.
- Use the Screen and State selectors (or **Screens** on mobile) to inspect all states.
- Theme controls support System, Light, and Dark.
- Demo SMS code: `123456`.
- Reset demo restores the original sample data.

Includes 23 named screens, 94 review states, and a downloadable kit with 188 light/dark screen exports. The `assets/skipit-design-kit.zip` archive includes the screenshot gallery, design tokens, logo and home-screen icons, and implementation handoff.

## Prototype boundary

All guest records and settings are fictional and persist only in the current browser. SMS, online payments, and admission verification are simulations. The camera can show a real preview but does not decode or validate tickets. Demo pass links resolve only where their local records exist.

Production needs server-side authentication and role permissions, protected private pass tokens, transactional capacity and duplicate checks, atomic single-use admission, payment verification, and live synchronization. See the handoff inside the design kit. Do not use this prototype to operate a live event.

## Files

- `index.html`, `styles.css`, `app.js`: interactive app and design-system explorer.
- `manifest.webmanifest`, `sw.js`: home-screen installation and prototype shell caching.
- `assets/`: locally bundled fonts, reconstructed SVG logos, PNG icons, tokens, QR library, and design kit.

## Validation

Browser checks covered all 94 screen/state combinations in both themes and layouts at 360, 390, and 430px. Core payment-confirmation, group check-in, duplicate signup, repeat-scan, cancellation, staff-management, and export interactions were checked. Text token pairs meet WCAG AA contrast. Physical-device Safari and Android testing is still required before production.

## Third-party assets

Archivo and DM Sans use the SIL Open Font License; license texts are in `assets/`. The QR encoder is qrcode-generator 1.4.4 (MIT), with its license in `assets/QR-LICENSE.txt`.
