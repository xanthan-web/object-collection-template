---
title: Objects
layout: default
date: 2026-01-01
summary: Every object in the collection, newest folder first — an image-first grid that builds itself from whatever is in objects/.
---

# Objects

{: .lede}
Every object in the collection, squared off and labelled so the entries can be
read down like a list. Nothing on this page is maintained by hand: it is
assembled from whatever folders exist under `objects/`, so adding a folder adds
a tile here. The [gallery]({{ site.baseurl }}/gallery) shows the same objects at
their own proportions, for looking rather than finding.

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
