---
layout: default
title: Publication List
abstract: Listed all contributed publications
permalink: /pub_list/
---

<ul>
{% for entry in site.data.papers.entries %}
    {% for x in entry %}
        {% if x.url %}
            <b><a href="{{ x.url }}">{{ x.title }}</a></b>
        {% else %}
            <b>{{ x.title }}</b>
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