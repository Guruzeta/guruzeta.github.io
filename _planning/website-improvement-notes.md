# Website Improvement Notes

Created: June 2026

## Current Temporary Direction

The site should currently read as a research-first physics website, not a fully rebranded ML + physics portfolio.

Near-term emphasis:

- Transitional turbulence
- Non-equilibrium phase transitions
- Tricritical directed percolation
- Stratified shear-flow transitions
- May's complexity-stability hypothesis
- Complex systems and random matrix stability

Applied ML, data science, and accelerator ML should remain visible, but they should be framed as computational methods and applied extensions rather than the primary brand.

## Changes Made In This Pass

- Homepage hero reframed from "Machine Learning for Complex Physical Systems" to "Statistical mechanics, turbulence, and machine learning."
- Sidebar tagline changed from "ML + Physics" to "Stat Mech · Turbulence · ML".
- Homepage about copy now foregrounds turbulence, instability, phase transitions, and complexity-stability.
- Projects page retitled to "Research + Applied Projects".
- Projects page now starts with research cards for:
  - Tricritical directed percolation in transitional turbulence
  - May's complexity-stability hypothesis in neural networks
  - Stratified shear-flow transition universality
- Applied ML/data projects remain lower on the Projects page.
- Research and Blog subtitles now avoid making ML theory the main framing.

## Later Rebrand Decisions

- Decide whether the long-term brand is:
  - Research physicist: turbulence and statistical mechanics
  - Scientific ML researcher: ML for complex physical systems
  - Hybrid: statistical physics of complex systems plus scientific ML
- Decide whether "Projects" should mean research projects, applied ML case studies, or both.
- Decide whether "Research" and "Projects" should be merged or clearly separated.
- Decide whether recruiter-facing project cards should live on a separate page such as `/applied/` or `/portfolio/`.

## Content Improvements To Tackle Later

- Add short visual summaries for the three core research projects.
- Add one plain-language explanation page for the PRL turbulence paper.
- Add a cleaner "Complexity-Stability" project page with:
  - motivation from May's theorem
  - what neural networks contribute as optimized systems
  - what observables are being measured
  - preliminary or planned diagnostics
- Add a "Current Research Questions" section to the homepage.
- Add a "Methods" section that connects finite-size scaling, Binder cumulants, stochastic modeling, spectral analysis, and machine learning.
- Make the applied ML cards shorter so they do not compete with the research cards.
- Add code or notebook links only when the repositories are clean and presentable.

## Design Improvements To Tackle Later

- Replace the profile image with a stronger final portrait when available.
- Consider a more physics-oriented visual language:
  - transition diagrams
  - phase-boundary motifs
  - turbulence/flow field imagery
  - sparse network spectra or eigenvalue plots
- Avoid making the site feel like a generic ML portfolio until the rebrand is intentional.
- Consider adding a small "Research Themes" row on the homepage.

## Technical Improvements To Tackle Later

- Move inline page CSS into reusable includes or a stylesheet.
- Replace hardcoded homepage research entries with data-driven entries from `_publications`.
- Fix the misspelled filename `_publications/2026-03-30-stratifed-turbulence-transition.md` while preserving the public permalink.
- Add link buttons inside project cards for matching Research detail pages.
- Create a clean build/test checklist for future edits.
