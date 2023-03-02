# github-pages-codespaces

## Introduction

This is a barebones website/blog based on [diezcami/arctic-fox-theme](https://github.com/diezcami/arctic-fox-theme) with some improvements and modifications.

This website uses the [Jekyll](https://jekyllrb.com/) static webiste framework.

It is intended to be developed with [GitHub Codespaces](https://github.com/features/codespaces) and deployed with [GitHub Pages](https://pages.github.com/).  Go to the code dropdown and create a codespace to get developing!

To run the server locally, run the `jekyll serve` command in your terminal.  Port 4000 will be forwarded, which you can open in your web browser.  

> This repo's [devcontainer.json](.devcontainer/devcontainer.json) includes a `postAttachCommand` that will execute this command automatically when connecting to the codespace 🚀

### Generating tags

1. Add your tag to the preamable of a post in `_posts/`

Eg: 
```
---
layout: post
title: "Hello, User!"
date: 2023-02-28
permalink: hello
tags: getting-started
---
```

2. Run `python3 tag_generator.py`
3. Restart the jekyll server.
