---
layout: post
title: "My experience of installing Jekyll: Part 2 – Github Pages"
date: 2025-09-16 22:00:00 +0100
categories: jekyll
---

Now it was time to put this on the internet somewhere.

## Github

Uploading the site to Github was simple, as the `.gitignore` file was already configured properly, only needing a line for the `.vscode` folder to be added.

The repository is at [oryant/oryan-uk-jekyll](https://github.com/oryant/oryan-uk-jekyll).

## Github Pages and Github Actions

The next step was to create a Github Pages site for the blog. Since the `_site` folder is not part of the repository, this needs to be generated dynamically using Github Actions.

It seemed logical to follow the [Github Actions](https://ashmaroli.github.io/jekyll/docs/continuous-integration/github-actions/) tutorial from the Jekyll site. This was okay at first, but I soon found that the Jekyll Actions link to the Github marketplace was dead. I decided to use the search tool in Github, and figured that the action called **GitHub Pages Jekyll** should work well enough.

Not knowing what most of the file meant, I left in untouched. I assume some stuff is being read from the site's config.yml file but actually the whole process is fairly opaque, which isn't my favourite.

I encountered an error message the first time this ran, because I hadn't set up Github Pages yet. Having to go to Settings in the repository to configure Pages seems like a weird choice, but I've done it before so I didn't have any trouble setting this up.

My blog is now live at [Github Pages](https://oryant.github.io/oryan-uk-jekyll).
