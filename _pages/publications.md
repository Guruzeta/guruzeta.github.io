---
layout: archive
title: "Research"
subtitle: "Published work, preprints, and projects-in-progress on statistical mechanics, turbulence, and complexity-stability."
eyebrow: "Publications"
permalink: /publications/
author_profile: false
---

{% comment %} Published work first (has paperurl), then in-preparation; newest first within each group {% endcomment %}
{% assign by_date = site.publications | sort: "date" | reverse %}
{% assign published = by_date | where_exp: "p", "p.paperurl" %}
{% assign in_prep = by_date | where_exp: "p", "p.paperurl == nil" %}
{% assign ordered = published | concat: in_prep %}

<ul class="v3-list">
{% for post in ordered %}
  <li>
    <div class="v3-meta">
      {% if post.venue %}{{ post.venue }}{% endif %}{% if post.date %} · {{ post.date | date: "%Y" }}{% endif %}
    </div>
    <div class="v3-title">
      <a href="{{ post.url | relative_url }}">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</a>
    </div>
    {% if post.excerpt %}
      <div class="v3-blurb">{{ post.excerpt | markdownify | strip_html | strip_newlines }}</div>
    {% endif %}
    <div class="v3-actions">
      <a href="{{ post.url | relative_url }}">Details</a>
      {% if post.paperurl %}<a href="{{ post.paperurl }}">Paper</a>{% endif %}

      {% comment %} per-paper extras {% endcomment %}
      {% if post.url contains "tricritical-dp-body-force" %}
        <a href="https://today.ucsd.edu/story/turbulence-with-a-twist">UCSD News</a>
      {% endif %}
    </div>
  </li>
{% endfor %}
</ul>

<p style="margin-top:32px; color:var(--muted); font-size:15px;">
For collaboration or reprint requests, email <a href="mailto:gjayasingh@ucsd.edu">gjayasingh@ucsd.edu</a>.
</p>
