---
layout: site
permalink: /
title: "Guru Kalyan Jayasingh"
excerpt: "Physics PhD, UC San Diego — turbulence, phase transitions, and complexity-stability."
author_profile: false
sitemap: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  .home-h1 {
    font-family:'Source Serif 4', serif;
    font-weight:600;
    font-size:58px;
    line-height:1.08;
    letter-spacing:-0.015em;
    margin:0 0 18px;
    color:var(--ink);
  }
  .home-tag {
    font-size:15px; color:var(--muted); margin:0 0 30px; line-height:1.6;
  }
  .home-tag span.k { color:var(--ink); }
  .home-tag .sep { color:var(--rule); margin:0 8px; }
  .home-lead {
    font-size:20px; line-height:1.6; color:var(--ink); margin:0 0 14px;
    max-width:740px;
  }

  .home-cta { display:flex; gap:10px; flex-wrap:wrap; margin-bottom:48px; }
  .home-btn {
    padding:10px 18px; border-radius:8px; border:1px solid var(--rule);
    background:var(--paper); color:var(--ink); font-size:15px; font-weight:500;
    text-decoration:none; transition: border-color .15s, background .15s, transform .15s;
  }
  .home-btn:hover { border-color:var(--ink); transform:translateY(-1px); }
  .home-btn.primary { background:var(--ink); color:var(--on-ink); border-color:var(--ink); }

  .home-sec { margin-top:56px; }
  .home-sec h2 {
    font-family:'JetBrains Mono', monospace;
    font-size:13px; font-weight:500; letter-spacing:0.18em; text-transform:uppercase;
    color:var(--muted); margin:0 0 18px;
  }
  .home-prose p { font-size:18px; line-height:1.72; color:var(--ink); margin:0 0 20px; }
  .home-prose a { color:var(--accent); text-decoration:none; border-bottom:1px solid transparent; transition:border-color .15s; }
  .home-prose a:hover { border-color:var(--accent); }

  /* --- news --- */
  .home-news { list-style:none; padding:0; margin:0; display:flex; flex-direction:column; }
  .home-news li { display:grid; grid-template-columns:110px 1fr; gap:24px; align-items:baseline; padding:14px 0; border-bottom:1px solid var(--rule); }
  .home-news li:last-child { border-bottom:0; }
  .home-news .when { font-family:'JetBrains Mono', monospace; font-size:13px; letter-spacing:0.1em; text-transform:uppercase; color:var(--muted); }
  .home-news .what { font-size:16px; color:var(--ink); line-height:1.6; }
  .home-news .what a { color:var(--accent); text-decoration:none; border-bottom:1px solid transparent; }
  .home-news .what a:hover { border-bottom-color:var(--accent); }
  @media (max-width:560px){ .home-news li { grid-template-columns:1fr; gap:4px; } }

  /* --- pinned mini cards --- */
  .home-pins { display:flex; flex-direction:column; gap:14px; }
  .home-pin { border:1px solid var(--rule); border-radius:8px; padding:18px 20px; position:relative; transition: border-color .15s, transform .15s; }
  .home-pin:hover { border-color:var(--ink); transform:translateY(-1px); }
  .home-pin .tag { font-family:'JetBrains Mono', monospace; font-size:11px; letter-spacing:0.15em; text-transform:uppercase; color:var(--accent); font-weight:600; }
  .home-pin h3 { font-family:'Source Serif 4', serif; font-size:19px; font-weight:600; margin:6px 0 6px; line-height:1.35; }
  .home-pin p { margin:0 0 8px; color:var(--muted); font-size:15px; line-height:1.58; }
  .home-pin .more { font-size:14px; color:var(--accent); text-decoration:none; font-weight:500; }
  .home-pin .stretched { position:absolute; inset:0; z-index:1; text-indent:-9999px; overflow:hidden; border-radius:inherit; }
  .home-pin p a, .home-pin .more { position:relative; z-index:2; color:var(--accent); text-decoration:none; }
  .home-pin p a:hover, .home-pin .more:hover { border-bottom:1px solid var(--accent); }

  /* --- pub list compact --- */
  .home-pubs { list-style:none; padding:0; margin:0; display:flex; flex-direction:column; gap:18px; }
  .home-pubs li { padding-bottom:18px; border-bottom:1px solid var(--rule); }
  .home-pubs li:last-child { border-bottom:0; }
  .home-pubs .meta { font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.1em; text-transform:uppercase; color:var(--muted); }
  .home-pubs .title { font-family:'Source Serif 4', serif; font-size:19px; font-weight:600; margin:4px 0 6px; line-height:1.35; }
  .home-pubs .title a { color:var(--ink); text-decoration:none; border-bottom:1px solid transparent; }
  .home-pubs .title a:hover { border-color:var(--accent); color:var(--accent); }
  .home-pubs .blurb { font-size:15px; color:var(--muted); margin:0 0 6px; line-height:1.6; }
  .home-pubs .actions { display:flex; gap:14px; font-size:14px; }
  .home-pubs .actions a { color:var(--accent); text-decoration:none; }
  .home-pubs .actions a:hover { text-decoration:underline; }

  /* --- toolkit --- */
  .home-chips { display:flex; flex-wrap:wrap; gap:6px; }
  .home-chip { font-size:13px; padding:5px 10px; background:var(--soft); border-radius:999px; color:var(--ink); }

  @media (max-width:780px){
    .home-h1 { font-size:42px; }
  }
</style>

<h1 class="home-h1">Statistical mechanics, turbulence, and machine learning.</h1>
<p class="home-lead">I study how complex systems become unstable, transition, and organize, from laminar-turbulent flows to optimized neural networks.</p>
<p class="home-lead">My work combines non-equilibrium phase transitions, finite-size scaling, stochastic modeling, and data-driven methods to develop quantitative models for physical phenomena.</p>
<p class="home-tag">
  <span class="k">Transitional turbulence</span><span class="sep">|</span>
  <span class="k">Complexity-stability</span><span class="sep">|</span>
  <span class="k">Scientific ML</span>
</p>

<div class="home-cta">
  <a class="home-btn primary" href="{{ '/publications/' | relative_url }}">View Research</a>
  <a class="home-btn" href="{{ '/projects/' | relative_url }}">Projects</a>
  <a class="home-btn" href="{{ '/files/Guru_Jayasingh_Resume.pdf' | relative_url }}">Resume (PDF)</a>
  <a class="home-btn" href="{{ '/files/Guru_Jayasingh_CV.pdf' | relative_url }}">Academic CV</a>
  <a class="home-btn" href="mailto:gjayasingh@ucsd.edu">Email</a>
</div>

<section class="home-sec home-prose">
  <h2>About</h2>
  <p>My PhD work, advised by <a href="https://guava.physics.ucsd.edu/~nigel/">Nigel Goldenfeld</a>, focuses on the statistical mechanics of turbulence and instability. I use non-equilibrium phase transitions, finite-size scaling, stochastic modeling, and random-matrix ideas to characterize how disordered physical systems transition between stable and unstable states.</p>

  <p>Current projects center on tricritical directed percolation in transitional turbulence, the universality class of stratified shear-flow transitions, and May's complexity-stability hypothesis in optimized systems such as neural networks.</p>

  <p>Previously: Dual Degree (B.Tech + M.Tech) in Engineering Physics at IIT Bombay — Institute Silver Medal, Best Master's Thesis. Research stints at Aalto University and TIFR Mumbai on quantum condensed matter and topological materials.</p>
</section>

<section class="home-sec">
  <h2>News</h2>
  <ul class="home-news">
    <li>
      <span class="when">Jun 2026</span>
      <span class="what"><strong>AI/ML Intern</strong> at <a href="https://www.tausystems.com">TAU Systems</a> (Carlsbad) — physics-informed ML for laser-plasma electron accelerators.</span>
    </li>
    <li>
      <span class="when">Oct 2025</span>
      <span class="what">Talk on tricritical DP &amp; transitional turbulence at the <a href="{{ '/talks/2025-10-18-talk-2' | relative_url }}">JIFT Workshop on Strong Turbulence</a>, UC San Diego.</span>
    </li>
    <li>
      <span class="when">Sep 2025</span>
      <span class="what">First-author paper published in <a href="https://doi.org/10.1103/46g3-n7cx">Phys. Rev. Lett. 135, 104001</a>; covered by <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>.</span>
    </li>
    <li>
      <span class="when">Mar 2025</span>
      <span class="what">Talk at the <a href="{{ '/talks/2025-03-17-talk-1' | relative_url }}">APS Global Physics Summit</a>, Anaheim CA.</span>
    </li>
  </ul>
</section>

<section class="home-sec">
  <h2>Selected Research</h2>
  <ul class="home-pubs">
    <li>
      <div class="meta">Phys. Rev. Lett. 135, 104001 · 2025</div>
      <div class="title"><a href="{{ '/publication/2025-09-03-tricritical-dp-body-force' | relative_url }}">Tricritical Directed Percolation Controls the Laminar–Turbulent Transition in Pipes with Body Forces</a></div>
      <p class="blurb">Jayasingh &amp; Goldenfeld. Identifies the tricritical DP universality class governing pipe-flow transition under body forces; reconciles long-standing discrepancies in transition phenomenology.</p>
      <div class="actions">
        <a href="https://doi.org/10.1103/46g3-n7cx">Paper</a>
        <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>
        <a href="https://chatgpt.com/g/g-68e699d7b85881918b87e4fae3b4f8c9-tricritical-dp-in-laminar-turbulent-transition">paper-GPT</a>
      </div>
    </li>
    <li>
      <div class="meta">In preparation · 2026</div>
      <div class="title"><a href="{{ '/publication/2026-03-30-stratified-turbulence-dp-transition' | relative_url }}">Universality class of turbulent transitions in stably stratified flows</a></div>
      <p class="blurb">Finite-size scaling and Binder cumulants resolve whether stratification is a relevant perturbation to DP at the turbulent onset.</p>
    </li>
    <li>
      <div class="meta">In preparation · 2026</div>
      <div class="title"><a href="{{ '/publication/2026-03-30-may-complexity-stability-neural-networks' | relative_url }}">May's complexity–stability hypothesis in neural networks</a></div>
      <p class="blurb">Treats trained networks as optimized interaction systems; asks whether SGD-trained dynamics violate random-matrix instability the way evolved ecosystems do.</p>
    </li>
  </ul>
  <p style="margin-top:14px; font-size:15px;"><a href="{{ '/publications/' | relative_url }}" style="color:var(--accent); text-decoration:none;">All publications →</a></p>
</section>

<section class="home-sec">
  <h2>Toolkit</h2>
  <div class="home-chips">
    <span class="home-chip">Python (7+ yrs)</span>
    <span class="home-chip">PyTorch</span>
    <span class="home-chip">scikit-learn</span>
    <span class="home-chip">XGBoost</span>
    <span class="home-chip">C / C++</span>
    <span class="home-chip">NumPy · SciPy · Pandas</span>
    <span class="home-chip">RNN / LSTM / GRU</span>
    <span class="home-chip">Time-series analysis</span>
    <span class="home-chip">Monte Carlo methods</span>
    <span class="home-chip">Statistical mechanics</span>
    <span class="home-chip">Non-equilibrium phase transitions</span>
    <span class="home-chip">Finite-size scaling</span>
  </div>
</section>

<section class="home-sec">
  <h2>Contact</h2>
  <p style="font-size:16px; color:var(--ink); margin:0;">
    <a href="mailto:gjayasingh@ucsd.edu" style="color:var(--accent); text-decoration:none;">gjayasingh@ucsd.edu</a>
    <span style="color:var(--rule); margin:0 10px;">·</span>
    <a href="mailto:gurukalyan1.618@gmail.com" style="color:var(--accent); text-decoration:none;">gurukalyan1.618@gmail.com</a>
  </p>
  <p style="font-size:14px; color:var(--muted); margin:8px 0 0;">San Diego, CA</p>
</section>
