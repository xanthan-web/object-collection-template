---
title: Map
layout: default
date: 2026-01-01
summary: Every object that carries coordinates, placed where it was made — the collection read as a geography rather than a list.
---

# Where the Objects Come From

{: .lede}
The same collection, arranged by place instead of by folder. An object appears
here as soon as its front matter carries `geo:` coordinates, and its marker
opens onto the catalogue facts already written there — nothing on this page is
a second list to keep in step with the first.

{% include nav/map.html
  folder="objects"
  fields="object-date,medium,collection"
  class="map-wrap--wide"
  height="70vh"
%}

## Putting an object on the map

Add two lines to an object's front matter and it arrives:

```yaml
geo: [38.1026, 46.3646]
placename: Tabriz, Iran
```

Right-click a spot in [Google Maps](https://maps.google.com) and click the
coordinates at the top of the menu to copy them. Objects without coordinates
simply do not appear — an object whose origin is unknown or contested is often
better left off the map than pinned to a guess.

The popup is assembled from the object's own front matter: `thumbnail`,
`title`, `placename`, then whatever `fields` names in the include above —
here `object-date`, `medium`, and `collection` — and finally `summary`. Change
that list to change what every popup shows.
