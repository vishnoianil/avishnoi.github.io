---
layout: default
title: Blog
permalink: /blog/
---
<div>
  <article class="post">
    <h2 class="post-title" style="text-align: center;color:#1a426d"> <b>Blog</b> </h2>
  </article>

  {% for blog in site.categories.blog %}
  {% assign post_url = paper.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url %}

  <article class="post">
    <h2 class="post-title">
      <a href="{{ blog.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url}}#disqus_thread">
        {{ blog.title }}
      </a>
    </h2>

    <p class="post-meta">
        <span class="post-meta">
            {{ blog.date | date: "%b %-d, %Y" }}
            {% if blog.tags %} • {{ blog.tags }}{% endif %}
            {% if blog.meta %} • {{ blog.meta }}{% endif %}
        </span>
    </p>

    {{ blog.excerpt }}
    <a href="{{ blog.url | replace: '//', '/' | prepend: site.baseurl | prepend: site.url }}">
      Continue reading »
    </a>
  </article>
  {% endfor %}
  </div>
