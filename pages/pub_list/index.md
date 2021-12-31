---
layout: default
title: Publication List
abstract: Listed all contributed publications
permalink: /pub_list/
---

<ul>
{% for entry in site.data.papers.entries %}
    {% for x in entry %}
        <b> {{ x.title }} </b> in <i> {{ x.journal }} </i> {{ x.year }}<br />
            {% for author in x.author %}
                {{ author.first }} {{ author.last }}
            {% endfor %} <br /> 
    {% endfor %}
{% endfor %}
</ul>