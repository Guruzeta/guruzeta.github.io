---
layout: site
permalink: /
title: "Guru Kalyan Jayasingh"
excerpt: "PhD candidate, statistical mechanics & turbulence — UC San Diego."
author_profile: false
sitemap: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  .v3-hero { display:grid; grid-template-columns:220px 1fr; gap:36px; align-items:center; padding-bottom:32px; border-bottom:1px solid var(--rule); }
  .v3-portrait {
    width:220px; height:220px; border-radius:18px; overflow:hidden;
    box-shadow: 0 18px 40px -18px rgba(0,0,0,0.35), 0 6px 14px -6px rgba(0,0,0,0.15);
    transition: transform .35s ease, box-shadow .35s ease;
    background:#eee;
  }
  .v3-portrait img { width:100%; height:100%; object-fit:cover; display:block; }
  .v3-portrait:hover { transform: translateY(-2px); box-shadow: 0 22px 50px -18px rgba(0,0,0,0.4), 0 8px 16px -6px rgba(0,0,0,0.18); }
  .v3-hero-body { display:flex; flex-direction:column; gap:20px; }
  .v3-hero-cta { display:flex; gap:10px; flex-wrap:wrap; }
  @media (max-width:780px){
    .v3-hero { grid-template-columns:1fr; gap:20px; justify-items:start; }
    .v3-portrait { width:160px; height:160px; border-radius:14px; }
  }

  /* social/contact icon row */
  .v3-links { list-style:none; padding:0; margin:6px 0 0; display:flex; flex-wrap:wrap; gap:8px; }
  .v3-links li {
    display:inline-flex; align-items:center; gap:8px;
    padding:7px 12px; border:1px solid var(--rule); border-radius:999px;
    background:#fff; color:var(--ink); font-size:13px; font-weight:500;
    transition:border-color .15s, transform .15s, background .15s;
  }
  .v3-links li > a {
    display:inline-flex; align-items:center; gap:8px;
    color:inherit; text-decoration:none;
  }
  .v3-links li:has(a):hover { border-color:var(--ink); transform:translateY(-1px); background:var(--soft); }
  .v3-ico { display:inline-flex; align-items:center; justify-content:center; color:var(--muted); line-height:0; }
  .v3-links li:hover .v3-ico { color:var(--ink); }
</style>

<div class="v3-wrap">

  <div class="v3-hero">
    <div class="v3-portrait">
      <img src="{{ base_path }}/images/profile_2.jpg" alt="Guru Kalyan Jayasingh">
    </div>
    <div class="v3-hero-body">
      <div>
        <h1 class="v3-name">Guru Kalyan Jayasingh</h1>
        <p class="v3-role">Physics PhD candidate, UC San Diego — statistical mechanics, turbulence, ML theory. This summer (2026): AI/ML Intern at <a href="https://www.tausystems.com" style="color:var(--ink); border-bottom:1px solid var(--rule);">TAU Systems</a>, building physics-informed ML for laser-plasma accelerators.</p>
      </div>
      <div class="v3-hero-cta">
        <a class="v3-btn primary" href="{{ base_path }}/files/Guru_K_Jayasingh_CV_Nov_2025.pdf">CV (PDF)</a>
        <a class="v3-btn" href="mailto:gjayasingh@ucsd.edu">Email</a>
      </div>

      <ul class="v3-links">
        <li>
          <span class="v3-ico" aria-hidden="true">
            <svg viewBox="0 0 24 24" width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
          </span>
          <span>San Diego, CA</span>
        </li>
        <li>
          <a href="mailto:gjayasingh@ucsd.edu">
            <span class="v3-ico" aria-hidden="true">
              <svg viewBox="0 0 24 24" width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
            </span>
            <span>Email</span>
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/guru-kalyan-jayasingh/" target="_blank" rel="noopener">
            <span class="v3-ico" aria-hidden="true">
              <svg viewBox="0 0 24 24" width="16" height="16" fill="currentColor"><path d="M19 0h-14c-2.76 0-5 2.24-5 5v14c0 2.76 2.24 5 5 5h14c2.76 0 5-2.24 5-5v-14c0-2.76-2.24-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.27c-.97 0-1.75-.79-1.75-1.76s.78-1.76 1.75-1.76 1.75.79 1.75 1.76-.78 1.76-1.75 1.76zm13.5 12.27h-3v-5.6c0-1.34-.03-3.07-1.87-3.07-1.87 0-2.16 1.46-2.16 2.97v5.7h-3v-11h2.88v1.5h.04c.4-.76 1.38-1.56 2.84-1.56 3.04 0 3.6 2 3.6 4.59v6.47z"/></svg>
            </span>
            <span>LinkedIn</span>
          </a>
        </li>
        <li>
          <a href="https://github.com/Guruzeta" target="_blank" rel="noopener">
            <span class="v3-ico" aria-hidden="true">
              <svg viewBox="0 0 24 24" width="16" height="16" fill="currentColor"><path d="M12 .5C5.65.5.5 5.65.5 12c0 5.08 3.29 9.39 7.86 10.91.58.11.79-.25.79-.56v-2c-3.2.7-3.87-1.54-3.87-1.54-.52-1.32-1.27-1.67-1.27-1.67-1.04-.71.08-.7.08-.7 1.15.08 1.76 1.18 1.76 1.18 1.02 1.75 2.68 1.24 3.34.95.1-.74.4-1.24.72-1.53-2.55-.29-5.24-1.28-5.24-5.7 0-1.26.45-2.29 1.18-3.1-.12-.29-.51-1.46.11-3.04 0 0 .97-.31 3.17 1.18a11 11 0 0 1 5.78 0c2.2-1.49 3.16-1.18 3.16-1.18.63 1.58.23 2.75.11 3.04.73.81 1.18 1.84 1.18 3.1 0 4.43-2.69 5.41-5.25 5.69.41.36.78 1.06.78 2.13v3.16c0 .31.21.67.79.56A11.5 11.5 0 0 0 23.5 12C23.5 5.65 18.35.5 12 .5z"/></svg>
            </span>
            <span>GitHub</span>
          </a>
        </li>
        <li>
          <a href="https://scholar.google.com/citations?hl=en&user=nmNd7oYAAAAJ" target="_blank" rel="noopener">
            <span class="v3-ico" aria-hidden="true">
              <svg viewBox="0 0 24 24" width="16" height="16" fill="currentColor"><path d="M12 14L2 8l10-6 10 6-10 6zm0 2.5l7-4.2v4.5c0 1.7-3.1 3.2-7 3.2s-7-1.5-7-3.2v-4.5l7 4.2z"/></svg>
            </span>
            <span>Google Scholar</span>
          </a>
        </li>
      </ul>
    </div>
  </div>

  <!-- ABOUT — intro paragraph from V1 -->
  <div class="v3-section">
    <h2 class="v3-h2">About</h2>
    <div class="v3-prose" style="max-width:760px;">
      <p>I study how ideas from statistical mechanics — phase transitions, universality, random matrices — explain complex systems that are far from equilibrium. My current work uses non-equilibrium critical phenomena to characterize the transition to turbulence in shear and stratified flows, and applies the same lens to optimized systems such as neural networks and ecological communities.</p>

      <p>I am advised by <a href="https://guava.physics.ucsd.edu/~nigel/">Nigel Goldenfeld</a>. Previously: Dual Degree (B.Tech + M.Tech) in Engineering Physics, IIT Bombay; research stints at Aalto University and TIFR Mumbai on quantum condensed matter and topological materials.</p>

      <p>Summer 2026: <strong>AI/ML Intern</strong> at <a href="https://www.tausystems.com">TAU Systems</a>, Carlsbad — physics-informed ML for laser-plasma electron accelerators.</p>
    </div>
  </div>

  <!-- PINNED — three things hiring managers should see first -->
  <div class="v3-section">
    <h2 class="v3-h2">Pinned</h2>
    <div class="v3-pinned">

      <div class="v3-pin">
        <a class="stretched" href="{{ base_path }}/publication/2025-09-03-tricritical-dp-body-force">Tricritical DP paper</a>
        <span class="v3-tag">PRL · 2025</span>
        <h3>Tricritical DP governs the laminar–turbulent transition under body forces</h3>
        <p>First-author paper showing pipe-flow transition under body forcing belongs to a new tricritical universality class. Covered by <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>. You can also <a href="https://chatgpt.com/g/g-68e699d7b85881918b87e4fae3b4f8c9-tricritical-dp-in-laminar-turbulent-transition">chat with the paper</a> — a custom GPT trained on it that explains, summarizes, and answers questions about the work.</p>
        <a class="more" href="{{ base_path }}/publication/2025-09-03-tricritical-dp-body-force">Read paper →</a>
      </div>

      <div class="v3-pin">
        <a class="stretched" href="{{ base_path }}/publication/2026-03-30-may-complexity-stability-neural-networks">May complexity-stability project</a>
        <span class="v3-tag">Project · in prep</span>
        <h3>Complexity–stability of trained neural networks</h3>
        <p>Random-matrix &amp; ecological-stability tools applied to gradient-trained networks. Probes which optimization regimes escape May's instability bound.</p>
        <a class="more" href="{{ base_path }}/publication/2026-03-30-may-complexity-stability-neural-networks">Project notes →</a>
      </div>

      <div class="v3-pin">
        <a class="stretched" href="{{ base_path }}/publication/2026-03-30-stratified-turbulence-dp-transition">Stratified turbulence project</a>
        <span class="v3-tag">Project · in prep</span>
        <h3>Universality class of stratified shear turbulence transitions</h3>
        <p>Large-domain DNS + finite-size scaling on a stratified Waleffe flow. Methodological contribution: Binder cumulants for DP transitions when wall-normal truncation breaks.</p>
        <a class="more" href="{{ base_path }}/publication/2026-03-30-stratified-turbulence-dp-transition">Project notes →</a>
      </div>

    </div>
  </div>

  <div class="v3-section v3-twocol">
    <div>
      <h2 class="v3-h2">Selected publications</h2>
      <ul class="v3-list">
        <li>
          <div class="v3-meta">Phys. Rev. Lett. 135, 104001 · 2025</div>
          <div class="v3-title"><a href="https://doi.org/10.1103/46g3-n7cx">Tricritical Directed Percolation Controls the Laminar–Turbulent Transition in Pipes with Body Forces</a></div>
          <div class="v3-blurb">Jayasingh &amp; Goldenfeld. Identifies the tricritical DP universality class governing pipe-flow transition under body forces; reconciles long-standing discrepancies in transition phenomenology.</div>
          <div class="v3-actions">
            <a href="https://doi.org/10.1103/46g3-n7cx">Paper</a>
            <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>
            <a href="https://chatgpt.com/g/g-68e699d7b85881918b87e4fae3b4f8c9-tricritical-dp-in-laminar-turbulent-transition">paper-GPT</a>
          </div>
        </li>
        <li>
          <div class="v3-meta">In preparation · 2026</div>
          <div class="v3-title"><a href="{{ base_path }}/publication/2026-03-30-stratified-turbulence-dp-transition">Universality class of turbulent transitions in stably stratified flows</a></div>
          <div class="v3-blurb">Finite-size scaling and Binder cumulants resolve whether stratification is a relevant perturbation to DP at the turbulent onset.</div>
        </li>
        <li>
          <div class="v3-meta">In preparation · 2026</div>
          <div class="v3-title"><a href="{{ base_path }}/publication/2026-03-30-may-complexity-stability-neural-networks">May's complexity–stability hypothesis in neural networks</a></div>
          <div class="v3-blurb">Treats trained networks as optimized interaction systems; asks whether SGD-trained dynamics violate random-matrix instability the way evolved ecosystems do.</div>
        </li>
      </ul>
      <div class="v3-actions" style="margin-top:14px;">
        <a href="{{ base_path }}/publications/">All publications →</a>
      </div>
    </div>

    <div>
      <h2 class="v3-h2">Toolkit</h2>
      <div class="v3-skills">
        <span class="v3-chip">Python (7+ yrs)</span>
        <span class="v3-chip">C / C++</span>
        <span class="v3-chip">Mathematica</span>
        <span class="v3-chip">PyTorch</span>
        <span class="v3-chip">TensorFlow</span>
        <span class="v3-chip">NumPy · SciPy · Pandas</span>
        <span class="v3-chip">scikit-learn</span>
        <span class="v3-chip">Matplotlib · Seaborn</span>
        <span class="v3-chip">XGBoost</span>
        <span class="v3-chip">Decision trees</span>
        <span class="v3-chip">Neural networks (RNN, LSTM)</span>
        <span class="v3-chip">Supervised learning / regression</span>
        <span class="v3-chip">Stochastic processes</span>
        <span class="v3-chip">Monte Carlo methods</span>
        <span class="v3-chip">Time-series analysis</span>
        <span class="v3-chip">Numerical methods</span>
        <span class="v3-chip">Statistical mechanics</span>
        <span class="v3-chip">Non-equilibrium phase transitions</span>
        <span class="v3-chip">Finite-size scaling</span>
      </div>

      <h2 class="v3-h2" style="margin-top:32px;">Background</h2>
      <p style="margin:0; color:var(--muted); font-size:14px;">
        PhD candidate, UCSD Physics, advised by <a href="https://guava.physics.ucsd.edu/~nigel/" style="color:var(--accent); text-decoration:none;">Nigel Goldenfeld</a>. Dual Degree (B.Tech + M.Tech), Engineering Physics, IIT Bombay. Research stints at Aalto University and TIFR Mumbai.
      </p>

      <h2 class="v3-h2" style="margin-top:32px;">Contact</h2>
      <p style="margin:0; color:var(--muted); font-size:14px;">
        <a href="mailto:gjayasingh@ucsd.edu" style="color:var(--accent);">gjayasingh@ucsd.edu</a> · <a href="mailto:gurukalyan1.618@gmail.com" style="color:var(--accent);">gurukalyan1.618@gmail.com</a>
      </p>
    </div>
  </div>

</div>
