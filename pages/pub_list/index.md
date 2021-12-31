---
layout: default
title: Publication List
abstract: Listed all contributed publications
permalink: /pub_list/
---

<ul>
{% for entry in site.data.papers.entries %}
  <li>
    {% for x in entry %}
      {{ x.title }}
    {% endfor %}
  </li>
{% endfor %}
</ul>