---
layout: default
title: Recent Articles
permalink: /recent/
---
{% include home-header.html %}
<h1>Recent Articles</h1>

{% assign articles = site.posts | where_exp: "p", "p.path contains '_posts/articles/'" %}

{% assign first_tags = "" | split: "" %}
{% for post in articles %}
  {% assign first_tag = post.tags[0] %}
  {% unless first_tags contains first_tag %}
    {% assign first_tags = first_tags | push: first_tag %}
  {% endunless %}
{% endfor %}

{% for tag in first_tags %}
  <h2>{{ tag }}</h2>
  <ul>
  {% for post in articles %}
    {% if post.tags[0] == tag %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      — {{ post.date | date: "%Y-%m-%d" }}
    </li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
