---
layout: page
title: Notes that have become posts.
tagline: so I don't forget them!
---
{% include JB/setup %}

Here's are the latest posts.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>