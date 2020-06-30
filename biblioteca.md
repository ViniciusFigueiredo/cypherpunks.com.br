---
layout: page
title: Biblioteca
permalink: /Biblioteca/
---

<ul>
  <!-- {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %} -->

  {% assign sorted-posts = site.posts | sort: 'title' %}
{% for post in sorted-posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>