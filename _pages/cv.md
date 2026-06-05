---
layout: site
permalink: /cv/
title: "Academic CV"
sitemap: true
---
<style>
  .cv2-wrap { max-width:1100px; margin:0 auto; padding:48px 32px 96px; display:grid; grid-template-columns:260px 1fr; gap:48px; font-family:'Inter', sans-serif; color:var(--ink); }
  .cv2-side { position:sticky; top:80px; align-self:start; }
  .cv2-side h1 { font-family:'Source Serif 4', serif; font-size:28px; margin:0 0 6px; letter-spacing:0; }
  .cv2-side p.sub { color:var(--muted); font-size:15px; margin:0 0 16px; }
  .cv2-side .ctas { display:flex; flex-direction:column; gap:8px; margin-bottom:18px; }
  .cv2-side .ctas a { padding:9px 12px; border:1px solid var(--rule); border-radius:6px; text-decoration:none; font-size:14px; color:var(--ink); background:var(--panel); font-weight:500; }
  .cv2-side .ctas a.primary { background:var(--ink); color:var(--on-ink); border-color:var(--ink); }
  .cv2-side nav.toc a { display:block; padding:6px 0; font-size:14px; color:var(--muted); text-decoration:none; border-left:2px solid transparent; padding-left:10px; }
  .cv2-side nav.toc a:hover { color:var(--ink); border-left-color:var(--accent); }
  .cv2-main section { padding:24px 0; border-bottom:1px solid var(--rule); }
  .cv2-main section:last-of-type { border-bottom:0; }
  .cv2-main h2 { font-family:'Source Serif 4', serif; font-size:24px; font-weight:600; margin:0 0 14px; letter-spacing:0; }
  .cv2-main [data-role] { padding:10px 0; }
  .cv2-main [data-role] header { display:flex; flex-wrap:wrap; gap:6px 14px; align-items:baseline; margin-bottom:4px; font-size:16px; }
  .cv2-main [data-role] header .when { margin-left:auto; font-family:'JetBrains Mono', monospace; font-size:13px; color:var(--muted); }
  .cv2-main p { color:var(--ink); }
  .cv2-main ul { margin:6px 0; padding-left:20px; font-size:15.5px; color:var(--ink); line-height:1.65; }
  .cv2-main a { color:var(--accent); text-decoration:none; }
  .cv2-main .cv-updated { color:var(--muted); font-size:14px; margin-top:24px; }
  .cv2-note { color:var(--muted); font-size:14px; line-height:1.6; margin:0 0 16px; }
  @media (max-width:880px){ .cv2-wrap{grid-template-columns:1fr;} .cv2-side{position:static;} }
</style>
<div class="cv2-wrap">
  <aside class="cv2-side">
    <h1>Academic CV</h1>
    <p class="sub">Guru Kalyan Jayasingh · Physics Ph.D. Candidate, UC San Diego</p>
    <p class="cv2-note">Full academic record: publications, talks, teaching, honors, research appointments, and coursework.</p>
    <div class="ctas">
      <a class="primary" href="{{ '/files/Guru_Jayasingh_CV.pdf' | relative_url }}">Download Academic CV</a>
      <a href="{{ '/files/Guru_Jayasingh_Resume.pdf' | relative_url }}">Industry Resume</a>
      <a href="mailto:gjayasingh@ucsd.edu">Email</a>
    </div>
    <nav class="toc">
      <a href="#position">Present Position</a>
      <a href="#honors">Honors</a>
      <a href="#experience">Experience</a>
      <a href="#publications">Publications</a>
      <a href="#education">Education</a>
      <a href="#research">Research</a>
      <a href="#talks">Talks</a>
      <a href="#teaching">Teaching</a>
      <a href="#skills">Skills</a>
      <a href="#coursework">Coursework</a>
    </nav>
  </aside>

  <div class="cv2-main">
    {% capture cv %}{% include cv-content.html %}{% endcapture %}
    {{ cv
      | replace: 'data-cv="position"',     'id="position" data-cv="position"'
      | replace: 'data-cv="honors"',       'id="honors" data-cv="honors"'
      | replace: 'data-cv="experience"',   'id="experience" data-cv="experience"'
      | replace: 'data-cv="publications"', 'id="publications" data-cv="publications"'
      | replace: 'data-cv="education"',    'id="education" data-cv="education"'
      | replace: 'data-cv="research"',     'id="research" data-cv="research"'
      | replace: 'data-cv="talks"',        'id="talks" data-cv="talks"'
      | replace: 'data-cv="teaching"',     'id="teaching" data-cv="teaching"'
      | replace: 'data-cv="skills"',       'id="skills" data-cv="skills"'
      | replace: 'data-cv="coursework"',   'id="coursework" data-cv="coursework"'
    }}
  </div>
</div>
