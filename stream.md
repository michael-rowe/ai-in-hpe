---
layout: default
title: Stream
---

# Feed

<div class="feed-index">
    {% for post in site.posts %}
        <div class="post">
            <h2><a href="{{ post.source }}">{{ post.title }}</a></h2>
            <p><strong>Author:</strong> {{ post.author }}</p>
            <p><strong>Source:</strong> <a href="{{ post.source }}">{{ post.source }}</a></p>
            <p><strong>Description:</strong> {{ post.description }}</p>
            
        </div>
    {% endfor %}
</div>