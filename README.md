# github-pages-codespaces

## Introduction

This is a barebones jekyll based on [diezcami/arctic-fox-theme](https://github.com/diezcami/arctic-fox-theme) with some improvements and modifications.  

It is intended to be developed with [GitHub Codespaces](https://github.com/features/codespaces) and deployed with [GitHub Pages](https://pages.github.com/).

### Usage

To run the server locally, run the `jekyll serve` command in your terminal.  Port 4000 will be forwarded, which you can open in your web browser.

#### Generating tags

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
