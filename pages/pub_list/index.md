---
layout: default
title: Publication List
abstract: Listed all contributed publications
permalink: /pub_list/
---

<ul>
{% for entry in site.data.papers.entries %}
    {% for x in entry %}
        {{ x.title }}
            {% for author in x.author %}
                {{ author.first }} {{ author.last }}
            {% endfor %}   
    {% endfor %}
{% endfor %}
</ul>