---
layout: default
title: Source Variorum
---

<section class="tool-deep-dive">

<div class="tool-entry-head">
<img src="/assets/images/tools/source-variorum.svg" alt="" class="tool-icon-lg">
<div>
<h1>Source Variorum</h1>
<p class="object"><em>Register:</em> collation. <em>Object:</em> two or more witnesses of a text, code or prose.</p>
<p><a href="https://sourcevariorum.vercel.app">sourcevariorum.vercel.app</a> · <a href="https://github.com/Computational-Hermeneutics/Source-Variorum">github.com/Computational-Hermeneutics/Source-Variorum</a> · <a href="/tools.html">All tools</a></p>
</div>
</div>

</section>

Source Variorum is a side-by-side textual collation workbench. A *variorum*, from *cum notis variorum*, "with the notes of various people", is a work of textual criticism that collates all known variants of a text and sets them side by side, so that a reader can track how textual decisions have been made in preparing a text for publication. Source Variorum brings that apparatus to computational close reading. It is the collation instrument of the Computational Hermeneutics family.

## Why Source Variorum

Versions of a text, whether commits of source code or witnesses of a poem, differ from one another in ways that are interpretively significant. Lines are added, deleted, and substituted; whole passages move. Standard diff tools show insertion and deletion but cannot see transposition: moved text reads as a deletion in one place and an unrelated addition in another, and the movement, often the most telling thing, is lost. Source Variorum is built to make movement visible, and to render the full range of variation as a single readable apparatus.

## Two modes

- **Source code** — line- and token-aware, monospace, for collating versions of code and reading the movement of code as a cultural-textual process.
- **Text** — sentence- and word-aware, proportional type, with witness sigla, for prose witnesses, paratexts, and classical or hermeneutic comparison.

## What it shows

- A three-column **braid** (Witness A · ribbon gutter · Witness B) with Bezier ribbons whose thickness scales with the length of the matched block.
- Variant typing: **match**, **substitution**, **addition**, **deletion**, **transposition** (moved text), and near-identical **variant** (fuzzy match).
- An auto-generated **critical apparatus** listing every locus of divergence by siglum.
- Auto-collation with hand-correction, so that the scholar remains the final arbiter of how witnesses are aligned.

## Theoretical background

Source Variorum makes the vocabulary of textual scholarship, the witness, the siglum, the copy-text, the *apparatus criticus*, the transposition, operable on computational material. It treats the differences between witnesses not as noise to be minimised but as the textual condition itself: the record of how a text was made and remade. The braid is the argument made visible.

## Stack

Next.js and TypeScript. Auto-collation produces an initial alignment that the reader can correct by hand. Hosted at [sourcevariorum.vercel.app](https://sourcevariorum.vercel.app); the repository carries full setup instructions.

## Status

Version 0.6.x. Source code and text modes are live, with the transposition braid, the five variant types plus fuzzy variant, and the auto-generated critical apparatus. Support for three or more witnesses is a later phase. See the repository for the current state of each capability.

## Siblings

[CCS Workbench](/tools/ccs-wb.html) takes the close-reading register, opening a single artefact of code for annotation and interpretation. The two instruments share an annotation layer, so a reading made over a single witness in the Workbench can be brought to bear on the loci of divergence that Source Variorum surfaces.
