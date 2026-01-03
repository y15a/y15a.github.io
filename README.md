# y15a.com

Personal blog built with [Hugo](https://gohugo.io/) and [PaperMod](https://github.com/adityatelange/hugo-PaperMod).

## Setup

Download Hugo extended binary to the repo root:

```bash
wget -qO- https://github.com/gohugoio/hugo/releases/download/v0.153.4/hugo_extended_0.153.4_linux-amd64.tar.gz | tar xz hugo && mv hugo hugo.linux
```

## Creating a new article

```bash
./hugo.linux new posts/my-article-slug.ja.md  # Japanese
./hugo.linux new posts/my-article-slug.en.md  # English
```

This creates a draft with the following frontmatter:

```yaml
---
title: "My Article Slug"
date: 2024-01-01T12:00:00+09:00
draft: true
tags: []
---
```

- `title`: Auto-generated from filename, edit as needed
- `draft`: Set to `false` to publish
- `tags`: Add relevant tags, e.g., `["Productivity", "Software"]`

## Preview locally

```bash
./hugo.linux server
```

Opens at http://localhost:1313/ with live reload.

Add `-D` to include drafts:

```bash
./hugo.linux server -D
```
