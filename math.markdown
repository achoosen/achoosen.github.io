---
layout: page
title: Math
permalink: /math/
---

A compilation of the maths I've done, what I find interesting and enjoy.

<link rel="stylesheet" href="/assets/math.css">

<html>
{% assign this_word = "math" %}
  {% for post in site.categories[this_word]%} 
    {% if post.url %}
    <ul>
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
        <p>{{post.description}}</p> 
    </ul>
    {% endif %}
{% endfor %}

</html>