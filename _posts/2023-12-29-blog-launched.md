---
layout: default
title: Blog launched
date: 2023-12-29
description: Where I describe the process of adding a blog to this site.
tags: []
author: Michael Rowe
---

# Blog launched

So the news section of the site is up and running. It was easier than I thought it would be.

I've had lots of experience with WordPress and Blogger blogs but those kinds of content management systems are typically easy to set up and don't require any understanding of how they work. They're also database-driven and this site doesn't have a database (see *[static site generators](https://www.wikiwand.com/en/Static_site_generator)*).

Since there isn't a database to serve posts, you basically create your posts as single markdown files, taking care to name them in date order. What you actually name the file will become part of the URL, and the post title is generated from the properties YAML front matter. I also added the *description* and *tags* properties, to enhance discoverability of the posts.

Next I created the *blog.md* file, which would serve as the index of blog posts. The first version included just the title and date in an unordered list. I used ChatGPT to write the code that would include the *description* property from the post, and then edited the HTML to play around with the basic formatting of the index.

Finally, I needed to edit the configuration file to have Jekyll generate the RSS feed so that someone could subscribe to the blog with an [RSS reader](https://www.wikiwand.com/en/Rss_reader). This was a simple case of adding a line to the Jekyll configuration file to turn on the *jekyll-feed* plugin. You can now subscribe to the [feed](https://michael-rowe.github.io/ai-in-hpe/feed.xml) using any RSS reader (I use [Reader](https://readwise.io/read) but[Inoreader](https://www.inoreader.com/) is another good option).

It's not a sophisticated blogging system but it achieves the goal of allowing me to easily write quick posts in Obsidian, and then use VS Code to publish them to Github, which converts the markdown to an HTML post, and generates the RSS feed that you can read in the reader of your choice.