---
layout: page
title:
permalink: /archive/
---

<div>
  <article class="post">
    <h2 class="post-title" style="text-align: center;color:#1a426d"> <b>Archived Posts</b> </h2>
  </article>

  {% for post in site.posts %}
    {% capture currentyear %}{{post.date | date: "%Y"}}{% endcapture %}
    {% if currentyear != year %}
      {% unless forloop.first %}
      </ul>
      {% endunless %}
      <h5>{{ currentyear }}</h5>
      <ul>
      {% capture year %}{{currentyear}}{% endcapture %}
    {% endif %}
    <li><b>[{{post.type}}] </b><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
  {% endfor %}
