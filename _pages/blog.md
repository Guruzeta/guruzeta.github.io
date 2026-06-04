---
layout: archive
title: "Blog"
subtitle: "Working notes and plain-language explanations on statistical mechanics, turbulence, and ML theory."
eyebrow: "Writing"
permalink: /blog/
author_profile: false
---

{% include base_path %}

{% if site.posts.size == 0 %}
  <p style="color:var(--muted);">No posts yet — first one coming soon.</p>
{% else %}
<ul class="v3-list">
{% for post in site.posts %}
  <li>
    <div class="v3-meta">{{ post.date | date: "%b %d, %Y" }}{% if post.tags.size > 0 %} · {{ post.tags | join: ", " }}{% endif %}</div>
    <div class="v3-title">
      <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
    </div>
    {% if post.excerpt %}
      <div class="v3-blurb">{{ post.excerpt | markdownify | strip_html | strip_newlines }}</div>
    {% endif %}
    <div class="v3-actions"><a href="{{ base_path }}{{ post.url }}">Read →</a></div>
  </li>
{% endfor %}
</ul>
{% endif %}

<p style="margin-top:32px; color:var(--muted); font-size:13px;">
RSS: <a href="{{ base_path }}/feed.xml">feed.xml</a>
</p>
