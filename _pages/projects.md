---
layout: site
permalink: /projects/
title: "Research + Applied Projects"
excerpt: "Research projects in turbulence, phase transitions, and complexity-stability, followed by selected applied modeling work."
author_profile: false
sitemap: true
---

<style>
  .proj-head { padding-bottom:32px; border-bottom:1px solid var(--rule); margin-bottom:36px; }
  .proj-h1 { font-family:'Source Serif 4', serif; font-weight:600; font-size:48px; line-height:1.1; letter-spacing:-0.015em; margin:0 0 14px; color:var(--ink); }
  .proj-intro { font-size:17px; line-height:1.68; color:var(--muted); margin:0 0 18px; max-width:700px; }
  .proj-intro a { color:var(--accent); text-decoration:none; border-bottom:1px solid transparent; }
  .proj-intro a:hover { border-bottom-color:var(--accent); }

  .proj-list { display:flex; flex-direction:column; gap:20px; }
  .proj-card { border:1px solid var(--rule); border-radius:8px; padding:24px 26px; background:var(--panel); transition: border-color .15s, transform .15s; }
  .proj-card:hover { border-color:var(--ink); transform:translateY(-1px); }
  .proj-card .top { display:flex; justify-content:space-between; align-items:baseline; flex-wrap:wrap; gap:10px; margin-bottom:8px; }
  .proj-card .kind { font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.15em; text-transform:uppercase; color:var(--accent); font-weight:600; }
  .proj-card .status { font-family:'JetBrains Mono', monospace; font-size:11px; letter-spacing:0.12em; text-transform:uppercase; color:var(--muted); padding:3px 9px; border:1px solid var(--rule); border-radius:999px; background:var(--soft); }
  .proj-card h3 { font-family:'Source Serif 4', serif; font-size:24px; font-weight:600; margin:0 0 10px; line-height:1.3; color:var(--ink); }
  .proj-card .summary { font-size:16px; line-height:1.65; color:var(--ink); margin:0 0 14px; }
  .proj-card .result { font-size:15px; color:var(--muted); margin:0 0 14px; line-height:1.6; }
  .proj-card .result strong { color:var(--ink); font-weight:600; }
  .proj-card .evidence { list-style:none; padding:0; margin:14px 0 0; display:grid; gap:7px; }
  .proj-card .evidence li { font-size:14.5px; color:var(--muted); line-height:1.55; padding-left:12px; border-left:2px solid var(--rule); }
  .proj-card .evidence strong { color:var(--ink); font-weight:600; }
  .proj-card .stack { display:flex; flex-wrap:wrap; gap:6px; margin-top:14px; }
  .proj-card .chip { font-size:12px; padding:4px 9px; background:var(--soft); border-radius:999px; color:var(--ink); font-family:'Inter', sans-serif; }

  .proj-foot { margin-top:48px; padding-top:24px; border-top:1px solid var(--rule); color:var(--muted); font-size:15px; }
  .proj-foot a { color:var(--accent); text-decoration:none; border-bottom:1px solid transparent; }
  .proj-foot a:hover { border-bottom-color:var(--accent); }

  @media (max-width:640px){
    .proj-h1 { font-size:34px; }
    .proj-card { padding:20px; }
  }
</style>

<div class="proj-head">
  <h1 class="proj-h1">Research + Applied Projects</h1>
  <p class="proj-intro">Current work in turbulence, non-equilibrium phase transitions, and complexity-stability, followed by selected applied modeling projects. This is the bridge between the academic research page and the more implementation-focused resume.</p>
  <p class="proj-intro" style="margin:0;"><a href="{{ '/publications/' | relative_url }}">See Research</a> for papers and project pages; <a href="{{ '/files/Guru_Jayasingh_Resume.pdf' | relative_url }}">download the resume</a> for the compact applied version.</p>
</div>

<div class="proj-list">

  <div class="proj-card">
    <div class="top">
      <span class="kind">Statistical Physics · Turbulence</span>
      <span class="status">Published + ongoing</span>
    </div>
    <h3>Tricritical Directed Percolation in Transitional Turbulence</h3>
    <p class="summary">Research on how pipe flow transitions from laminar to turbulent when body forces are applied. The work identifies a tricritical directed-percolation point that enriches the phase diagram of transitional turbulence.</p>
    <p class="result"><strong>Result:</strong> published in <em>Physical Review Letters</em> 135, 104001 (2025), with UC San Diego news coverage. The project connects fluid mechanics with non-equilibrium phase transitions and universal scaling near turbulent onset.</p>
    <ul class="evidence">
      <li><strong>Physics:</strong> laminar-turbulent transition, body-forced shear flow, directed percolation, tricritical scaling.</li>
      <li><strong>Methods:</strong> finite-size scaling, stochastic modeling, phase-transition phenomenology, statistical inference.</li>
      <li><strong>Why it matters:</strong> gives a compact universality-class explanation for transition behavior that previously looked inconsistent across forcing regimes.</li>
    </ul>
    <div class="stack">
      <span class="chip">Turbulence</span><span class="chip">Directed Percolation</span><span class="chip">Finite-Size Scaling</span><span class="chip">Statistical Mechanics</span><span class="chip">PRL 2025</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">Complex Systems · Random Matrix Theory</span>
      <span class="status">In preparation</span>
    </div>
    <h3>May's Complexity-Stability Hypothesis in Neural Networks</h3>
    <p class="summary">Project asking whether optimized neural networks behave like random complex systems, or whether training produces stabilizing structure analogous to evolved ecological networks.</p>
    <p class="result"><strong>Goal:</strong> test whether gradient descent and selection pressure can move high-dimensional interaction systems away from the random-matrix instability predicted by May's theorem.</p>
    <ul class="evidence">
      <li><strong>Physics/math:</strong> random matrix stability, optimized interaction systems, complex networks, dynamical stability.</li>
      <li><strong>Methods:</strong> spectral analysis, trained-network diagnostics, interaction-structure statistics, comparison to ecological stability mechanisms.</li>
      <li><strong>Why it matters:</strong> reframes neural networks as optimized complex systems whose stability may be governed by statistical-physics structure, not only architecture or loss curves.</li>
    </ul>
    <div class="stack">
      <span class="chip">Complexity-Stability</span><span class="chip">Random Matrix Theory</span><span class="chip">Neural Networks</span><span class="chip">Spectral Analysis</span><span class="chip">Complex Systems</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">Geophysical Turbulence · Universality</span>
      <span class="status">In preparation</span>
    </div>
    <h3>Universality Class of Stratified Shear-Flow Transitions</h3>
    <p class="summary">Project on whether stable density stratification is a relevant perturbation to directed-percolation universality at turbulent onset in shear flows.</p>
    <p class="result"><strong>Goal:</strong> use finite-size scaling and Binder cumulants to separate finite-domain artifacts from genuine stratification-induced changes to critical behavior.</p>
    <ul class="evidence">
      <li><strong>Physics:</strong> stratified Waleffe flow, geophysical shear turbulence, laminar-turbulent onset, directed-percolation scaling.</li>
      <li><strong>Methods:</strong> large-domain simulation constraints, finite-size scaling, Binder cumulants, universality-class diagnostics.</li>
      <li><strong>Why it matters:</strong> connects fundamental turbulence transition theory to stratified flows relevant to oceans, thermoclines, and atmospheric boundary layers.</li>
    </ul>
    <div class="stack">
      <span class="chip">Stratified Turbulence</span><span class="chip">Universality</span><span class="chip">Binder Cumulants</span><span class="chip">Finite-Size Scaling</span><span class="chip">Geophysical Flow</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">ML · Sensor Physics</span>
      <span class="status">Case study in progress</span>
    </div>
    <h3>Structural Health Monitoring from Sensor Time Series</h3>
    <p class="summary">End-to-end pipeline on a <strong>34.8M-entry</strong> multi-sensor dataset to detect structural damage in buildings. Multivariate LSTM predicts 4-floor acceleration response from excitation input; prediction residuals serve as damage signal.</p>
    <p class="result"><strong>Result:</strong> test MSE 0.00278; on heavily damaged state error rose to MSE 0.0347 (~12.5× separation), enabling clean anomaly classification. Welch PSD / FFT feature engineering + multinomial classifier achieved <strong>85.29% accuracy across 17 structural states</strong>.</p>
    <ul class="evidence">
      <li><strong>Physics/data:</strong> vibration response, excitation forcing, and frequency-domain damage signatures.</li>
      <li><strong>ML role:</strong> forecast healthy dynamics, then use residuals and spectral features as damage signals.</li>
      <li><strong>Recruiting signal:</strong> large time-series pipeline, model evaluation, and interpretable anomaly separation.</li>
    </ul>
    <div class="stack">
      <span class="chip">Python</span><span class="chip">PyTorch (LSTM)</span><span class="chip">scikit-learn</span><span class="chip">SciPy (Welch PSD/FFT)</span><span class="chip">NumPy</span><span class="chip">Pandas</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">ML · Graph-RNN · Hackathon</span>
      <span class="status">Case study in progress</span>
    </div>
    <h3>Graph-RNN for High-Dimensional ECG Forecasting</h3>
    <p class="summary">NSF HDR ML hackathon ($4k prize pool). Forecasts ECG signals from multi-channel neural activity. 3-layer GRU + graph convolutions with scheduled sampling; tackles out-of-distribution generalization from session-to-session distribution shift.</p>
    <p class="result"><strong>Result:</strong> in-distribution MSE 32,925 with <strong>R² = 0.80</strong>; beat ARIMA/ETS baselines; currently <strong>17th on global leaderboard</strong>.</p>
    <ul class="evidence">
      <li><strong>Physics/data:</strong> high-dimensional coupled physiological time series with session-level distribution shift.</li>
      <li><strong>ML role:</strong> recurrent forecasting with graph structure and scheduled sampling for stable rollouts.</li>
      <li><strong>Recruiting signal:</strong> fast modeling under leaderboard constraints, baseline comparison, and generalization testing.</li>
    </ul>
    <div class="stack">
      <span class="chip">Python</span><span class="chip">PyTorch (GRU)</span><span class="chip">Graph Convolutions</span><span class="chip">NumPy</span><span class="chip">Pandas</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">Data Science · Housing Economics</span>
      <span class="status">Resume project</span>
    </div>
    <h3>Golden Handcuffs: Mortgage Rate Lock-In and Housing Supply</h3>
    <p class="summary">Automated macroeconomic modeling pipeline to quantify how mortgage rate lock-in affects housing supply. Pulled <strong>24 FRED macroeconomic series</strong> and assembled a <strong>67-variable national/state-level panel dataset</strong> for forecasting and state-level segmentation.</p>
    <p class="result"><strong>Result:</strong> XGBoost outperformed SARIMAX by <strong>30%+ on national RMSE</strong> and <strong>70%+ at the state level</strong>. The project found that lock-in effects are amplified by weak labor markets, while industry structure shapes listing volumes nonlinearly in ways tree-based models detect but SARIMAX misses.</p>
    <ul class="evidence">
      <li><strong>Data:</strong> FRED API macro series, national housing indicators, and state-level economic panels.</li>
      <li><strong>ML role:</strong> PCA, LASSO, and K-means to identify latent macro structure; XGBoost and SHAP for nonlinear forecasting and interpretability.</li>
      <li><strong>Recruiting signal:</strong> automated data ingestion, panel-data feature engineering, econometric baselines, model comparison, and interpretable ML.</li>
    </ul>
    <div class="stack">
      <span class="chip">Python</span><span class="chip">FRED API</span><span class="chip">XGBoost</span><span class="chip">SHAP</span><span class="chip">scikit-learn</span><span class="chip">statsmodels</span><span class="chip">Pandas</span><span class="chip">Matplotlib</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="top">
      <span class="kind">Physics-Informed ML · Accelerator</span>
      <span class="status">Starting Summer 2026</span>
    </div>
    <h3>Physics-Informed ML for Laser-Plasma Accelerators</h3>
    <p class="summary">AI/ML Intern at <a href="https://www.tausystems.com" style="color:var(--accent); text-decoration:none;">TAU Systems</a> (Carlsbad). Surrogate modeling and physics-informed prediction for electron-bunch properties from laser/plasma parameters. Sanitized writeup will follow after the internship.</p>
    <ul class="evidence">
      <li><strong>Physics/data:</strong> laser-plasma accelerator inputs and electron-bunch output properties.</li>
      <li><strong>ML role:</strong> physics-informed prediction and surrogate modeling for expensive experimental/simulation regimes.</li>
      <li><strong>Recruiting signal:</strong> direct fit for scientific ML, accelerator physics, and hardware-adjacent AI roles.</li>
    </ul>
    <div class="stack">
      <span class="chip">Python</span><span class="chip">PyTorch</span><span class="chip">Physics-informed ML</span><span class="chip">Surrogate modeling</span>
    </div>
  </div>

</div>

<div class="proj-foot">
  For research publications and academic work, see <a href="{{ '/publications/' | relative_url }}">Research</a> or download the <a href="{{ '/files/Guru_Jayasingh_CV.pdf' | relative_url }}">Academic CV</a>.
</div>
