# 💛 Aditi & Chethan — Interactive Wedding Invitation

A single, self-contained web invitation with a **scratch-to-reveal** centrepiece,
sparkler + confetti celebration, and an elegant temple-romance design.
Everything lives in one file: **`index.html`**. No internet-hosted images, no plugins.

## How guests experience it
1. **Tap to open** — golden curtains part.
2. **Scratch the card** (finger on phone / mouse on laptop) to reveal **Aditi & Chethan**.
3. **Sparkler + confetti** celebration 🎉 with a gentle phone buzz.
4. **Scroll** through: Ganesha blessing → the couple → both families (incl. Muffin 🐾)
   → Save the Date → venue with Google Maps button + scannable QR → closing blessing.

A **"tap to reveal"** button and a reduced-motion mode are built in, so it works for
everyone (older phones, accessibility settings, guests who don't realise it's scratchable).

## How to share it
Pick whichever is easiest for you:

- **Easiest — send the file:** WhatsApp/email the `index.html` file. Tapping it opens
  it in the phone's browser. Works fully offline.
- **Best — send a link:** host it free and share the URL (nicer on WhatsApp — shows a preview).
  Drag-and-drop `index.html` onto any of these:
  - Netlify Drop — https://app.netlify.com/drop
  - Cloudflare Pages / GitHub Pages / Vercel
  Then share the link (e.g. `https://aditi-chethan.netlify.app`).

## ✍️ To add the wedding date once it's fixed
Open `index.html` in any text editor, find **"Save the Date"** (there's a comment right
above it), and edit two lines:
```html
<div class="big foil">24 · 08 · 2026</div>
<div class="soon">Sunday · Muhurat at 10:30 AM</div>
```
Save the file. Done — nothing else changes.

## Editing other details
- **Names / families / venue:** search the file for the text (e.g. `Ravi Shankar`) and edit in place.
- **Map + QR:** both point to the venue link `maps.app.goo.gl/sfCVG7uoX561nidR7`.
  To change, edit the `href` on the "Open in Google Maps" button and regenerate the QR
  (`assets/qr-map.svg` was made with the `segno` Python library).

## Files
- `index.html` — the invitation (this is the whole thing).
- `assets/qr-map.svg` — the source QR (already inlined into `index.html`).
- `PLAN.md` — design plan & decisions.
