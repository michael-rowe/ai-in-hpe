---
layout: default
title: News
---

# News

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    <p>{{ post.description }}</p> <!-- Display the description -->
    <span>{{ post.date | date_to_string }}</span>
  </li>
{% endfor %}
</ul>
