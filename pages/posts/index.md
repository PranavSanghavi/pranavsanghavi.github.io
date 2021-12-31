---
layout: default
title: Posts
abstract: Listed below are some of my posted ramblings
permalink: /posts/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date | date: "%d %B %Y" }}
    </li>
  {% endfor %}
</ul>