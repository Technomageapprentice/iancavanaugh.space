# iancavanaugh.space

**Status:** Active — in progress  
**Last updated:** 2026-05-30  
**Hosting:** BlueHost (basic) — static HTML, WordPress removed  
**Repo:** https://github.com/Technomageapprentice/Obsidian

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

## About Page — DRAFT

> **Needs context to finalize:** years in current role, company type, certifications in progress, pre-SE background, outside interests (martial arts, travel, urbanism — 1–2 sentences max).

---

Ian Cavanaugh is a sales engineer and systems designer working in industrial manufacturing. His career sits at the intersection of technical sales and software architecture — a position he's occupied long enough to understand why the gap between those two disciplines keeps creating problems.

His day-to-day work involves translating customer requirements into fabricated product. What he's built around that work is a different story: an end-to-end estimating pipeline that replaced a manual, spreadsheet-driven process with a three-layer automation system — takeoff ingestion, pricing logic, and proposal generation — running on AWS with a Python core and browser-based interfaces. The pipeline moved job coverage from 14% to 56% within a single quarter. The estimators who use it have moved from doing the math to checking the math.

That pattern — finding the workflow that's held together with Word documents and institutional memory, then designing the system that should replace it — is the work he finds most interesting.

He's been writing code long enough to have VBA scars. He's building toward cloud architecture certifications and a role where the scope is infrastructure rather than individual tools. **[ADD: cert timeline + target role framing.]**

Outside of work, **[ADD: 1–2 sentences — martial arts, travel, urbanism. Signal there's a person here.]**

This site is where he keeps the work that's worth showing.

---

## Core Sections

| Section | Status | Notes |
|---|---|---|
| Home / Landing | **Draft** | `index.html` written — tagline, 3 portfolio cards, about teaser, footer |
| About | Not started | Needs personal context (see draft above) |
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

## AI Parseability

Built in from day one — no plugin discipline needed.

- Semantic HTML with proper heading hierarchy (already in `index.html`)
- JSON-LD `Person` on homepage; add `Article` to blog posts
- `llms.txt` in site root — plain-text summary for LLM crawlers
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
- [ ] Open `index.html` in browser and review
- [ ] Finalize About bio — needs personal context (coming next session)
- [ ] Disable WordPress on BlueHost, confirm static file serving
- [ ] Screenshot current WordPress site before teardown
- [ ] Write `llms.txt`
- [ ] Build: About, Portfolio, Contact pages
- [ ] Promote blue accent (`#4a9eff`) as secondary color across site
- [ ] Outline first blog post (title + 3 bullets — don't write it yet)

---

## Log

- **2026-05-30** — Document created; moved to `20_Forge/Website/`. Platform decided: static HTML. Homepage drafted (`index.html`). Portfolio candidates defined. About bio drafted — awaiting personal context. Social links confirmed. Color scheme: Pittsburgh industrial palette retained; blue accent to be promoted.
