---
layout: post
title: News
---

# News

 You can bookmark this page or subscribe to the [RSS feed](./feed.xml) in a newsreader.
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> (<span>{{ post.date | date_to_string }}</span>): {{ post.description }}
  </li>
{% endfor %}
</ul>
