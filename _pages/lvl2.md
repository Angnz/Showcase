---
permalink: /lvl2/
layout: page
title: "LVL2: BOB"
---


<ul>
    {% for post in site.posts %}
      {% if post.categories contains 'lvl2' %}
        <li><a href="{{ post.url }}">{{ post.categories }} - {{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
</ul>