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

## Two engines

Collation is not one operation. Code is almost one-to-one, lines correspond closely and the question is which lines changed, whereas prose is discourse, the "same" sentence is routinely rephrased and the question is which passages correspond at all. Source Variorum therefore collates with two engines, each with its own braid settings, selected to match the object under comparison. Both run on the same pure, deterministic core, so the typed variants, the apparatus, and the statistics stay in step whichever engine is in play.

- **CX-Engine** (CodeX, for code and exact textual collation). It reads the braid *literally*: leftover lines are paired only when genuinely alike, a renamed label or a changed operand, and otherwise called a clean addition or deletion; reformatting is ignored, so added or removed blank lines do not register as variants; and a block must be near-identical to count as a move. There is no locality prior, because code is not a narrative. The result is a tight, conservative braid suited to small edits between versions of a program.
- **TX-Engine** (TextX, for prose, verse, and translation). It pairs much more loosely, because correspondence here is semantic rather than positional, and adds a **locality prior**: corresponding passages tend to sit at similar relative positions in a narrative, so nearer-in-the-text pairings are preferred and a distant relocation must clear a higher similarity bar. It can segment by **line** rather than sentence for verse and drama. The braid is correspondingly smarter, reflecting that the "same" passage may read very differently across witnesses.

The engine follows the mode by default, the CX profile for code and the TX profile for prose, and the per-engine braid options are exposed in a settings panel for hand-tuning, with a three-tier confidence reading on each ribbon.

## What it shows

- A three-column **braid** (Witness A · ribbon gutter · Witness B) with Bezier ribbons whose thickness scales with the length of the matched block.
- Variant typing: **match**, **substitution**, **addition**, **deletion**, **transposition** (moved text), and near-identical **variant** (fuzzy match), with a live legend and counts in the status bar.
- **Word-level refinement** inside a differing line or sentence: only the words that actually change are tinted (a CollateX-style token alignment), so the eye lands on the divergence rather than the whole locus; the selected locus is framed in a strong version-variation highlight.
- A vertical **overview minimap** down the edge, every variant as a band at its position with a viewport box and click-to-jump, plus a horizontal change-overview histogram.
- An auto-generated **critical apparatus** listing every locus of divergence by siglum, and a **deep-dive** of quantitative statistics (verbatim overlap, moved-block counts, Jaccard / Dice / cosine similarity).
- In code mode, **syntax highlighting** layered over the variant tints, for modern languages and historical assembly dialects (PDP-1 MACRO, AGC, MAD, FORTRAN, IPL-V, BASIC).
- Auto-collation with hand-correction, so that the scholar remains the final arbiter of how witnesses are aligned. In Advanced mode, passages can be **hand-linked** by dragging an exact character range on each side.

## Theoretical background

Source Variorum makes the vocabulary of textual scholarship, the witness, the siglum, the copy-text, the *apparatus criticus*, the transposition, operable on computational material. It treats the differences between witnesses not as noise to be minimised but as the textual condition itself: the record of how a text was made and remade. The braid is the argument made visible.

## Stack

Next.js, React, TypeScript, Tailwind, CodeMirror, jsdiff, and jsPDF. The collation is computed **live in the browser** by a set of pure, deterministic functions: it is local-first, with no server and no model calls. A saved `.svar` project stores only the source of truth, the witnesses and your apparatus notes, and never the variants, which are recomputed deterministically on load. Hosted at [sourcevariorum.vercel.app](https://sourcevariorum.vercel.app); the repository carries full setup instructions.

## Status

Version 0.7.x. Source code and text modes are live, with the two collation engines (CX and TX), the transposition braid, the five variant types plus fuzzy variant, word-level refinement, the overview minimap, a project workbench (sources, folders, per-panel editing, undo/redo), an auto-generated critical apparatus with a quantitative deep-dive, and export to Markdown, TEI P5, PDF, and JSON. Support for three or more witnesses is a later phase. See the repository for the current state of each capability.

## Siblings

[CCS Workbench](/tools/ccs-wb.html) takes the close-reading register, opening a single artefact of code for annotation and interpretation. The two instruments share an annotation layer, so a reading made over a single witness in the Workbench can be brought to bear on the loci of divergence that Source Variorum surfaces.
