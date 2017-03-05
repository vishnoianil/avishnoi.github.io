---
layout: default
title: Patents
permalink: /patents/
---
<div>
  <article class="post">
    <h2 class="post-title" style="text-align: center;color:#1a426d"> <b>Patents</b> </h2>
  </article>

  {% for patent in site.categories.patents %}
  {% assign post_url = patent.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url %}

  <article class="post">
    <h1 class="post-title">
      <a href="{{ patent.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url}}#disqus_thread">
        {{ patent.title }}
      </a>
    </h1>
    <p class="post-meta">
        <span class="post-meta">
            {{ patent.date | date: "%b %-d, %Y" }}
            {% if patent.tags %} • {{ patent.tags }}{% endif %}
            {% if patent.meta %} • {{ patent.meta }}{% endif %}
        </span>
    </p>

    {{ patent.excerpt }}
    <a href="{{ patent.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url }}">
      Continue reading »
    </a>
  </article>
  {% endfor %}
