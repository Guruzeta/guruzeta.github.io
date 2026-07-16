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
    font-size:50px;
    line-height:1.1;
    letter-spacing:0;
    margin:0 0 16px;
    color:var(--ink);
  }
  .home-tag {
    font-size:14px; color:var(--muted); margin:0 0 26px; line-height:1.55;
  }
  .home-tag span.k { color:var(--ink); }
  .home-tag .sep { color:var(--rule); margin:0 8px; }
  .home-lead {
    font-size:18px; line-height:1.55; color:var(--ink); margin:0 0 13px;
    max-width:700px;
  }

  .home-cta { display:flex; gap:9px; flex-wrap:wrap; margin-bottom:40px; }
  .home-btn {
    padding:9px 15px; border-radius:7px; border:1px solid var(--rule);
    background:var(--paper); color:var(--ink); font-size:14px; font-weight:500;
    text-decoration:none; transition: border-color .15s, background .15s, transform .15s;
  }
  .home-btn:hover { border-color:var(--ink); transform:translateY(-1px); }
  .home-btn.primary { background:var(--ink); color:var(--on-ink); border-color:var(--ink); }

  .home-sec { margin-top:48px; }
  .home-sec h2 {
    font-family:'JetBrains Mono', monospace;
    font-size:12px; font-weight:500; letter-spacing:0.18em; text-transform:uppercase;
    color:var(--muted); margin:0 0 16px;
  }
  .home-prose p { font-size:16.5px; line-height:1.66; color:var(--ink); margin:0 0 18px; }
  .home-prose a { color:var(--accent); text-decoration:none; border-bottom:1px solid transparent; transition:border-color .15s; }
  .home-prose a:hover { border-color:var(--accent); }

  /* --- credentials --- */
  .home-creds { display:flex; flex-direction:column; gap:14px; margin-top:0; }
  .home-cred {
    border:1px solid var(--rule); border-radius:8px; padding:20px 22px;
    display:grid; grid-template-columns:48px 1fr; gap:16px; align-items:start;
    background:var(--panel);
  }
  .home-cred-logo {
    width:48px; height:48px; border-radius:10px; object-fit:contain;
    background:#fff; border:1px solid var(--rule); padding:5px;
  }
  .home-cred .cred-head {
    display:flex; justify-content:space-between; align-items:baseline;
    gap:14px; margin:0 0 4px;
  }
  .home-cred .label {
    font-family:'JetBrains Mono', monospace; font-size:11px; letter-spacing:0.15em;
    text-transform:uppercase; color:var(--accent); font-weight:600; margin:0;
  }
  .home-cred .when {
    font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.08em;
    color:var(--muted); white-space:nowrap;
  }
  .home-cred h3 {
    font-family:'Source Serif 4', serif; font-size:20px; line-height:1.25;
    font-weight:600; color:var(--ink); margin:0 0 5px;
  }
  .home-cred p { color:var(--muted); font-size:14.5px; line-height:1.55; margin:0; }
  .home-awards { margin-top:34px; }
  .home-awards h2 {
    font-family:'JetBrains Mono', monospace;
    font-size:12px; font-weight:500; letter-spacing:0.18em; text-transform:uppercase;
    color:var(--muted); margin:0 0 16px;
  }
  .home-awards-list { list-style:none; padding:0; margin:0; display:flex; flex-direction:column; }
  .home-awards-list li {
    padding:14px 0; border-bottom:1px solid var(--rule);
  }
  .home-awards-list li:last-child { border-bottom:0; }
  .home-awards-list .aw-head {
    display:flex; justify-content:space-between; align-items:baseline; gap:14px;
  }
  .home-awards-list .aw-name { font-size:15.5px; color:var(--ink); font-weight:600; }
  .home-awards-list .aw-where {
    font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.08em;
    color:var(--muted); white-space:nowrap;
  }
  .home-awards-list .aw-desc { font-size:14.5px; color:var(--muted); line-height:1.55; margin:4px 0 0; }
  @media (max-width:560px){
    .home-cred .cred-head, .home-awards-list .aw-head { flex-direction:column; gap:2px; }
  }

  /* --- news --- */
  .home-news { list-style:none; padding:0; margin:0; display:flex; flex-direction:column; }
  .home-news li { display:grid; grid-template-columns:110px 1fr; gap:24px; align-items:baseline; padding:14px 0; border-bottom:1px solid var(--rule); }
  .home-news li:last-child { border-bottom:0; }
  .home-news .when { font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.1em; text-transform:uppercase; color:var(--muted); }
  .home-news .what { font-size:15px; color:var(--ink); line-height:1.58; }
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

  @media (max-width:780px){
    .home-h1 { font-size:38px; }
    .home-lead { font-size:17px; }
    .home-creds { grid-template-columns:1fr; }
  }
</style>

<h1 class="home-h1">Hi, I'm Guru.</h1>
<p class="home-lead">I'm a fourth-year Physics PhD student at UC San Diego, advised by <a href="https://guava.physics.ucsd.edu/~nigel/" style="color:var(--accent); text-decoration:none;">Nigel Goldenfeld</a>, working on the statistical mechanics of turbulence and machine learning.</p>
<p class="home-lead">The common thread in my work is how complex systems become unstable, transition, and organize — and I study it in two settings. In fluids, I showed that the laminar–turbulent transition in pipes with body forces is governed by tricritical directed percolation (<a href="https://doi.org/10.1103/46g3-n7cx" style="color:var(--accent); text-decoration:none;">Physical Review Letters, 2025</a>), and I am testing its universality in stratified flows. In machine learning, I ask whether trained neural networks escape the random-matrix instability that May's complexity–stability theorem predicts for complex systems.</p>
<p class="home-lead">My tools: non-equilibrium phase transitions, finite-size scaling, stochastic modeling, and random-matrix theory.</p>
<p class="home-lead">Before UCSD, I did a Dual Degree in Engineering Physics at <a href="https://www.iitb.ac.in/" style="color:var(--accent); text-decoration:none;">IIT Bombay</a>, working on quantum condensed matter with <a href="https://www.phy.iitb.ac.in/en/content/hridis-kumar-pal" style="color:var(--accent); text-decoration:none;">Hridis Kumar Pal</a> on topological insulator–superconductor junctions. I also spent time at <a href="https://theory.tifr.res.in/" style="color:var(--accent); text-decoration:none;">TIFR Mumbai</a> on electron–phonon equilibration via Keldysh field theory, and at <a href="https://www.aalto.fi/en" style="color:var(--accent); text-decoration:none;">Aalto University</a> on fluctuations in non-centrosymmetric superconductors.</p>

<div class="home-cta">
  <a class="home-btn primary" href="{{ '/publications/' | relative_url }}">View Research</a>
  <a class="home-btn" href="{{ '/files/Guru_Jayasingh_CV.pdf' | relative_url }}">Academic CV</a>
</div>

<section class="home-sec" style="margin-top:0;">
  <h2>Affiliations</h2>
  <div class="home-creds">
    <div class="home-cred">
      <img class="home-cred-logo" src="{{ '/images/ucsd_seal.png' | relative_url }}" alt="UC San Diego seal">
      <div>
        <div class="cred-head">
          <p class="label">Current</p>
          <span class="when">2022 – present</span>
        </div>
        <h3>UC San Diego Physics</h3>
        <p>Ph.D. candidate in theoretical physics. Thesis work: transition to turbulence under body forces, stratified flows, and the statistical mechanics of machine learning.</p>
      </div>
    </div>
    <div class="home-cred">
      <img class="home-cred-logo" src="{{ '/images/iitb_logo.svg' | relative_url }}" alt="IIT Bombay logo">
      <div>
        <div class="cred-head">
          <p class="label">Education</p>
          <span class="when">2017 – 2022</span>
        </div>
        <h3>IIT Bombay</h3>
        <p>Dual Degree (B.Tech + M.Tech) in Engineering Physics, specialization in Nanoscience. Master's thesis on topological insulator–superconductor junctions.</p>
      </div>
    </div>
  </div>
</section>

<section class="home-sec">
  <h2>Selected Research</h2>
  <ul class="home-pubs">
    <li>
      <div class="meta">Physical Review Letters 135, 104001 · Peer-reviewed · 2025</div>
      <div class="title"><a href="{{ '/publication/2025-09-03-tricritical-dp-body-force' | relative_url }}">Tricritical Directed Percolation Controls the Laminar–Turbulent Transition in Pipes with Body Forces</a></div>
      <p class="blurb">Jayasingh &amp; Goldenfeld. Identifies the tricritical DP universality class governing pipe-flow transition under body forces; reconciles long-standing discrepancies in transition phenomenology.</p>
      <div class="actions">
        <a href="https://doi.org/10.1103/46g3-n7cx">Paper</a>
        <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>
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
      <span class="what">First-author paper published in <a href="https://doi.org/10.1103/46g3-n7cx">Physical Review Letters 135, 104001</a>; covered by <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>.</span>
    </li>
    <li>
      <span class="when">Mar 2025</span>
      <span class="what">Talk at the <a href="{{ '/talks/2025-03-17-talk-1' | relative_url }}">APS Global Physics Summit</a>, Anaheim CA.</span>
    </li>
  </ul>
</section>

<section class="home-sec">
  <div class="home-awards">
    <h2>Honors</h2>
    <ul class="home-awards-list">
      <li>
        <div class="aw-head">
          <span class="aw-name">Institute Silver Medal</span>
          <span class="aw-where">IIT Bombay · 2022</span>
        </div>
        <p class="aw-desc">Awarded to the top-ranked student in the graduating class of each academic program.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">K. Seshia Research Excellence Award</span>
          <span class="aw-where">IIT Bombay · 2022</span>
        </div>
        <p class="aw-desc">Given for the best Master's thesis in Physics, recognizing research originality and rigor.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">Physics Excellence Award</span>
          <span class="aw-where">UC San Diego · 2022</span>
        </div>
        <p class="aw-desc">Departmental award from the UC San Diego Department of Physics.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">Institute Academic Prizes</span>
          <span class="aw-where">IIT Bombay · 2019, 2021</span>
        </div>
        <p class="aw-desc">Annual award for the highest GPA in the Physics Department.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">Aalto Science Institute (AScI) Fellowship</span>
          <span class="aw-where">Finland · 2020</span>
        </div>
        <p class="aw-desc">International research fellowship for top students in science and engineering.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">Indian Young Physicists' League — All-India Rank 3</span>
          <span class="aw-where">India · 2021</span>
        </div>
        <p class="aw-desc">National theoretical physics competition.</p>
      </li>
      <li>
        <div class="aw-head">
          <span class="aw-name">KVPY Fellowship</span>
          <span class="aw-where">Dept. of Science &amp; Technology, India · 2017</span>
        </div>
        <p class="aw-desc">National fellowship for the top ~1% of science students identified for research potential.</p>
      </li>
    </ul>
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
