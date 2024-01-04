---
layout: default
title: Added a navigation menu to all pages
description: Where I describe the process of adding a menu to the site.
date: 2024-01-04
author: Michael Rowe
---
# Navigation menu added

*Note: One of the reasons for describing this in this level of detail is also for me to document what I'm learning.*

When I started this project and chose to use a static site generator to build the pages, I didn't really appreciate how much of the output of database-driven sites is typically dynamically created.

Menus are one of those things that don't come automatically with a static site, which means you need to build it from scratch.

The way I've done it - probably not the best way but it's the simplest way - was to create a *menu.html* file in a new *_includes* folder, and then include a [Liquid tag](https://shopify.github.io/liquid/basics/introduction/) in the `<header>` element of the *default.html* layout template to point to that menu file. So:

- menu.html - the menu content is written in basic HTML in this file.
- default.html - configures the layout of the pages that are generated.
- Liquid tag in default.html - specifies where to place the menu in the generated page, and where to find the content of the menu.

It's not very complicated but it took me a while to figure out exactly how to do it. At some point, once things are up and running and I'm mainly focused on building out the content, I'd like to get back into CSS to style some of the menu elements and add a bit of flair to the menu.

I'd also like to experiment a bit with *includes* and see what else I can add to the site using this feature.