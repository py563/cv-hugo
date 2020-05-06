---
title: "Search Results"
sitemap:
  priority: 0.1
layout: "search"
---

This file exists solely to respond to /search URL with the related `search` layout template.

No content shown here is rendered, all content is based in the template layouts/page/search.html

Setting a very low sitemap priority will tell search engines this is not important content.

This implementation uses Fusejs, jquery and mark.js

## Initial setup

Search depends on additional output content type of JSON in config.toml

```json
[outputs]
  home = ["HTML", "JSON"]
```
