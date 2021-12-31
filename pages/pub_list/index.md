---
layout: default
title: Publication List
abstract: Listed all contributed publications
permalink: /pub_list/
---

<ul>
{% for paper in site.data.papers.entries %}
  <li>
      {{ paper.title }}
  </li>
{% endfor %}
</ul>