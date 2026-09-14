# joachimc.github.io

This repository serves static pages through GitHub Pages. It holds pages only.
It holds no code and no keys.

## What is here

| Path | Address | Source |
|---|---|---|
| `ironload/` | `https://joachimc.github.io/ironload/` | generated, see below |
| `index.html` | `https://joachimc.github.io/` | edit here |

## Search engines

Every page carries `<meta name="robots" content="noindex">`. IronLoad is not in
the stores yet, so the pages stay out of search results. A store reviewer still
reaches them, because a reviewer opens the address directly.

Remove the line from `index.html` at launch. For the pages under `ironload/`,
set `BEFORE_LAUNCH=0` in `scripts/build-site.sh` in the IronLoad repository, then
build and publish again.

There is no `robots.txt` that blocks a crawler on purpose. A blocked crawler
never reads the page, so it never sees the `noindex` line.

## Do not edit the IronLoad pages here

A script builds everything under `ironload/` from Markdown in the IronLoad
repository. An edit here goes away at the next build.

To change a page, edit the Markdown in the IronLoad repository, then run:

    scripts/build-site.sh --publish /path/to/JoachimC.github.io

Commit and push in both repositories.
