---
layout: default
title: "Mi blog de recetas"
---

# 🍳 Recetas

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
