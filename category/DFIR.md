---
layout: category
category: DFIR
title: DFIR
permalink: /category/DFIR/
---


<h1>DFIR Posts</h1>

<ul>
  {% for post in site.categories.cybersecurity %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
