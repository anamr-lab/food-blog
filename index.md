---
layout: default
title: "Mi blog de recetas"
---

<style>
  body {
    font-family: Arial, sans-serif;
    background: #f6f6f6;
  }

  .container {
    max-width: 700px;
    margin: 40px auto;
    background: white;
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.08);
  }

  h1 {
    text-align: center;
  }

  ul {
    padding: 0;
    list-style: none;
  }

  li {
    padding: 12px 0;
    border-bottom: 1px solid #eee;
  }

  a {
    text-decoration: none;
    font-size: 18px;
    color: #007acc;
  }
</style>

<div class="container">

# 🍳 Recetas

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

</div>
