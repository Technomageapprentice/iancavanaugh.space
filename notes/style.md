# Notes Style Guide

**Voice, structure, and principles for iancavanaugh.space/notes**

---

## What This Is

Not a blog. A personal wiki, built on the belief that most writing worth keeping is worth revising rather than superseding.

A blog is a stream: posts go up, get pushed down the feed by newer posts, and are effectively archived the day after publication. A wiki is a network: notes get better over time, link densely to each other, and don't expire. This site is the second kind. There's no reverse-chronological feed as primary navigation — notes are entered through links, an index, or backlinks, not by scrolling.

Practically, this means:

- **Notes get revised in place**, not superseded by a new post that says "update." See Revision History below.
- **Links carry weight.** A dense, well-linked note is worth more than a chronological archive of loosely related ones. See Links & Previews below.
- **A note can publish rough and sharpen later.** The revision history is the record of that sharpening — it doesn't need to hide.
- **Evergreen over topical.** Prefer notes that stay true in five years over ones pegged to this week's news cycle.

---

## Inspirations

| Site | What to steal |
|---|---|
| [Gwern](https://gwern.net) | The whole model: wiki over blog, popup link previews, information density, concept linking, trust the reader to go deeper |
| [Experimental History](https://www.experimental-history.com) — Adam Mastroianni | Personal flair, self-deprecating humor, tooltip footnotes, direct address |
| [SatPost](https://www.satpost.com) — Trung Phan | Research depth, relatable framing of complex ideas |

---

## Voice

Governed by `00_Citadel/Voice-Tone.md` — Section I for the core traits (Confident, Humble, etc. with their anti-patterns) and Section III for the AI-tell/hedge problem. Notes get the full Core + personal register (see Voice-Tone Section V, "Website — Notes/wiki"); that's the one thing specific to this surface: **notes are the personal register of the site. The portfolio is the resume. Notes are the person.**

First person throughout. The do/don't examples below are the validated instance set referenced from Voice-Tone Section III — kept here since they're notes-specific, but the underlying rule (avoid hedge/preamble language, prefer one concrete detail) lives there, not here.

**What this sounds like:**
- "I got this wrong for two years before I understood why."
- "The estimators stopped doing the math and started checking it."
- A dry footnote the main text doesn't need but is better for having.

**What this doesn't sound like:**
- "In this post, I'll explore..."
- "It's important to note that..."
- Anything that would appear on a LinkedIn thought leadership carousel.

---

## Structure

This applies to **essay-type notes** — the ones developing a single argument. Reference notes, running lists, and short evergreen definitions don't need this shape; don't force it on them.

1. **Epigraph** — required (see below)
2. **Hook** — a scene, a question, or a contradiction. No thesis yet.
3. **Thesis** — stated plainly, once the reader is oriented.
4. **Development** — argument, evidence, example. Footnotes live here.
5. **Concrete example** — own work where applicable. Don't assert the principle; show where it ran.
6. **Close** — actionable or provocative. Short. No summary paragraph.
7. **Sign-off**

**Target length:** 800–1,500 words for essay-type notes. Long enough to develop an idea, short enough to respect the reader's time. Reference notes have no target length — as long as they need to be, no longer.

---

## Epigraphs

Required for essay-type notes. One per note, before the body.

**The job:** Intellectual signaling that doesn't explain itself. The connection to the thesis becomes clear during or after reading — not before. The epigraph is the oblique angle.

**The model:** Watership Down's chapter epigraphs — quotes from a parallel world that illuminate this one without annotating it. The invisible chapter architecture of Ulysses — structure doing work the reader never sees. The epigraph rewards the reader who recognizes the source. It doesn't punish the one who doesn't.

**The test:** After reading the note, does the epigraph feel inevitable? If it still feels random, swap it. When it works, it's the best sentence on the page.

**Publishing gate:** No great epigraph, no publish. If the note is done and the epigraph isn't landing, the note isn't done. The difficulty is the point — an epigraph that won't come is a signal the thesis isn't sharp enough yet.

**Draw from:**
- Engineering and systems literature (Deming, Reason, Shingo, Norman)
- Philosophy, political theory, history of science
- Fiction and poetry — the unexpected source that turns out to be exactly right
- Obscure technical history; primary sources over summaries

**Avoid:**
- Business books
- Anything that has appeared on a motivational poster
- Quotes that summarize the thesis directly — that's a caption, not an epigraph

---

## Footnotes

Tooltip style. Three jobs, sometimes in the same note:

1. **Humor** — the dry aside that would interrupt the main text's momentum. The footnote is where the smirk lives. Don't kill the joke by putting it in the body.
2. **Depth** — for the reader who wants to go further. Context and asides that aren't quite a full link. Don't over-explain in the body; offer the thread in the footnote.
3. **Citation** — source plus brief context. Not just a URL. One sentence on why it matters.

Footnotes should feel like marginalia from someone paying close attention, not endnotes from someone covering their bases. They're distinct from link previews (below): a footnote is *my* aside, written by me; a link preview is a window into *someone else's* page (or another note of mine), generated automatically rather than authored inline.

---

## Links & Previews

Every link — internal or external — shows an in-window preview on hover (desktop) or tap (mobile). No navigation required to see what's on the other end.

**Internal links** (note → note): the preview card shows the target note's title, epigraph, and opening paragraph. Enough to decide whether to follow it, not so much that following becomes pointless.

**External links** (note → the rest of the web): the preview card shows the destination's title, domain, and a short excerpt (`og:description` or equivalent). Same job — orient the reader before they leave.

**Recursion:** a preview can contain its own links, which can themselves preview. Let the reader go a few links deep without ever losing their place in the original note. This is the single biggest structural debt to Gwern — his `popups.js` is the reference implementation.

**Writing implication:** because the preview does some of the explaining, anchor text doesn't have to. Link the phrase that's actually the concept, not "click here" or a clause-long description of what's on the other end. Trust the preview — and the reader — to do the rest. Over-explanation in the body is condescension dressed as helpfulness. As the archive grows, link backward to earlier notes where a concept first appeared — build the web deliberately, don't just link forward.

**Build notes (not yet implemented):**
- Internal previews: generate from each note's frontmatter (title, epigraph, first paragraph) at build time — no runtime fetch needed.
- External previews: cache `og:` metadata at link-add time rather than fetching live on every hover, so a note doesn't depend on a third-party site staying up.
- Mobile: tap opens the preview card; a second tap (or a follow-through affordance inside the card) navigates.
- Dismiss on click-away or Esc.
- As the archive grows, consider a **backlinks** block at the bottom of each note — every note that links *to* this one, generated at build time. Gwern does this; it's what makes the wiki feel like a graph instead of a pile.

---

## Revision History

Every note carries a visible revision history: a panel (right rail on desktop, collapsible on mobile) listing dated revisions. Clicking a date opens a diff of what changed, in place — no separate page, no leaving the note.

**Why this exists:** the wiki's core claim is that notes are living documents. A claim like that is worthless if it's just asserted in prose. The revision panel makes it observable — a reader can watch a thesis get sharper, a claim get corrected, a section get added, across real revisions with real diffs.

**Voice implication:** don't rewrite silently. When a note changes materially, its revision entry gets a one-line description of what changed and why — Gwern-style: "Corrected the coverage numbers in the estimating example," "Added a section on latent vs. active errors," "Walked back the second claim, wasn't holding up." The revision log is allowed to admit the note was wrong before. That's the whole point of it existing.

**What counts as a revision worth logging:** a change to substance — claims, structure, examples, thesis. Typo fixes and formatting passes don't need their own entry; batch them or skip them. The log is for the reader who wants to trace how the thinking moved, not a git blame.

**Publishing implication:** this replaces the one-draft-one-publish model. A note can go live rough — thesis stated, argument sketched — and sharpen over weeks of real revisions. The diff panel is the receipt for that process instead of a liability to hide.

**Build notes (not yet implemented):**
- Static site, no CMS or database — revision history is derived from `git log` on each note's source file. Each commit touching the file becomes one panel entry (date + commit message as the one-line summary).
- Diff view renders the actual git diff for that commit, rendered as prose-diff (word-level, not line-level — line diffs on prose are close to unreadable).
- Generate a per-note JSON history file at build time (date, summary, diff) so the panel doesn't need a live git backend in production (relevant since hosting is plain static HTML on BlueHost).
- Commit messages for note changes should be written with this in mind — they become reader-facing copy, not just repo hygiene.

---

## Sign-Off

*A flourish, a fumble, a smirk, and a shrug.*

Keep it. Four words doing exactly what the voice does: ambition (flourish), honesty about the result (fumble), awareness of the gap (smirk), refusal to be precious about it (shrug). It's a stance, not a comment on the specific note. It will get more meaningful the longer the site runs.

---

## What to Avoid

Universal writing-craft avoids (lists substituting for argument, passive voice as a hedge, burying the thesis in qualifications, ending on a summary instead of the sharpest line, anything LinkedIn-thought-leadership-shaped) now live in `00_Citadel/Voice-Tone.md` Section III — this site is one instance of that rule, not a separate source of it.

Site-specific to the notes/wiki structure:
- Epigraphs that explain themselves
- Silent rewrites — if a claim materially changes, the revision history says so
- A reverse-chronological feed as primary navigation — this is a wiki, not a stream