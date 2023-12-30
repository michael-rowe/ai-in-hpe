---
layout: default
title: News
---

# News

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> <span>{{ post.date | date_to_string }}</span>
    <p>{{ post.description }}</p> <!-- Display the description -->
  </li>
{% endfor %}
</ul>
