---
layout: archive
title: "Research"
subtitle: "Published work, preprints, and projects-in-progress on statistical mechanics, turbulence, and machine-learning theory."
eyebrow: "Publications"
permalink: /publications/
author_profile: false
---

{% include base_path %}

<ul class="v3-list">
{% for post in site.publications reversed %}
  <li>
    <div class="v3-meta">
      {% if post.venue %}{{ post.venue }}{% endif %}{% if post.date %} · {{ post.date | date: "%Y" }}{% endif %}
    </div>
    <div class="v3-title">
      <a href="{{ base_path }}{{ post.url }}">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</a>
    </div>
    {% if post.excerpt %}
      <div class="v3-blurb">{{ post.excerpt | markdownify | strip_html | strip_newlines }}</div>
    {% endif %}
    <div class="v3-actions">
      <a href="{{ base_path }}{{ post.url }}">Details</a>
      {% if post.paperurl %}<a href="{{ post.paperurl }}">Paper</a>{% endif %}

      {% comment %} per-paper extras {% endcomment %}
      {% if post.url contains "tricritical-dp-body-force" %}
        <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>
        <a href="https://chatgpt.com/g/g-68e699d7b85881918b87e4fae3b4f8c9-tricritical-dp-in-laminar-turbulent-transition">Chat with the paper (GPT)</a>
      {% endif %}
    </div>
  </li>
{% endfor %}
</ul>

<p style="margin-top:32px; color:var(--muted); font-size:14px;">
For collaboration or reprint requests, email <a href="mailto:gjayasingh@ucsd.edu">gjayasingh@ucsd.edu</a>.
</p>
