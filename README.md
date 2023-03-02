# github-pages-codespaces

## Introduction

This is a barebones website/blog based on [diezcami/arctic-fox-theme](https://github.com/diezcami/arctic-fox-theme) with some improvements and modifications.

This website uses the [Jekyll](https://jekyllrb.com/) static website framework.  This repo is setup to work nicely with [GitHub Codespaces](https://github.com/features/codespaces) and deployed with [GitHub Pages](https://pages.github.com/).

The contents of this repo are deployed to GitHub Pages at: [https://demo.spicer.dev/](https://demo.spicer.dev/).

## How To...

### Get started

This is a template repo.  Click the 'Use this Template' button to copy this GitHub repo to your account or org.

### Start Developing

To develop with Codespaces, click the Code dropdown on this repo and create a new codespace from the 'Codespace' tab. This will build and open a development environment for you.

To run the server locally, run the `jekyll serve` command in your terminal.  Port 4000 will be forwarded, which you can open in your web browser.  

> This repo's [devcontainer.json](.devcontainer/devcontainer.json) includes a `postAttachCommand` that will execute this command automatically when connecting to the codespace 🚀

### Deploying to GitHub Pages

This repo contains a [GitHub Action](https://github.com/joshspicer/github-pages-codespaces/blob/main/.github/workflows/jekyll-gh-pages.yml) that rebuilds and deploys the Jekyll app to GitHub pages on each push to the `main` branch.

See the [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) docs for more info on setting this up.

### Generate tags

This template lets you tag various posts. Tags appear on individual posts and when clicked, show an aggregated lists of all posts with that tag.  See the demo site's two example posts for an example.

When you add a new tag, you'll need to run through the steps below:

1. First, add your new, desired tag to the preamable of a post in `_posts/`

Eg: 
```
---
layout: post
title: "Hello, User!"
date: 2023-02-28
permalink: hello
tags: getting-started
---
...
...
```

2. Run `python3 tag_generator.py`
3. Restart the jekyll server.
