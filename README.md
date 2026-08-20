# Object Collection Template

A website template for collections built around things — artefacts, sites,
specimens, images, places — built on the [Xanthan](https://github.com/xanthan-web/xanthan)
framework and hosted on GitHub Pages.

**[Live demo](https://xanthan-web.github.io/object-collection-template)** · **[Xanthan docs](https://xanthan-web.github.io/xanthan/docs/)**

---

## What This Is

Each object gets its own folder holding its page and its images. The catalogue
facts live in that page's front matter, so they are written once and read
everywhere: an image-first grid assembles the directory, a map plots whatever
carries coordinates, and search indexes the lot.

Choose this over the Essay Collection template when the object *is* the entry
and the writing supports it — a digital exhibit, a material-culture course, a
site survey, a collection catalogue.

A finished example: [Material Objects of the Silk Road](https://amaranth.unm.edu/silk-road/)

---

## Structure

```
objects/
  bowl-with-dragons/
    index.md        ← the entry, with catalogue facts in its front matter
    images/         ← that object's images, kept beside it
index.md            ← homepage: hero, featured objects, links
objects.md          ← the grid, assembled from objects/
map.md              ← every object with geo coordinates
about.md            ← what the collection is and who made it
instructions.md     ← how to add an object
docs/               ← full Xanthan documentation (synced from the framework)
```

Nothing indexes objects by hand. The grid is a Liquid query over the folder:

```liquid
{% assign objects = site.pages | where_exp: "p", "p.path contains 'objects/'" %}
```

So adding a folder adds a tile, and deleting one removes it.

---

## Getting Started

1. Click **Use this template** on GitHub to make your own copy.
2. In `_config.yml`, set `title` and `baseurl` to match your repository name.
3. Copy a folder under `objects/`, rename it, and replace what is inside.
4. Delete the three samples when you no longer need them.

`instructions.md` covers the front matter fields in full, and ships as a page on
the site so contributors can read it without opening the repository.

---

## The Samples

Three sample objects are included as stand-ins so the site looks like a working
collection before you add anything. Their images come from
[The Metropolitan Museum of Art](https://www.metmuseum.org/)'s open-access
collection; the text is placeholder written for this template.
