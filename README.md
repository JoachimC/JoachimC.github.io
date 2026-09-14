# joachimc.github.io

This repository serves static pages through GitHub Pages. It holds pages only.
It holds no code and no keys.

## What is here

| Path | Address | Source |
|---|---|---|
| `ironload/` | `https://joachimc.github.io/ironload/` | generated, see below |
| `index.html` | `https://joachimc.github.io/` | edit here |

## Do not edit the IronLoad pages here

A script builds everything under `ironload/` from Markdown in the IronLoad
repository. An edit here goes away at the next build.

To change a page, edit the Markdown in the IronLoad repository, then run:

    scripts/build-site.sh --publish /path/to/JoachimC.github.io

Commit and push in both repositories.
