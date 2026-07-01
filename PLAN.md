# Aditi ♥ Chethan — Interactive Wedding Invitation

## Brief (from client)
- **Cute & romantic**, "tap-and-reveal" experience: guests **scratch the card** to reveal the couple's names.
- **Sparkler / celebration reveal**, motion-graphics feel, on-trend (2026).
- Deliverable: **single self-contained interactive web page** (opens on any phone / WhatsApp link).
- Aesthetic: **Traditional temple romance** — marigold, gold, maroon, blush, Ganesha (venue is a Ganapati temple, Bengaluru).
- Single event: the wedding ceremony. **Date not finalized → graceful "Save the Date" placeholder.**

## People
- **Bride:** Aditi RS Singh — daughter of Ravi Shankar Singh & Soumya Ravi; sister Anchal RS Singh; + Muffin 🐾 (dog)
- **Groom:** TM Chethan Kumar — son of Murali T & Vani TM; sister TM Rakshitha

## Venue
SMBG – Sumukha Hall, Sri Shesha Maha Balamuri Ganapati Temple, 4th Main, 6th Cross,
Behind Ramanjaneya Gudda, Hanumantha Nagar, Bengaluru.
Map: https://maps.app.goo.gl/sfCVG7uoX561nidR7  → encoded as an inline SVG QR (self-contained).

## Experience flow
1. **Intro** — temple-red screen, A&C monogram, glowing "Tap to open".
2. **Curtain part** — gold panels slide away → scratch scene.
3. **Scratch card** — golden foil coating over the couple's names; scratch with a sparkle-trail brush; auto-reveals at ~55%.
4. **Celebration** — gold-foil shimmer names, confetti + sparkler burst, haptic buzz, "scroll down".
5. **Scroll invite** — Ganesha invocation + shloka → couple → both families (incl. Muffin) → Save the Date → venue + map + QR → blessing/close.

## Approach (why original art, not downloads)
Random web images = dead links + copyright risk for something sent to guests. Instead: **original inline SVG/CSS ornaments + a hand-written canvas particle engine** (petals, sparkler, confetti) + Google Fonts. Optional custom-generated motif art (Ganesha, marigold toran) embedded as base64 for a premium finish. Result = one file, works offline.

## Tech
- Single `index.html`, mobile-first, responsive.
- Scratch: canvas + Pointer Events, `destination-out`, DPR-aware, %-erased auto-complete, `touch-action:none`.
- Motion: rAF particle systems, IntersectionObserver scroll reveals, CSS gold shimmer (`background-clip:text`).
- Accessibility: `prefers-reduced-motion` fallback, **Tap-to-reveal** button, high-contrast QR.

## Status
- [x] Project scaffold + git
- [x] Self-contained QR (segno, ECC-H)
- [x] Trend research (6-agent workflow) → build spec (validated the design)
- [x] Build index.html (full interactive version)
- [x] Adopt spec refinements (Lora body font, tighter type, cleaner toran)
- [x] Fix: scene-dismiss handoff to scrolling invite
- [x] Fix: confetti hard-stop + tab-hidden clear
- [x] QA verified in browser — mobile (375) + desktop: intro → scratch → reveal
      → sparkler/confetti → all sections. QR, map link, families, Muffin 🐾 all correct.
- [ ] (Optional, pending client) Add real wedding date
- [ ] (Optional) Soft background music, custom-generated Ganesha art
