# 💍 Aditi & Chethan — Interactive Engagement Invitation

A single, self-contained web invitation whose centrepiece is an **illustrated Indian
couple with a ring-ceremony animation** — Chethan gently places the ring on Aditi's
finger, with a sparkle + heart celebration. Everything lives in one file: **`index.html`**.
No hosted images, no plugins — original SVG/CSS art + a hand-written animation engine.

- **Engagement · Sunday, 12 July 2026 · Bengaluru**
- Live link: **https://ganeshphutane-g.github.io/aditi-and-chethan-invite/**

## How guests experience it
1. **Tap to begin** — warm-gold "A & C" cover.
2. **Scratch the card** — a golden foil card covers the scene; scratching it reveals the
   couple's **engagement video, which plays on loop** (the real ring-ceremony clip in the
   golden floral arch with candles & bokeh) with a **sparkle + floating-heart** burst, and
   the names "Aditi & Chethan" appear. A **"Replay"** button restarts it.
   The video is muted + `playsinline` (autoplays after the scratch on real devices; a
   play-button fallback covers reduced-motion / blocked-autoplay). It's compressed to
   ~1.5 MB (`assets/hero.mp4`, 1440-wide H.264, faststart) with `assets/hero-poster.jpg`
   as the instant-paint poster.
3. **Scroll** through: Ganesha blessing → the couple → both families (incl. Muffin 🐾)
   → Save the Date (12 July 2026) → venue + Google Maps + QR → closing blessing.

The whole palette is a **warm candlelit gold / amber / blush** theme matched to the
reference video. Fully responsive (verified 360 / 375 / 1280px), text never crops (all text
is real HTML, never baked into the artwork), and a **reduced-motion** mode shows the
finished "ring placed" tableau (no scratch required) for accessibility.

## How to share it
- **Best — the link:** share **https://ganeshphutane-g.github.io/aditi-and-chethan-invite/**
  on WhatsApp / SMS. Works on any phone or laptop, online or offline.
- **Or send the file:** WhatsApp/email `index.html`; tapping it opens in the browser.

## Editing details
- **Date / time:** search `12 · 07 · 2026` and `Sunday · 12 July 2026` in `index.html`.
- **Names / families / venue:** search the text (e.g. `Ravi Shankar`) and edit in place.
- **Map + QR:** both point to `maps.app.goo.gl/sfCVG7uoX561nidR7`.
- **Animation timing:** in the script, `var hold=320, dur=1600;` controls the ring reach.

## A note on the artwork
The couple, arch, garland, lights, sparkles and hearts are **original vector illustrations
+ CSS/JS animation** (safe to share, works offline). We deliberately avoided scraping
third-party "free" illustration packs (licensing risk + not riggable for the ring motion).

## Files
- `index.html` — the engagement invitation (this is the whole thing).
- `wedding.html` — an earlier *wedding*-framed version (scratch-to-reveal), kept for reference.
- `assets/qr-map.svg` — the source QR (already inlined into the pages).
- `PLAN.md` — design plan & decisions.
