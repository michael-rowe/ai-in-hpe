---
layout: post
title: Created the AI in HPE Github Pages repository
date: 2023-12-27
description: Where I explain setting up the Github repository and connecting it to Visual Studio Code. Basically, launching this project.
tags:
  - visual-studio-code
  - Github-Pages
author: Michael Rowe
---

# Created the AI in HPE Github Pages repository

On the 27th of Dec I created the [ai-in-hpe Github repository](https://github.com/michael-rowe/ai-in-hpe) for this project. I had a basic idea of how the markdown files in that repo would be converted into a website via [Jekyll](https://www.wikiwand.com/en/Jekyll_(software)) but no real understanding of the process.

I edited the README.md file to make sure that the content was displaying on the home page, and then added a few more pages with links to ensure that they site actually worked.

Next I set up [Visual Studio Code](https://www.wikiwand.com/en/Visual_Studio_Code) to connect to the Github repository. This meant I could edit markdown files on my local machine and then use VS Code to publish those files to the remote repository where Jekyll would build the HTML for the site.

I ended up using ChatGPT to help with some of the file editing, which I could have done without but which sped up the process of getting things done.

If I exclude all the faffing about with minor content editing, it probably took me about a day's worth of work to get the site up and running. This included time spent learning how to change the markdown in [Obsidian](https://www.wikiwand.com/en/Obsidian_(software)) (my default writing tool), which is slightly different for things like images and links. It also took me a while to experiment with the [YAML properties](https://help.obsidian.md/Editing+and+formatting/Properties). Even though it's not complicated, it did take some time to make sure that the Obsidian implementation was compatible with Github Pages.

All in all, it was a relatively quick and very satisfying experience.