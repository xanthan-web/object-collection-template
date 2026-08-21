---
title: Borrowed Forms
layout: base
author: Your Name
date: 2026-01-01
position: 1
header-image: /objects/bowl-with-dragons/images/cropped-theme-essay-header.jpg
header-title: Borrowed Forms
header-tier: banner
header-position: center
thumbnail: /objects/buddha-head/images/buddha-head-front.jpg
summary: A Greek way of carving a face and a Chinese way of drawing a dragon, both a long way from home — shapes travel more easily than the meanings attached to them.
tags:
  - iconography
  - exchange

objects:
  - slug: buddha-head
    label: Gandhara, 4th–5th century
  - slug: bowl-with-dragons
    label: Tabriz, 1210
---

# Borrowed Forms

This is sample content. Replace it with your own argument and keep the shape.

{: .lede}
Two objects in this collection were made by people who had learned a shape from
somewhere else. Neither is a copy, and neither is quite an original. They are
useful together because they show the same thing happening twice, six centuries
and three thousand miles apart: a form arrives ahead of the belief that produced
it, and the people who receive it put it to their own use.

{% include layout/picks.html
  items=page.objects
  collection="objects"
  variant="strip"
  columns=2
  kicker="Objects in this essay"
  title="Two things that borrowed a shape."
%}

## A Greek habit of carving

The [Head of the Buddha]({{ site.baseurl }}/objects/buddha-head) is a South
Asian subject rendered by hands trained in a Mediterranean tradition — the wavy
hair, the heavy lids, the naturalism of the mouth. The sculptors of Gandhara had
inherited Greek workshop practice from the Hellenistic kingdoms that preceded
them, and they applied it to a figure those workshops had never had reason to
depict.

{% include images/figure-wrap.html
  image-path="/objects/buddha-head/images/buddha-head-front.jpg"
  image-position="right"
  image-width="38%"
  alt-text="Stucco head of the Buddha with wavy hair and downcast eyes"
  caption="[The Metropolitan Museum of Art](https://www.metmuseum.org/), open access."
  text="What crossed the distance was technique, not doctrine. The carvers did not become Buddhists by learning to carve a Buddha, and the Buddhists who commissioned the work were not importing Greek religion along with the Greek chisel. A method of representing a human face turned out to be portable in a way that the beliefs on either side of the exchange were not."
%}

## A Chinese motif on an Iranian bowl

The dragons on the [Bowl with Dragons]({{ site.baseurl }}/objects/bowl-with-dragons)
arrive from further east than the workshop that glazed them. The coiled form is
recognisably Chinese; the reading of it in thirteenth-century Iran — a device
against eclipses, according to some scholars — is not.

{% include typography/pullquote.html
  text="The shape survived the journey intact. What it was understood to mean did not, and that is the more interesting half of the story."
%}

Put the two objects beside each other and the pattern is legible in a way it is
not from either page alone. That is the whole case for having essays in a
collection built around things.

## Writing your own

An essay is a folder under `essays/` with an `index.md` in it, exactly like an
object. The two habits worth keeping:

**Name the objects you are arguing from.** Link them in the prose, and list them
in the `objects:` block in this page's front matter so the strip above builds
itself. If you rename an object's folder, the strip prints a visible warning
rather than failing silently.

**Do not repeat the catalogue.** The object page already says what the thing is,
where it was made, and what it is made of. The essay should say what it is
evidence *for*.

---

## Bibliography

- Author. *Title*. Publisher, Year.
