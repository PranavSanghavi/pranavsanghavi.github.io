---
layout: default
title: List of Posts 
permalink: /posts/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date | date: "%d %B %Y" }}
    </li>
  {% endfor %}
</ul>