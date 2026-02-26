---
layout: default
title: Recent Articles
permalink: /recent/
---
<h1>Recent Articles</h1>

<ul>
{% assign articles = site.posts | where_exp: "p", "p.path contains '_posts/articles/'" %}
{% for post in articles %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    — {{ post.date | date: "%Y-%m-%d" }}
  </li>
{% endfor %}
</ul>