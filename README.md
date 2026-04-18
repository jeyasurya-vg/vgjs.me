# vgjs.me

Personal portfolio and research site for Jeyasurya VG — cybersecurity researcher,
MS/PhD candidate at IIT Madras, security engineer at Securin.

Built on [al-folio](https://github.com/alshedivat/al-folio) with a custom dark
cybersecurity theme. Design sensibility inspired by [steipete.me](https://steipete.me).

**Live:** https://jeyasurya-vg.github.io/vgjs.me/
**License:** Content CC BY 4.0 · Code MIT

---

## Local development

```bash
git clone https://github.com/jeyasurya-vg/vgjs.me.git
cd vgjs.me
bundle install
bundle exec jekyll serve --livereload
```

Visit http://localhost:4000

---

## Adding a blog post

Create `_posts/YYYY-MM-DD-your-slug.md` with this front matter:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0530
description: One sentence summary for SEO and post cards.
tags: [tag1, tag2]
categories: research
giscus_comments: true
related_posts: true
toc:
  beginning: true
---
```

---

## Adding a publication

Add a BibTeX entry to `_bibliography/papers.bib`. Set `selected={true}` to feature
it on the homepage. The publications page renders automatically.

---

## Updating the CV

Edit `_data/cv.yml`. A PDF is auto-compiled by GitHub Actions on every push
that touches `_pages/cv.md` or `_data/cv.yml`.

---

## Deployment

Push to `main`. GitHub Actions builds the Jekyll site and deploys to GitHub Pages
automatically. Enable GitHub Pages in Settings → Pages → Source: GitHub Actions.
