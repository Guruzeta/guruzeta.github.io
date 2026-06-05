# Site Fix List — Ranked by ROI / Effort

Target audience: ML + physics recruiters / labs. Position as bridge, not chips.

Scoring: **ROI** = recruiter-impact, **Effort** = clock time, **Score** = ROI / Effort.

---

## Tier 0 — Free wins (do first, < 1 hr total)

These are zero-risk, ship-today fixes. Pure credibility recovery.

| # | Fix | ROI | Effort | Notes |
|---|-----|-----|--------|-------|
| 0.1 | Close unclosed `<div>` in PRL publication page | High | 2 min | `_publications/2025-09-03-tricritical-dp-body-force.md` — paper-GPT callout box missing `</div>` |
| 0.2 | Fix "University of San Diego California" → "University of California San Diego" | High | 2 min | `_teaching/2022-spring-teaching-2.md` line 2 |
| 0.3 | Fix IIT teaching permalink `/teaching/2014-spring-teaching-1` → `/teaching/2019-spring-teaching-1` | Med | 2 min | `_teaching/2019-spring-teaching-1.md` line 5 |
| 0.4 | Stop tracking `.DS_Store`; add to `.gitignore`; remove from index | Med | 5 min | currently dirty in git status |
| 0.5 | Update footer + hero CV link to current PDF | High | 5 min | site references Feb/Mar 2026 content but link = `Guru_K_Jayasingh_CV_Nov_2025.pdf`. Either rename to current or update href |
| 0.6 | Delete academicpages legacy pages: `markdown.md`, `archive-layout-with-content.md`, `non-menu-page.md`, `portfolio.html`, `terms.md`, sample comments residue | High | 10 min | Recruiter clicking one of these = instant judgment hit |
| 0.7 | Add Industry Resume PDF CTA next to CV (Resume_Feb_2026.pdf already in /files/) | High | 5 min | Two PDFs, two audiences. CV stays for academic, Resume for industry |

**Tier 0 total: ~30 min. Ships polished baseline. Do before anything else.**

---

## Tier 1 — Positioning rewrite (1-2 hrs, single highest leverage)

Site currently reads "physics PhD also interested in ML." Should read "bridge between physical modeling and ML."

| # | Fix | ROI | Effort | Notes |
|---|-----|-----|--------|-------|
| 1.1 | Rewrite hero one-liner to bridge-explicit positioning | Very High | 20 min | Candidate: "I build ML and statistical-physics models for complex physical systems — from turbulent flows to laser-plasma accelerators." Mirrors resume tone but sharper |
| 1.2 | Add "News" strip below hero (PRL Sept 2025 · TAU summer 2026 · talk dates · in-prep status) | High | 20 min | 5 bullets max. Makes site feel alive vs frozen |
| 1.3 | Rename landing "Pinned" → "Selected work" w/ ML+physics mix; promote SHM + Graph-RNN cards alongside PRL | Very High | 30 min | Card-grid same style as current. Mixes physics paper + ML projects = bridge visible at a glance |
| 1.4 | Add Awards strip (Silver Medal, Best Master's Thesis, IYPL 3rd India, INMO top-50, JEE 99.62%ile) as pill row | High | 15 min | Filter-pass signal. Costs nothing |

**Tier 1 total: ~1.5 hr. Single biggest perceived improvement.**

---

## Tier 2 — Case studies (the actual content gap, 1-2 days)

Both codex and direct review agree: portfolio evidence is the missing piece. Two strong > five weak.

| # | Fix | ROI | Effort | Notes |
|---|-----|-----|--------|-------|
| 2.1 | Case study page: SHM (LSTM, 34.8M-entry dataset) | Very High | 3-4 hr | Format: Problem → Data → Model → Baselines → Metrics → Result → Code. Numbers from resume: MSE 0.00278 → 0.0347 (12.5×), 85.29% / 17 states, Welch PSD features |
| 2.2 | Case study page: Graph-RNN (NSF HDR, $4k pool, 17th global) | Very High | 3-4 hr | Same format. 3-layer GRU + graph conv, scheduled sampling, R²=0.80, beat ARIMA/ETS |
| 2.3 | Add 1 figure to PRL pinned card (scaling collapse / phase diagram / Binder cumulant) | Very High | 1 hr | Site currently 100% text. Single biggest "feels professional" lever |
| 2.4 | Link GitHub repos for both case studies (clean up + pin on GH profile) | High | 1-2 hr | Quant/ML recruiters want to see code. Currently zero code links from site |
| 2.5 | Add Fukushima diffusion model as third compact card | Med | 1 hr | Physics-ML bridge artifact, demonstrates modeling instinct |

**Tier 2 total: ~1-2 days. Where the actual hiring impact lives.**

---

## Tier 3 — Blog decision (30 min OR 1 day)

Empty blog hurts more than no blog. Pick one:

| # | Fix | ROI | Effort | Notes |
|---|-----|-----|--------|-------|
| 3.A | Hide blog from nav until first real post exists | Med | 10 min | Safe option |
| 3.B | Ship 1 real technical post (DP derivation walk-through, finite-size scaling explainer, ML-theory note) | High | 4-8 hr | Signals writing ability + thinking. If shipping, do one well |

---

## Tier 4 — Structural / sustainability (later, when time permits)

| # | Fix | ROI | Effort | Notes |
|---|-----|-----|--------|-------|
| 4.1 | Refactor dark mode: replace `!important` overrides w/ proper `[data-theme="dark"]` cascade | Low | 2-3 hr | Codex correct that current setup is fragile. Not visible to recruiters but breaks as pages grow |
| 4.2 | Add BibTeX + slides + plain-language summary affordances to publications | Med | 1-2 hr per paper | Polish layer; matters for academic audience |
| 4.3 | Polish PRL page paper-GPT callout (currently has unclosed div + structural issues) | Med | 30 min | Post-bugfix tightening |
| 4.4 | Research statement page (3-5 paragraph intellectual agenda) | Med | 2-3 hr | Useful for grad-school / postdoc audience; less critical for industry |
| 4.5 | Surface Topology Quantum Matter + Kadanoff-Baym solver as research blurbs | Med | 1 hr | C++/numerical depth currently invisible |

---

## Execution order (recommended)

**Session 1 (today, ~1 hr):** Tier 0 entire (bug fixes + cleanup + resume CTA).
**Session 2 (this week, ~2 hr):** Tier 1 (positioning rewrite + News + Selected work + Awards).
**Session 3 (next week, ~1-2 days):** Tier 2 (case studies — the actual content gap).
**Session 4 (decide):** Tier 3 (blog ship or hide).
**Backlog:** Tier 4 (sustainability + polish).

---

## What NOT to do

- Build two separate websites. One site, two paths. Maintenance drag + identity split.
- Add a `/scientific-ml/` index page before the case studies exist. Empty section worse than no section.
- More chips/keywords without proof. Site already lists PyTorch/XGBoost/RNN. Recruiters discount lists; they want artifacts.
- Add TAU outcomes before internship starts (June 2026). Frame as "current work," don't claim results yet.
