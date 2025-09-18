---
layout: post
title: "My experience of installing Jekyll: Part 3 – more Github Pages"
date: 2025-09-18 17:00:00 +0100
categories: jekyll
---

Once I had got the build process sorted and the site was live on Github Pages, I suspected I would have some work to do to get the site working behind my Cloudfront distribution.

I knew I wanted to serve the site at <https://www.oryan.uk/blog/>, but this seemed impossible because, it turns out, the build process for Github Pages disregards the `baseurl` variable specified in **_config.yml** and forces it to use a path corresponding to the name of the Github repo.

My various attempts to change the base url to /blog, or even /oryan-uk-jekyll/blog were unsuccessful. Removing the dynamically-generated `--baseurl` value from the build workflow and overwriting it with my own simply cause the build to fail in ways I couldn't understand.

In the end, I simply changed the name of the repo to **blog** in order to force the Github Pages URL to change. I didn't like doing that – I'd prefer to have a more descriptive name for the repo, but unless it's possible to change the path that Github Pages serves from (I don't think it is), it's a necessary compromise.

In any case, all this means that I don't need to write a part 4 of this covering Cloudfront, since the existing distribution that I created for another purpose still works. If it turns out I need to change it in future, I might write about it then.

So anyway now I have a blog. Now I just need to remember to actually write things on it, and maybe get off the boring default template.
