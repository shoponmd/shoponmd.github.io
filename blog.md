---
layout: page
title: Hi! I'm Shopon
subtitle: Programmer | Artificial Intelligence Enthusiast
use-site-title: true
bigimg: '/img/home.gif'
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>
