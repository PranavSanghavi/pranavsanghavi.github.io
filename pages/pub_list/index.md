---
layout: default
title: Publication List
author: Pranav Sanghavi
abstract: Listed below are all contributed publications
date: 2020-12-31
permalink: /pub_list/
---

<ul>
{% for entry in site.data.pubs.papers.entries %}
    {% for x in entry %}
        {% if x.url %}
            <b><a href="{{ x.url }}">{{ x.title }}</a></b><br /> 
        {% else %}
            <b>{{ x.title }}</b><br /> 
        {% endif %}
            {% for author in x.author %}
                {% if author.first == "Pranav" and author.last == "Sanghavi" %}
                    <b>{{ author.first }} {{ author.last }}</b>, 
                {% elsif author.first == "P." and author.last == "Sanghavi" %}
                    <b>{{ author.first }} {{ author.last }}</b>,
                {% else %}
                    {{ author.first }} {{ author.last }},
                {% endif %}
            {% endfor %} <i> {{ x.journal }}{{ x.booktitle}} </i> {{ x.year }}<br /> 
    {% endfor %}
{% endfor %}
</ul>
