---
layout: default
title: Research Papers
permalink: /papers/
---
<div>
  <article class="post">
    <h2 class="post-title" style="text-align: center;color:#1a426d"> <b>Research Papers</b> </h2>
  </article>

  {% for paper in site.categories.papers %}
  {% assign post_url = paper.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url %}

  <article class="post">
    <h2 class="post-title">
      <a href="{{ paper.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url}}#disqus_thread">
        {{ paper.title }}
      </a>
    </h2>

    <p class="post-meta">
        <span class="post-meta">
            {{ paper.date | date: "%b %-d, %Y" }}
            {% if paper.tags %} • {{ paper.tags }}{% endif %}
            {% if paper.meta %} • {{ paper.meta }}{% endif %}
        </span>
    </p>

    {{ paper.excerpt }}
    <a href="{{ paper.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url }}">
      Continue reading »
    </a>
  </article>
  {% endfor %}
