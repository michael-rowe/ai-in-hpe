---
layout: post
title: Stream
---

# Feed

<ul>
{% for post in site.stream %}
  <li>
    <strong><a href="{{ post.source }}">{{ post.title }}</a></strong> ({{ post.author }}): {{ post.description }}
  </li>
{% endfor %}
</ul>
