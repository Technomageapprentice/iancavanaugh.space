# iancavanaugh.space

**Status:** Active — in progress  
**Last updated:** 2026-06-29  
**Hosting:** BlueHost (basic) — static HTML, WordPress removed  
**Repo:** https://github.com/Technomageapprentice/iancavanaugh.space

---

## Purpose

A professional anchor on the web. Not a social profile — a destination.  
Communicates who I am, what I've built, and what I'm thinking — without feeling like a resume PDF.

---

## Brand Direction

- Tone: Competent, direct, slightly unconventional. Not corporate. Not casual.
- Audience: Technical hiring managers, potential collaborators, curious people who Google me.
- Visual: Dark industrial palette (black + gold), IBM Plex Mono/Sans, Bebas Neue. Pittsburgh-coded but reads as industrial heritage, not sports branding. Blue accent (`#4a9eff`) to be promoted as a secondary color.
- No buzzwords.

---

## Homepage Tagline

**Chosen:** *Systems over spreadsheets.*  
**Subtext:** *Sales engineer turned systems designer — I build the tools that make complex workflows predictable.*

> Needs refinement once additional context is provided: industry framing, cert timeline, preferred self-descriptor.

---

## About Page — COMPLETE

`about.html` written and live. See file for full text.

**Credentials listed:** B.S. Naval Architecture & Marine Engineering (Webb Institute), EIT, Eagle Scout, AWS SAA-C03 (in progress), 3rd Dan Black Belt (Tang Soo Do), Brown Belt (BJJ).

**Framing:** Naval Architecture positioned as the origin of the integrator identity — cross-disciplinary systems integration that transfers across industries (maritime → HVAC → software). Industry-agnostic by design.

---

## Core Sections

| Section | Status | Notes |
|---|---|---|
| Home / Landing | **Live** | `index.html` reviewed in browser, GoatCounter wired |
| About | **Live** | `about.html` written and uploaded |
| Portfolio | Not started | 3 case studies — see Portfolio Candidates |
| Blog | Not started | Quarterly cadence, not a feed |
| Contact | Not started | Email + social links |

---

## Professional Links

- [x] GitHub — https://github.com/Technomageapprentice
- [x] LinkedIn — https://www.linkedin.com/in/icavanaugh/
- [ ] Email (obfuscated or contact form — decide when building Contact page)

---

## Portfolio Candidates

Three pieces, three different stories — ordered by strength.

### 1. On-Screen Takeoff Tool
**Safe to show in full.** Browser-based measurement tool for HVAC floor plans. Custom canvas engine, AWS Cognito + DynamoDB + S3. No proprietary data.  
**Show:** live demo link, architecture diagram, before/after workflow.

### 2. Estimating Pipeline
**Show interfaces + architecture; protect pricing logic.** Three-layer pipeline (ingestion → pricing → proposal dashboard). Coverage: 14% → 56%. Stack: Python, SQLite, PowerShell, AWS, HTML/JS.  
**Do not publish:** pricing-ruleset.yaml, parts.db, real job JSON files (contain customer names).  
**Show:** scope-builder + Proposal dashboard with anonymized data, architecture diagram, coverage metrics.

### 3. VBA → Python Modernization
**Written case study, no live demo.** Maintained production VBA for years, led migration to Python. QEX translator is the concrete example. Strong differentiator for SA targets in legacy-heavy companies.

---

## Analytics

**GoatCounter** — https://iancavanaugh.goatcounter.com  
Privacy-first, no cookie banner required. Script wired into `index.html` and `about.html`. Add to each new page as built.

---

## AI Parseability

Built in from day one — no plugin discipline needed.

- Semantic HTML with proper heading hierarchy (already in `index.html`)
- JSON-LD `Person` on homepage; add `Article` to blog posts
- `llms.txt` in site root — written and uploaded
- `sitemap.xml` kept current
- Clean `<meta>` descriptions — written as sentences, not keyword lists
- No critical content behind JavaScript

---

## To-Do

- [x] Define portfolio pieces
- [x] Draft homepage tagline + About bio
- [x] Decide platform → build from scratch, static HTML on BlueHost
- [x] Draft homepage HTML → `index.html`
- [x] Confirm social links → GitHub + LinkedIn wired into `index.html`
- [x] Open `index.html` in browser and review
- [x] Finalize About bio — needs personal context (coming next session)
- [x] Disable WordPress on BlueHost, confirm static file serving
- [x] Screenshot current WordPress site before teardown
- [x] Write `llms.txt`
- [x] Build: About page
- [ ] Build: Portfolio, Contact pages
- [ ] Promote blue accent (`#4a9eff`) as secondary color across site
- [ ] Outline first blog post (title + 3 bullets — don't write it yet)

---

## Log

- **2026-06-29** — About page written and live (`about.html`). WordPress removed from BlueHost; static file serving confirmed. `llms.txt` written and uploaded. GoatCounter analytics wired into `index.html` and `about.html`. Naval Architecture framed as origin of integrator identity. Credentials finalized: Webb BSNAME, EIT, Eagle Scout, AWS SAA-C03 (in progress), TSD 3rd Dan, BJJ brown belt.
- **2026-05-30** — Document created; moved to `20_Forge/Website/`. Platform decided: static HTML. Homepage drafted (`index.html`). Portfolio candidates defined. About bio drafted — awaiting personal context. Social links confirmed. Color scheme: Pittsburgh industrial palette retained; blue accent to be promoted.
