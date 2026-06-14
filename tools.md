---
layout: default
title: Tools
---

# Tools

A brief guide to each instrument. Follow the **Deep dive** link on any tool for its extended page with operations, theoretical background, and status. The close-reading register opens a single artefact for intensive interpretation; the collation register sets witnesses side by side.

---

## Close reading

<section class="tool-entry scope">

<div class="tool-entry-head">
<img src="/assets/images/tools/ccs-wb.svg" alt="" class="tool-icon-lg">
<div>
<h2><a href="/tools/ccs-wb.html">CCS Workbench</a></h2>
<p class="object"><em>Register:</em> close reading. <em>Object:</em> a single artefact of code.</p>
<p><a href="/tools/ccs-wb.html">Deep dive</a> · <a href="https://ccs-wb.vercel.app">ccs-wb.vercel.app</a> · <a href="https://github.com/Computational-Hermeneutics/CCS-WB">github.com/Computational-Hermeneutics/CCS-WB</a></p>
</div>
</div>

The Critical Code Studies Workbench is a web application for the close reading and hermeneutic analysis of software as a cultural artefact. It works in three modes. **Critique** is an IDE-style close reading of existing code, with inline annotations across six types (observation, question, metaphor, pattern, context, critique) and an AI co-reader at the level of an expert peer. **Interpret** teaches the CCS methodology and the hermeneutic frameworks themselves, scaffolding the reader who is new to the approach. **Create** is generative coding to understand algorithms by building them. Annotation infrastructure is shared with the wider family.

<p class="tool-meta"><em>Stack:</em> Next.js, React, TypeScript, with multi-provider AI adapters.</p>

</section>

---

## Collation

<section class="tool-entry comparative">

<div class="tool-entry-head">
<img src="/assets/images/tools/source-variorum.svg" alt="" class="tool-icon-lg">
<div>
<h2><a href="/tools/source-variorum.html">Source Variorum</a></h2>
<p class="object"><em>Register:</em> collation. <em>Object:</em> two or more witnesses of a text, code or prose.</p>
<p><a href="/tools/source-variorum.html">Deep dive</a> · <a href="https://sourcevariorum.vercel.app">sourcevariorum.vercel.app</a> · <a href="https://github.com/Computational-Hermeneutics/Source-Variorum">github.com/Computational-Hermeneutics/Source-Variorum</a></p>
</div>
</div>

Source Variorum is a side-by-side textual collation workbench. A *variorum*, from *cum notis variorum*, "with the notes of various people", collates all known variants of a text so that a reader can track how textual decisions were made. Source Variorum brings that apparatus to computational close reading across two registers, **source code** (line- and token-aware, monospace) and **prose** (sentence- and word-aware, with witness sigla). It renders two witnesses in parallel with a central *braid*: curved ribbons connecting matched passages, including passages that have moved. The crossing of those ribbons is the analytical payload, showing at a glance where text has been added, deleted, substituted, or transposed, with an auto-generated critical apparatus listing every locus of divergence by siglum.

<p class="tool-meta"><em>Stack:</em> Next.js, TypeScript; auto-collation with hand-correction.</p>

</section>

## A note on naming

The naming grammar borrows from the vocabulary of textual scholarship:

- <strong>Workbench</strong>: a surface for close, iterative work with a single artefact, in the manner of critical code studies.
- <strong>Variorum</strong>: an edition that collates the variants of a text and records, in an apparatus, the notes of its various readers.
- <strong>Witness</strong>, <strong>siglum</strong>, <strong>apparatus</strong>: the terms of art the instruments make operable on computational material.

{% include mermaid.html %}
