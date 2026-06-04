---
layout: site
permalink: /cv/
title: "Curriculum Vitae"
sitemap: true
---
{% include base_path %}
<style>
  .cv2-wrap { max-width:1100px; margin:0 auto; padding:48px 32px 96px; display:grid; grid-template-columns:260px 1fr; gap:48px; font-family:'Inter', sans-serif; color:#1a1a1a; }
  .cv2-side { position:sticky; top:80px; align-self:start; }
  .cv2-side h1 { font-family:'Source Serif 4', serif; font-size:26px; margin:0 0 6px; letter-spacing:-0.01em; }
  .cv2-side p.sub { color:#666; font-size:14px; margin:0 0 16px; }
  .cv2-side .ctas { display:flex; flex-direction:column; gap:8px; margin-bottom:18px; }
  .cv2-side .ctas a { padding:8px 12px; border:1px solid #ddd; border-radius:6px; text-decoration:none; font-size:13px; color:#1a1a1a; font-weight:500; }
  .cv2-side .ctas a.primary { background:#1a1a1a; color:#fff; border-color:#1a1a1a; }
  .cv2-side nav.toc a { display:block; padding:6px 0; font-size:13px; color:#666; text-decoration:none; border-left:2px solid transparent; padding-left:10px; }
  .cv2-side nav.toc a:hover { color:#1a1a1a; border-left-color:var(--accent); }
  .cv2-main section { padding:24px 0; border-bottom:1px solid #eee; }
  .cv2-main section:last-of-type { border-bottom:0; }
  .cv2-main h2 { font-family:'Source Serif 4', serif; font-size:22px; font-weight:600; margin:0 0 14px; letter-spacing:-0.01em; }
  .cv2-main [data-role] { padding:10px 0; }
  .cv2-main [data-role] header { display:flex; flex-wrap:wrap; gap:6px 14px; align-items:baseline; margin-bottom:4px; font-size:15px; }
  .cv2-main [data-role] header .when { margin-left:auto; font-family:'JetBrains Mono', monospace; font-size:12px; color:#888; }
  .cv2-main ul { margin:6px 0; padding-left:20px; font-size:14.5px; color:#333; line-height:1.6; }
  .cv2-main a { color:var(--accent); text-decoration:none; }
  .cv2-main .cv-updated { color:#888; font-size:13px; margin-top:24px; }
  @media (max-width:880px){ .cv2-wrap{grid-template-columns:1fr;} .cv2-side{position:static;} }
</style>
<div class="cv2-wrap">
  <aside class="cv2-side">
    <h1>Guru Kalyan Jayasingh</h1>
    <p class="sub">Ph.D. Candidate, Theoretical Physics · UC San Diego</p>
    <div class="ctas">
      <a class="primary" href="{{ base_path }}/files/Guru_K_Jayasingh_CV_Nov_2025.pdf">Download PDF</a>
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
