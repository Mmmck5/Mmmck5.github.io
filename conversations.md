---
layout: default
title: Conversations
permalink: /conversations/
---
{% include home-header.html %}
<h1>Conversations</h1>

<ul>
{% assign posts = site.posts | where_exp: "p", "p.tags contains 'conversations'" %}
{% for post in posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    — {{ post.date | date: "%Y-%m-%d" }}
  </li>
{% endfor %}
</ul>
