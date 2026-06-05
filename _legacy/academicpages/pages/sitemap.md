---
layout: archive
title: "Sitemap"
subtitle: "Current public routes for the rebuilt site shell."
eyebrow: "Site"
permalink: /sitemap/
author_profile: false
---

<ul class="v3-list">
  <li>
    <div class="v3-title"><a href="{{ '/' | relative_url }}">Home</a></div>
    <div class="v3-blurb">Current landing page.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/projects/' | relative_url }}">Projects</a></div>
    <div class="v3-blurb">Applied ML, physics-informed modeling, and computational projects.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/publications/' | relative_url }}">Research</a></div>
    <div class="v3-blurb">Publications and research projects.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/talks/' | relative_url }}">Talks</a></div>
    <div class="v3-blurb">Conference talks and presentations.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/blog/' | relative_url }}">Blog</a></div>
    <div class="v3-blurb">Working notes and explanations.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/teaching/' | relative_url }}">Teaching</a></div>
    <div class="v3-blurb">Teaching assistant roles and courses.</div>
  </li>
  <li>
    <div class="v3-title"><a href="{{ '/cv/' | relative_url }}">Academic CV</a></div>
    <div class="v3-blurb">Academic record and downloadable CV.</div>
  </li>
</ul>

<h2>Research Items</h2>
<ul class="v3-list">
{% for post in site.publications reversed %}
  <li>
    <div class="v3-meta">{% if post.venue %}{{ post.venue }}{% endif %}{% if post.date %} · {{ post.date | date: "%Y" }}{% endif %}</div>
    <div class="v3-title"><a href="{{ post.url | relative_url }}">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</a></div>
  </li>
{% endfor %}
</ul>

<h2>Talks</h2>
<ul class="v3-list">
{% for post in site.talks reversed %}
  <li>
    <div class="v3-meta">{% if post.venue %}{{ post.venue }}{% endif %}{% if post.date %} · {{ post.date | date: "%Y" }}{% endif %}</div>
    <div class="v3-title"><a href="{{ post.url | relative_url }}">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</a></div>
  </li>
{% endfor %}
</ul>

<h2>Blog Posts</h2>
<ul class="v3-list">
{% for post in site.posts %}
  <li>
    <div class="v3-meta">{{ post.date | date: "%b %d, %Y" }}</div>
    <div class="v3-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
  </li>
{% endfor %}
</ul>
