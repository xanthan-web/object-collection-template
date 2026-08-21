---
title: Essays
layout: default
date: 2026-01-01
summary: Thematic essays that read across the collection — the arguments the objects make together rather than one at a time.
---

# Essays

{: .lede}
An object page describes one thing. An essay follows something *through* several
of them — a motif, a material, a habit of making, a silence in the record — and
says what the collection knows that no single entry can. This is where a
collection stops being an inventory and starts making a claim.

{% assign essays = site.pages
   | where_exp: "p", "p.path contains 'essays/'"
   | where_exp: "p", "p.path != 'essays/index.md'" %}

{% include cards/card-grid.html cards=essays show-tags=true %}

## How the essays and the objects hold together

The two sample essays above deliberately overlap. The [Head of the
Buddha]({{ site.baseurl }}/objects/buddha-head) appears in both, once as
evidence of a borrowed carving tradition and once as an object whose paint has
gone. That is the point: an object is not used up by the first argument made
about it, and a reader who arrives at it from one essay can leave through
another.

So the relationship runs both ways. Essays name objects, and the objects sit in
the collection independent of any essay that cites them. Nothing breaks if an
essay is deleted, and nothing needs updating when an object is added.

## How this page builds itself

Like the other index pages, this one is a query rather than a list:

```liquid
{% raw %}{% assign essays = site.pages
   | where_exp: "p", "p.path contains 'essays/'"
   | where_exp: "p", "p.path != 'essays/index.md'" %}{% endraw %}
```

The second line keeps this page from listing itself. Add a folder under
`essays/` with an `index.md` in it and a card appears here; the card's picture is
that essay's `thumbnail`, its text is `summary`, and the pills are its `tags`.
Set `position: 1`, `position: 2` and so on in an essay's front matter to fix the
reading order — without it the cards come out in whatever order Jekyll found the
folders.

[Instructions]({{ site.baseurl }}/instructions) has the full front matter list
and the pattern for citing objects inside an essay.
