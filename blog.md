---
layout: page
title: Hi! I'm Shopon
subtitle: Programmer | Artificial Intelligence Enthusiast
use-site-title: true
bigimg: '/img/home.gif'
---

<ul >
    {% for post in site.posts limit 4 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
        {{ post.content | strip_html | truncatewords:75}}<br>
            <a href="{{ post.url }}">Read more...</a><br><br>
    {% endfor %}
</ul>