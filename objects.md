---
title: Objects
layout: default
date: 2026-01-01
summary: Every object in the collection, newest folder first — an image-first grid that builds itself from whatever is in objects/.
---

# Objects

{: .lede}
Every object in the collection. Nothing on this page is a list you maintain by
hand: it is assembled from whatever folders exist under `objects/`, so adding a
folder adds a tile here.

{% assign objects = site.pages
   | where_exp: "p", "p.path contains 'objects/'"
   | where_exp: "p", "p.path != 'objects.md'" %}

{% include nav/gallery-grid.html
  items=objects
  variant="uniform"
  min-width="200px"
  show-summary=true
  class="gallery-grid--wide"
%}
