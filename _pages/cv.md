---
layout: site
permalink: /cv/
title: "Academic CV"
sitemap: true
---
<style>
  .cv2-wrap { margin:0; padding:0 0 72px; font-family:'Inter', sans-serif; color:var(--ink); }

  .cv2-head { margin-bottom:8px; }
  .cv2-head h1 { font-family:'Source Serif 4', serif; font-size:40px; font-weight:600; margin:0 0 8px; letter-spacing:0; }
  .cv2-head .sub { color:var(--muted); font-size:16px; margin:0 0 4px; line-height:1.6; }
  .cv2-head .sub a { color:var(--accent); text-decoration:none; }
  .cv2-head .sub a:hover { text-decoration:underline; }
  .cv2-ctas { display:flex; flex-wrap:wrap; gap:9px; margin:20px 0 4px; }
  .cv2-ctas a {
    padding:9px 15px; border:1px solid var(--rule); border-radius:7px; text-decoration:none;
    font-size:14px; color:var(--ink); background:var(--paper); font-weight:500;
    transition: border-color .15s, transform .15s;
  }
  .cv2-ctas a:hover { border-color:var(--ink); transform:translateY(-1px); }
  .cv2-ctas a.primary { background:var(--ink); color:var(--on-ink); border-color:var(--ink); }

  /* jump bar */
  .cv2-toc { display:flex; flex-wrap:wrap; gap:6px 8px; margin:26px 0 0; padding:16px 0 0; border-top:1px solid var(--rule); }
  .cv2-toc a {
    font-family:'JetBrains Mono', monospace; font-size:11px; letter-spacing:0.1em; text-transform:uppercase;
    color:var(--muted); text-decoration:none; padding:5px 10px; border-radius:999px; background:var(--soft);
    transition: color .15s, background .15s;
  }
  .cv2-toc a:hover { color:var(--ink); }

  .cv2-main section { padding:34px 0; border-bottom:1px solid var(--rule); scroll-margin-top:24px; }
  .cv2-main section:last-of-type { border-bottom:0; }
  .cv2-main h2 {
    font-family:'JetBrains Mono', monospace; font-size:12px; font-weight:500;
    letter-spacing:0.18em; text-transform:uppercase; color:var(--muted); margin:0 0 18px;
  }
  .cv2-main [data-role] { padding:0 0 22px; }
  .cv2-main [data-role]:last-child { padding-bottom:0; }

  /* header: title left, date right — no flex gap next to punctuation */
  .cv2-main [data-role] header {
    display:flex; justify-content:space-between; align-items:baseline; gap:20px;
    margin-bottom:3px; font-size:16.5px; line-height:1.45;
  }
  .cv2-main [data-role] header .what { flex:1 1 auto; }
  .cv2-main [data-role] header .what strong { font-weight:600; }
  .cv2-main [data-role] header .what em { font-style:normal; color:var(--muted); }
  .cv2-main [data-role] header .when {
    flex:none; font-family:'JetBrains Mono', monospace; font-size:12.5px;
    color:var(--muted); white-space:nowrap;
  }

  .cv2-main .cv-proj { color:var(--ink); font-size:15px; margin:2px 0 6px; line-height:1.6; }
  .cv2-main .cv-venue { color:var(--muted); font-size:14px; margin:2px 0 6px; line-height:1.55; }
  .cv2-main p { color:var(--ink); font-size:15.5px; line-height:1.65; margin:4px 0; }
  .cv2-main ul { margin:6px 0; padding-left:19px; font-size:15.5px; color:var(--ink); line-height:1.68; }
  .cv2-main ul li { margin-bottom:3px; }
  .cv2-main a { color:var(--accent); text-decoration:none; }
  .cv2-main a:hover { text-decoration:underline; }
  .cv2-main .cv-updated { color:var(--muted); font-size:14px; margin-top:28px; }

  /* education rows with logos */
  .cv2-main .cv-edu { display:grid; grid-template-columns:44px 1fr; gap:16px; align-items:start; }
  .cv2-main .cv-logo-img {
    width:44px; height:44px; border-radius:9px; object-fit:contain;
    background:#fff; border:1px solid var(--rule); padding:4px;
  }

  @media (max-width:640px){
    .cv2-head h1 { font-size:32px; }
    .cv2-main [data-role] header { flex-direction:column; gap:2px; }
    .cv2-main .cv-edu { grid-template-columns:36px 1fr; gap:12px; }
    .cv2-main .cv-logo-img { width:36px; height:36px; }
  }
</style>

<div class="cv2-wrap">
  <header class="cv2-head">
    <h1>Academic CV</h1>
    <p class="sub">
      Guru Kalyan Jayasingh · Physics Ph.D. Candidate, UC San Diego<br>
      <a href="mailto:gjayasingh@ucsd.edu">gjayasingh@ucsd.edu</a> · Department of Physics, 9500 Gilman Drive, La Jolla CA 92093
    </p>
    <div class="cv2-ctas">
      <a class="primary" href="{{ '/files/Guru_Jayasingh_CV.pdf' | relative_url }}">Download Academic CV</a>
      <a href="{{ '/files/Guru_Jayasingh_Resume.pdf' | relative_url }}">Industry Resume</a>
    </div>
    <nav class="cv2-toc">
      <a href="#education">Education</a>
      <a href="#experience">Positions</a>
      <a href="#publications">Publications</a>
      <a href="#talks">Talks</a>
      <a href="#teaching">Teaching</a>
      <a href="#honors">Honors</a>
      <a href="#skills">Skills</a>
      <a href="#leadership">Outreach</a>
    </nav>
  </header>

  <div class="cv2-main">
    {% capture cv %}{% include cv-content.html %}{% endcapture %}
    {{ cv
      | replace: 'data-cv="interests"',     'id="interests" data-cv="interests"'
      | replace: 'data-cv="education"',     'id="education" data-cv="education"'
      | replace: 'data-cv="experience"',    'id="experience" data-cv="experience"'
      | replace: 'data-cv="publications"',  'id="publications" data-cv="publications"'
      | replace: 'data-cv="talks"',         'id="talks" data-cv="talks"'
      | replace: 'data-cv="teaching"',      'id="teaching" data-cv="teaching"'
      | replace: 'data-cv="honors"',        'id="honors" data-cv="honors"'
      | replace: 'data-cv="skills"',        'id="skills" data-cv="skills"'
      | replace: 'data-cv="leadership"',    'id="leadership" data-cv="leadership"'
    }}
  </div>
</div>
