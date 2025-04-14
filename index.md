---
layout: default
title: Início
---


## 📝 Postagens recentes

<div class="card-grid">
  {% for post in site.posts %}
    <div class="post-card">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="post-date">{{ post.date | date: "%d/%m/%Y" }}</p>
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 120 }}</p>
      <a class="read-more" href="{{ post.url | relative_url }}">Ler mais →</a>
    </div>
  {% endfor %}
</div>
