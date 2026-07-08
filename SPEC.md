# Village Oaks Website — Spec

Static one-page marketing site for **Village Oaks Apartment Homes** (TCVO LLC), 9920 Forest Lane, Dallas TX. Built/maintained via Claude (no separate handoff needed — it's a simple one-page form site).

## Hosting & deploy
- **GitHub Pages** · repo `ww7085w/village-oaks` · branch `main` (root) · `CNAME` → **villageoaksdallas.com**
- HTTPS via Let's Encrypt (Enforce HTTPS on). Deploy = **push to `main` → live in ~1 min.**
- Migrated off the old WordPress/Hostinger site on 2026-05-31.

## Stack
Vanilla HTML/CSS/JS, no build step. Files: `index.html`, `privacy-policy.html`, `terms-of-service.html`, `images/`, `CNAME`.

## Page structure (index.html)
Header (top utility bar + nav + logo) · Hero · Stat bar · About · Amenities · Floor Plans · Gallery (15 photos) · Neighborhood · Residents (AppFolio links) · **Schedule a Tour (GHL form)** · Footer.

## Lead form — the key integration
- The "Schedule a Tour" section embeds the **GHL hosted form "Tour Submission Form"** (id `lUZeU6QJV2ra91Wh9seH`) inline.
- Collects name / phone / email + move-in date, floor plan, budget, tour interest, message; **two SMS-consent checkboxes** (transactional + promotional).
- **Full lead-capture / GHL workflow / A2P / consent detail lives in the Combined Marketing Plan**, not here: `.All Marketing\EG-Combined-Marketing-Plan-V3.3.md` (Village Oaks sections + "A2P 10DLC — STANDARD TEMPLATE").

## AppFolio
Pay Rent / resident portal → `https://tcvo.appfolio.com/connect`.

## Brand
Colors: charcoal `#26323A`, terracotta `#B9744F`, cream `#F7F4EF`. Fonts: Playfair Display + Inter. Logo: `images/vo-logo.png`.

## To edit
Edit the HTML/CSS locally → commit → push to `main` → GitHub Pages redeploys (~1 min). Legal pages are `privacy-policy.html` / `terms-of-service.html`.

_Local doc — not committed to the public repo (it references internal paths). Last updated 2026-06-01._
