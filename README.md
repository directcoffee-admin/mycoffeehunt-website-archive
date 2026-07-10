# mycoffeehunt.com.au — Website Backup

A static, offline-viewable backup of the old My Coffee Hunt website
(https://mycoffeehunt.com.au), captured on **2026-07-10**.

## What this is

The old site is a single-page static website (all navigation is in-page
`#anchor` links). This backup contains the full homepage HTML with all
CSS/JS inlined, plus every image asset it references.

To view it, open:

```
mycoffeehunt.com.au/index.html
```

in any web browser. Links have been rewritten for offline viewing.

## Contents

```
mycoffeehunt.com.au/
├── index.html                     # Homepage (CSS + JS inlined)
└── assets/images/
    ├── card.jpg                   # Open Graph / social share image
    ├── container07.jpg            # Background image
    └── image01–07.(png|jpg)       # Page imagery
```

Total: 10 files, ~500 KB.

## How it was captured

Mirrored with `wget --mirror --page-requisites --convert-links
--adjust-extension`, followed by manually fetching the `<head>`-only
referenced assets (`card.jpg`) that the crawler skipped because they
aren't linked from the page body. The `?v=88e49ae2` cache-busting query
strings are preserved in the local filenames, and the HTML's links were
rewritten to match, so the page renders correctly offline.

## Known limitations (external content, not part of the site)

These are hosted by third parties and therefore cannot be captured in a
site backup — they require a live internet connection to display:

- **Embedded YouTube video** (Cartel Roasters clip) — served from
  youtube-nocookie.com.
- **Google Fonts** (Dosis, Source Sans Pro, Lato) — loaded from the
  Google Fonts CDN. The browser falls back to system fonts offline.

The `robots.txt`/`sitemap.xml` list only the homepage, and the site has
no other pages, so this backup is complete for the site's own content.
