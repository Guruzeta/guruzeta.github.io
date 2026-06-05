---
layout: archive
title: "Blog"
subtitle: "Working notes and plain-language explanations on statistical mechanics, turbulence, and complex systems."
eyebrow: "Writing"
permalink: /blog/
author_profile: false
---

{% if site.posts.size == 0 %}
  <p style="color:var(--muted);">No posts yet — first one coming soon.</p>
{% else %}
<ul class="v3-list">
{% for post in site.posts %}
  <li>
    <div class="v3-meta">{{ post.date | date: "%b %d, %Y" }}{% if post.tags.size > 0 %} · {{ post.tags | join: ", " }}{% endif %}</div>
    <div class="v3-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </div>
    {% if post.excerpt %}
      <div class="v3-blurb">{{ post.excerpt | markdownify | strip_html | strip_newlines }}</div>
    {% endif %}
    <div class="v3-actions"><a href="{{ post.url | relative_url }}">Read →</a></div>
  </li>
{% endfor %}
</ul>
{% endif %}

<p style="margin-top:32px; color:var(--muted); font-size:14px;">
RSS: <a href="{{ '/feed.xml' | relative_url }}">feed.xml</a>
</p>
