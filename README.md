# Keo's Blog

This is a Jekyll blog deployed with GitHub Pages.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

## Publish

1. Create a GitHub repository named `keo-dara.github.io`.
2. Push this project to the `main` branch.
3. In the repository settings, open **Pages** and set source to **GitHub Actions**.
4. Every push to `main` will auto-deploy.

## Create new Post command

```
DATE=$(date +%F)
SLUG="my-new-post"
cat > "_posts/${DATE}-${SLUG}.markdown" <<EOF
---
layout: post
title: "Failed to beaware of myself"
date: $(date +"%Y-%m-%d %H:%M:%S %z")
categories: blog
---
Write your post here.
EOF
```
