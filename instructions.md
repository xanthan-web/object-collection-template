---
title: Instructions
layout: default
date: 2026-01-01
summary: How to add an object to this collection, and what each front matter field does.
---

{% include nav/scrollspy-toc.html %}

# Adding an Object

{: .lede}
Everything in this collection is a folder with a page in it. To add an object,
copy one of the samples, rename the folder, and change what is inside. Nothing
else on the site needs editing — the grid, the map, and search all read from the
page you just made.

## The short version

1. Copy any folder under `objects/` and give the copy a new name.
2. Put your images in its `images/` folder.
3. Open `index.md` in the copy and change the front matter and the text.
4. Commit. The object appears on the [objects page]({{ site.baseurl }}/objects)
   and, if it has coordinates, on the [map]({{ site.baseurl }}/map).

The folder name becomes the object's web address, so use lowercase words joined
by hyphens: `bowl-with-dragons`, not `Bowl With Dragons (final).md`.

---

## What each front matter field does

The block at the top of an object page, between the `---` lines, is where the
catalogue facts live. Write them once here and they appear everywhere.

| Field | Required | What it does |
|-------|----------|--------------|
| `title` | yes | The object's name, used on the page, the grid, and the map |
| `summary` | yes | One or two sentences. Appears under the title on the grid and in the map popup |
| `thumbnail` | yes | The image the grid tile uses, and the picture in the map popup. A path inside this folder, e.g. `images/bowl.jpg` |
| `header-image` | no | The wide image across the top of the object's own page |
| `header-title` | no | The text shown on that header. Without it the header renders empty |
| `header-tier` | no | `hero` (full screen), `section` (~60vh), or `banner` (~22vh). The samples use `banner` |
| `header-position` | no | Which part of the image to keep when it is cropped, e.g. `center 38%` |
| `author` | no | Who wrote the entry. Shown on cards that display a byline |
| `geo` | no | `[latitude, longitude]`. Add it and the object appears on the map; leave it out and it does not |
| `placename` | no | Where the object is from, shown in the map popup |
| `medium`, `object-date`, `collection` | no | Your own catalogue fields. These three are printed in the map popup because `map.md` asks for them by name; add whatever else your collection needs |
| `tags` | no | A list. Objects that share a tag can be found together |

Field names you invent yourself work the same way as the ones above. If your
collection needs `accession-number` or `excavation-season`, add it — and if you
want it in the map popup as well, add it to the `fields` list in `map.md`.

---

## Images

Keep an object's images in its own folder, next to its page. Then a path like
`images/bowl.jpg` works, and moving the folder moves everything with it.

Two sizes are worth thinking about:

- **The thumbnail** is seen small, in a grid with others. Crop it so the object
  fills the frame.
- **The header image** runs wide and shallow across the top of the page. A tall
  image will be cropped badly; a wide one will not.

Images larger than about 2000 pixels on the long side make pages slow to load
without looking any better. Resize before uploading.

---

## Writing the entry

The sample objects show the shape: a paragraph saying what the reader is looking
at, then sections that make an argument about it. Use the
[Component Library]({{ site.baseurl }}/docs/reference/component-library) for
figures, asides, pull quotes, and carousels.

Two habits worth keeping:

**Say why the object is in the collection.** The front matter already says what
it is. The page should say what it lets a reader see.

**Credit the image.** If it comes from a museum's open-access collection, name
the museum and link the record. Captions are the right place.

---

## Removing the samples

The three sample objects are stand-ins. When you have your own, delete their
folders, then edit `index.md` at the top level — the hero text, the three
featured objects, and the closing links all name them.
