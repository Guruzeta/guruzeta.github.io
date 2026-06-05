# Website Roadmap

Created: June 2026

## Current Positioning

The site should currently read as a research-first physics website centered on:

- Statistical mechanics
- Transitional turbulence
- Non-equilibrium phase transitions
- Complexity-stability
- Scientific machine learning as a method, not yet the whole brand

The current homepage line is the right temporary anchor:

> Statistical mechanics, turbulence, and machine learning.

The supporting sentence should keep emphasizing that the work develops quantitative models for physical phenomena. This avoids over-branding the site as a generic ML portfolio before the ML + physics rebrand is fully built.

## Primary Audiences

Academic physics audience:

- Needs to see a coherent research agenda.
- Should immediately find the PRL turbulence work, current in-prep projects, talks, CV, and advisor/context.

Scientific ML / applied research audience:

- Needs to see that the ML work is tied to physical systems, time series, surrogate modeling, and quantitative modeling.
- Should find applied projects, but not at the expense of the research identity.

Recruiting / internship audience:

- Needs evidence of implementation ability, clean metrics, and project outcomes.
- Should find resume, projects, and contact quickly.

## What Is Done

- Active site now uses a compact custom template instead of the previous academicpages visual system.
- Sidebar rail is the primary navigation across all current routes.
- Dark mode persists across page changes.
- Homepage hero now emphasizes stat mech, turbulence, and ML.
- News section is back on the homepage.
- Projects page starts with turbulence, complexity-stability, and stratified-flow research before applied ML work.
- Golden Handcuffs project is present.
- Fukushima project is removed.
- Current public image folder only contains active assets.
- Old academicpages templates, demo pages, Sass, JS, talkmap helpers, sample images, old mockup, and old fix list are archived under `_legacy/`.

## Launch Checklist Before Push

- Run `bundle exec jekyll build --config _config.yml,_config.dev.yml`.
- Click through:
  - `/`
  - `/projects/`
  - `/publications/`
  - `/talks/`
  - `/blog/`
  - `/teaching/`
  - `/cv/`
  - `/blog/notes/`
- Test dark mode after navigating across at least three pages.
- Check all PDF links:
  - Resume
  - Academic CV
  - Notes PDFs
- Check that no public route exposes old academicpages pages.
- Review `git status --short` before staging.

## Positioning Improvements

1. Decide the long-term brand.
   - Option A: Research physicist in turbulence and statistical mechanics.
   - Option B: Scientific ML researcher for complex physical systems.
   - Option C: Hybrid statistical physics + scientific ML.
   - Current site should stay closest to Option C, with the physics side leading.

2. Make the intellectual agenda explicit.
   - Add a short "Research Questions" section to the homepage.
   - Candidate questions:
     - How do turbulent systems transition between stable and unstable states?
     - When does complexity destabilize a system, and when does structure stabilize it?
     - How can data-driven models respect physical constraints?

3. Clarify "Research" versus "Projects".
   - Research should remain papers, talks, and in-prep academic directions.
   - Projects should remain a bridge page with research cards first and applied modeling cards second.
   - If applied work grows, create a separate `/applied/` or `/case-studies/` page later.

4. Add a one-paragraph research statement.
   - This should sit near the homepage About section or on a new `/research-statement/` route.
   - It should connect turbulence, phase transitions, random matrix stability, and scientific ML.

## Research Content Improvements

1. Upgrade the PRL page.
   - Add a plain-language summary.
   - Add one figure or schematic:
     - phase diagram
     - scaling collapse
     - tricritical point schematic
   - Add "What this changes" and "Predictions" sections.

2. Build a stronger complexity-stability page.
   - Explain May's theorem in plain language.
   - Explain why neural networks are useful optimized complex systems.
   - List measurable observables:
     - spectrum
     - interaction matrix structure
     - pairwise correlations
     - stability margins
     - topology or low-rank structure

3. Build a stronger stratified turbulence page.
   - Explain why stratification may be a relevant perturbation to DP.
   - Explain finite-size scaling and Binder cumulants briefly.
   - Add current status, expected outputs, and simulation constraints.

4. Add paper metadata polish.
   - Add BibTeX for published papers.
   - Add slide links where clean.
   - Add "Related work" links for each research page.

## Applied Project Improvements

1. Structural health monitoring case study.
   - Add a dedicated page with:
     - problem statement
     - dataset size and sensors
     - healthy dynamics prediction setup
     - LSTM architecture
     - residual anomaly detection
     - Welch PSD / FFT feature pipeline
     - metrics and limitations
   - Add a small result figure if available.

2. Graph-RNN ECG forecasting case study.
   - Add a dedicated page with:
     - problem statement
     - graph structure
     - GRU architecture
     - scheduled sampling
     - baseline comparisons
     - in-distribution and OOD behavior
   - Link code only when the repository is cleaned.

3. Golden Handcuffs project.
   - Add a compact case study page if it remains relevant to recruiting.
   - Emphasize data ingestion, panel construction, econometric baselines, XGBoost, SHAP, and state-level segmentation.
   - Keep it below physics/scientific ML projects unless the audience is explicitly data science.

4. TAU Systems accelerator ML.
   - Keep current language conservative until internship outputs are public.
   - Add a sanitized project page later if allowed.
   - Avoid claiming results before the work is complete.

## Design Improvements

1. Replace the profile image when the final picture is ready.
   - Use a sharper, higher-resolution portrait.
   - Keep the crop professional and natural.
   - Avoid overly stylized avatar imagery for the main academic site.

2. Add visual research cues.
   - Turbulence flow field.
   - Phase diagram.
   - Scaling collapse.
   - Eigenvalue spectrum.
   - Sparse network or interaction matrix.

3. Reduce inline CSS over time.
   - Move page-specific styles into `_includes/site/style.html` or a proper stylesheet.
   - Keep class naming consistent; current `v3-*` classes can be renamed later if desired.

4. Improve mobile polish.
   - Check sidebar drawer behavior.
   - Check hero text wrapping.
   - Check project card density.
   - Check CV table-of-contents layout.

## Technical Improvements

1. Data-drive homepage research entries.
   - Pull selected research cards from `_publications/` metadata instead of hardcoding them.

2. Fix publication filename spelling.
   - Current file has `stratifed` in the filename.
   - Preserve the existing permalink while renaming the file to `stratified`.

3. Add a small build checklist script.
   - Build site.
   - Confirm key routes exist in `_site`.
   - Grep for archived route names in `_site`.

4. Add link integrity checks.
   - Internal links.
   - PDF links.
   - External DOI/news links.

5. Review SEO/social metadata.
   - Confirm Open Graph image.
   - Confirm homepage excerpt.
   - Confirm title and description.
   - Add ORCID if available.

## GitHub Push Checklist

Suggested sequence:

```bash
bundle exec jekyll build --config _config.yml,_config.dev.yml
git status --short
git add .
git status --short
git commit -m "Rebuild website around current research template"
git push
```

After push:

- Wait for GitHub Pages to rebuild.
- Open `https://guruzeta.github.io/`.
- Test the same click path as the local launch checklist.
- Confirm dark mode persists on the deployed site.
