---
layout: page
title: Work
permalink: /work/
---

{% for post in site.categories.portfolio %}
  <div class="project-info">
    <a href="{{ post.url | relative_url }}">
      <div class="project-background"></div>
      <div class="project-image"><img src="{{ post.image }}"></div>
      <h1><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h1>
    </a>
  </div>
{% endfor %}
