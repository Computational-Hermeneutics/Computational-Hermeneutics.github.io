# Computational-Hermeneutics.github.io

Landing site and map for the **Computational Hermeneutics** family of tools:
research tools that bring the apparatus of textual criticism and
interpretation to computational artefacts, to code as much as to text.

Published at **[computational-hermeneutics.github.io](https://computational-hermeneutics.github.io)**.

## Build

A Jekyll site, built and served by GitHub Pages. No local toolchain is
required to edit content; GitHub Pages compiles the SCSS and Liquid on push.

To preview locally (optional):

```
gem install bundler jekyll
jekyll serve
```

## Structure

- `index.md`, `tools.md` — the two top-level pages.
- `tools/*.md` — per-tool deep-dive pages.
- `_layouts/default.html` — shared layout, with light/dark theme toggle and
  per-theme image swapping.
- `_includes/mermaid.html` — theme-aware Mermaid rendering for the family map.
- `assets/css/style.scss` — the editorial styles (philological palette).
- `assets/images/` — light artwork; `assets/images/dark/` — dark variants.

## Design

Light is the default theme; dark is activated by `html[data-theme="dark"]` and
persisted in `localStorage`. The palette and typography are those of a critical
edition: aged-parchment grounds and sepia ink set in EB Garamond, with rubric
oxblood as the primary brand and link colour, antique gold for the close-reading
method, and manuscript lapis for the collation method.

Maintained by [David M. Berry](https://github.com/dmberry).
