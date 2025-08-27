# Old Man Yells at HEMA — Jekyll Blog

A minimal, dark‑mode blog for articles and photo posts. Built for GitHub Pages.

## Quick start
1. Create a new GitHub repo and upload these files.
2. In **Settings → Pages**, choose **GitHub Actions** (Jekyll) or **Deploy from branch** (main / root).
3. Visit your live URL. Add posts in `_posts/` as `YYYY-MM-DD-title.md`.

## Write a post
Create a file in `_posts/` like:
```
---
layout: post
title: "First Post"
description: "Why I still fence longsword."
image: /assets/images/hero.svg
tags: [hema, training]
---

Your markdown goes here.
```

## Gallery images
Drop images into `assets/images/` then reference them like: `![alt](/assets/images/filename.jpg)`

## Custom domain (optional)
Add your domain in **Settings → Pages**, then create DNS records per GitHub’s docs.