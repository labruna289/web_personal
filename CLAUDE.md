# Claude Session Memory — Daniel Rot CV Website

## Project
Single-page CV website for **Daniel Rot**, a SAP BW/4HANA · ABAP · SAC · Datasphere consultant based in Barcelona, Spain.

Deployed on **Cloudflare Workers** (static assets) via `wrangler.jsonc`.
Active development branch: `claude/build-cv-website-BfzUD`

---

## Owner / Personal Info
- **Name:** Daniel Rot
- **Phone / WhatsApp:** +34 663 415 069 → `https://wa.me/34663415069`
- **Email:** danielrot@gmail.com
- **LinkedIn:** linkedin.com/in/daniel-rot-43ba9814
- **Location:** Barcelona, Spain · EU Citizen (Slovenia) · NIE (Spain)

---

## Tech Stack
- Pure HTML/CSS/JS — single file `index.html`, no frameworks, no external dependencies
- `profile.png` — profile photo in repo root
- `wrangler.jsonc` — Cloudflare Workers static assets config

---

## Site Structure (sections)
| # | ID | Content |
|---|---|---|
| Hero | `#hero` | Photo, name, title, icon links (WhatsApp/envelope/LinkedIn), location, skill tags |
| 01 | `#experience` | 8-role vertical timeline (Nov 2009 – Jan 2026) |
| 02 | `#skills` | 6 skill cards grid |
| 03 | `#education` | UBA degree + 2 SAP certifications |
| 04 | `#languages` | Spanish / English / Slovenian / Portuguese |
| 05 | `#contact` | mailto form + WhatsApp / email / LinkedIn quick links |

---

## Design System
- **Theme:** Dark (`--bg: #0f1117`)
- **Accent:** Blue (`--accent: #3b82f6`) / Indigo (`--accent2: #6366f1`)
- **Font:** Segoe UI / system-ui
- **Nav:** Sticky, blurred, centered, `flex-wrap` on mobile
- **Hero avatar:** 120px circle, `profile.png`, `object-fit: cover; object-position: center top`

---

## Behaviours & UX Rules
- **Home nav link** hides (opacity + width: 0) while the hero section is in view; reappears on scroll past it
- **Mobile hero:** column layout, avatar on top, everything centered (`text-align: center`)
- **Mobile nav:** `justify-content: center` + `flex-wrap: wrap`
- **Contact form:** uses `mailto:` to pre-fill an email to danielrot@gmail.com — no backend needed

---

## Work Experience (for reference)
1. Freelance BW4/HANA · Datasphere · SAC – Banking | Barcelona | Jan 2024 – Jan 2026
2. Freelance BW4/HANA · ABAP – NTT Data | Barcelona | Mar 2021 – Dec 2023
3. SAP ABAP/BW/BPC · S/4HANA – Minsait | Barcelona | May 2019 – Jan 2021
4. SAP ABAP/BW/BPC · S/4HANA – Quales Group | Buenos Aires | Sep 2017 – Apr 2019
5. SAP APO/ABAP/BW/BI/SCM – MSP Consulting | Buenos Aires | Mar 2014 – Feb 2016
6. BW/ABAP – IBM | Buenos Aires | Nov 2013 – Feb 2014
7. BW/ABAP – Neoris | Buenos Aires | Nov 2012 – Nov 2013
8. ABAP/BW – Accenture | Buenos Aires | Nov 2009 – Oct 2012

---

## Certifications
- SAP Certified Application Associate – SAP Analytics Cloud (Mar 2020, no expiry)
- SAP Certified Application Associate – Reporting/Modeling & Data Acquisition with SAP BW/4HANA (Mar 2020, no expiry)

---

## Languages
- Spanish (native) · English (advanced) · Slovenian (advanced) · Portuguese (basic)

---

## Git Workflow
- Always develop on `claude/build-cv-website-BfzUD`
- Push with: `git push -u origin claude/build-cv-website-BfzUD`
- Do NOT create a pull request unless the user explicitly asks
