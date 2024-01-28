---
layout: page
title: Blog
permalink: /blog/
---
<link rel="stylesheet" href="/assets/math.css">
I basically talk about **things**.
<ul class="post-ul">
{% for post in site.posts  %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      <p>{{ post.date | date: "%d %B %Y"}}</p>
{% endfor %}
</ul>