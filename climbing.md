---
layout: default
title: Climbing
permalink: /climbing/
---
<h1>Climbing</h1>

<ul>
{% assign posts = site.posts | where_exp: "p", "p.tags contains 'climbing'" %}
{% for post in posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    — {{ post.date | date: "%Y-%m-%d" }}
  </li>
{% endfor %}
</ul>
