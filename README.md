# Bluechar — Coastal Carbon Infrastructure (Website V1)

A polished, lean first website that positions Bluechar as a coastal carbon
infrastructure platform — turning invasive seaweed into biochar, carbon-removal
value and practical municipal solutions. Now using the official Bluechar logo.

## What's included (V1 pages)
Home · Solution · For Municipalities · Carbon Removal · Partners · Careers · Contact

## How to view it
**Just open `index.html`** in this top folder, or double-click it. Every page
here is fully self-contained (CSS, JS and the logo are inlined) — no server
needed — so you can click through the whole site offline and share the files.

## Folder structure
```
bluechar-website/
├── index.html, solution.html, ...   ← self-contained site (view / share)
├── brand-assets/                     ← logo variants extracted from your doc
└── developer-source/                 ← clean, maintainable build to deploy
    ├── *.html + styles.css + main.js + assets/   ← shared-asset version to host
    └── partials/                     ← editable source + build.py
```

- **Top level** = standalone pages. Best for viewing.
- **developer-source/** = the same site with one shared `styles.css`, `main.js`
  and an `assets/` folder. This is the version to host; edit `styles.css` once
  and every page updates. Run `partials/build.py` to regenerate both variants.

## Logo & branding (from your profile document)
I pulled the official logo out of the "Bluechar Profile Job Description" doc and
turned it into web-ready assets. Sampled brand colors matched the brief almost
exactly — Ocean Blue `#016E9A` (≈ `#006F9F`) and Charcoal `#1F211D` (≈ `#1F2528`).

`brand-assets/` contains, on transparent backgrounds:
- `logo-full-color.png` / `logo-full-white.png` — full lockup with the
  "Sargassum Carbon Solutions" tagline (white version for dark backgrounds).
- `logo-color.png` / `logo-white.png` — primary lockup, mark + wordmark, no
  tagline (used in the site header).
- `mark-color.png` / `mark-white.png` — the wave-to-carbon-block mark alone.
- `favicon.png` — the mark at icon size.
- `logo-original-master.png` — the full-resolution original from your document.

Where each is used on the site:
- **Header** (navy): primary white lockup.
- **Footer** (charcoal): full white lockup with tagline.
- **Favicon / touch icon**: the mark.

A note on naming: the logo art carries the **Sargassum Carbon Solutions**
descriptor, while the website brief uses **Coastal Carbon Infrastructure** as the
primary descriptor. I kept the logo's own wording intact and used "Coastal Carbon
Infrastructure" as the positioning line in copy — both per the brief. Say the
word if you'd prefer one descriptor everywhere.

## Design system
- **Palette:** Navy `#06324A` (dominant) · Ocean Blue `#006F9F`/`#016E9A` ·
  Signal Teal `#00A7A5` (carbon-value accent) · Seafoam `#DFF3F4` · Sand
  `#F2E8D8` · Charcoal `#1F2528`. Green `#6B8F3E` reserved as a minimal accent.
- **Type:** Manrope ExtraBold (headlines) · Inter (body) · IBM Plex Mono
  (technical micro-labels, e.g. `where eligible`). Loaded via Google Fonts.
- The hero keeps an animated wave→particles→carbon-block motif that echoes the
  logo concept; everything else stays disciplined.

## Wording discipline (built in)
Carbon claims use careful language throughout — "where eligible", "subject to
technical and certification requirements", "designed for verification". A footer
disclaimer states credits are a designed pathway, not guaranteed, and that
pilot/target markets do not imply signed contracts.

## Functional notes
- Responsive with a mobile menu; sticky header; scroll-reveal (respects
  reduced-motion); visible keyboard focus; cookie notice.
- SEO: per-page titles, meta descriptions and Open Graph tags.
- The **Contact form** is wired for UX (validation + routed confirmation by
  inquiry type) but has **no backend yet** — connect to email/CRM on deploy and
  set routing addresses. The "Request the overview" link needs the profile PDF.
- No browser-storage APIs are used.

## Suggested V2 (per brief)
Technology page · detailed Projects (Cádiz pilot, Florida/Gulf reference,
Caribbean) · Insights/News · Spanish version · investor materials · carbon-buyer
portal · interactive map.
```
```
# Bluechar
