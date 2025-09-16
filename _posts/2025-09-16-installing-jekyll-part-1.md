---
layout: post
title: "My experience of installing Jekyll: Part 1 – Local setup"
date: 2025-09-16 17:54:24 +0100
categories: jekyll
---

I was a bit wary about installing and self-hosting this blog, but it has turned out to be a fairly simple experience so far – although there were a couple of issues with the macOS instructions on the Jekyll website.

## Installing Ruby

The instructions for macOS mention that Big Sur comes with Ruby 2.6.3 installed, which is greater than the 2.5.0 the Jekyll apparently requires, but that earlier macOS versions will need to install Ruby through Homebrew. In fact, I immediately ran into issues with this version because some of the dependencies required at least version 3.0.0 of Ruby.

After installing the latest version of Ruby using Homebrew, I still needed to install rbenv in order to get the correct binary to execute. For some reason, `which ruby` kept returning the OS version instead of the Homebrew version. Once rbenv was installed and initialised, and I'd restarted my terminal a couple of times, I was able to install Jekyll itself.

## Quickstart

This was pretty basic but it worked. I decided not to go through the full tutorial right now, but I did have a look at it and it would have been useful to have some of the information from there in the quickstart.
