---
layout: default
title: CCS Workbench
---

<section class="tool-deep-dive">

<div class="tool-entry-head">
<img src="/assets/images/tools/ccs-wb.svg" alt="" class="tool-icon-lg">
<div>
<h1>CCS Workbench</h1>
<p class="object"><em>Method:</em> close reading. <em>Object:</em> a single artefact of code.</p>
<p><a href="https://ccs-wb.vercel.app">ccs-wb.vercel.app</a> · <a href="https://github.com/Computational-Hermeneutics/CCS-WB">github.com/Computational-Hermeneutics/CCS-WB</a> · <a href="/tools.html">All tools</a></p>
</div>
</div>

</section>

The Critical Code Studies Workbench is a web application for the close reading and hermeneutic analysis of software as a cultural artefact. Software deserves the same close reading we give literature; the Workbench is the tool that makes that reading practicable, holding code, annotation, and interpretation in a single interpretive surface. It is the close-reading tool of the Computational Hermeneutics family.

## Why the Workbench

Critical code studies argued, more than a decade ago, that code is a text with meaning, susceptible to interpretation, situated in culture and history. What has been missing is an tool that supports the practice at the resolution it demands: line-by-line annotation, typed interpretive moves, the recovery of historical software, and an AI interlocutor pitched at the right level for the reader. The Workbench treats a body of code as an object of reading and provides the apparatus, the IDE-style layout, the annotation types, the methodological scaffolding, for reading it well.

## Modes

- **Critique.** An IDE-style close reading of existing code. A file tree, a code editor with line numbers, and an annotation layer. Click any line or select a range to annotate, across six types: observation, question, metaphor, pattern, context, and critique. The AI co-reader engages as an expert practitioner, challenging interpretations and pressing on technical depth, a peer rather than a tutor.
- **Interpret.** A guided exploration of CCS methodology, the hermeneutic frameworks, and the archaeological recovery of historical software. The AI engagement here is beginner-friendly, scaffolding concepts and suggesting readings, for the scholar coming to the approach for the first time.
- **Create.** Generative coding to understand algorithms by building them, in the "vibe coding" sense: writing code as a way of thinking through what it does. The AI works as an intermediate practitioner, using CCS vocabulary and encouraging experimentation.

## Annotation

Both reading modes use a unified annotation layer. Annotations are typed, anchored to lines or ranges, and summarised by type in a side panel. An AI auto-annotation pass can propose annotations for review, which the reader accepts or discards, so that machine suggestion is always subordinate to the reader's judgement. The annotation infrastructure is shared with the wider family, including Source Variorum, so that a reading made in one tool can travel to the other.

## Theoretical background

The Workbench operationalises the critical code studies tradition associated with Mark Marino and the 10 PRINT collective, and the longer argument that software is a proper object of hermeneutic and critical-theoretical reading. It places the human reader's intention, the model's generative contribution, and the executable artefact in a single triadic frame, and it insists that interpretation and evidence stay bound together: every claim is anchored to the code that occasions it.

## Stack

Next.js and React with TypeScript for the interface, and multi-provider adapters for the AI co-reader. Hosted at [ccs-wb.vercel.app](https://ccs-wb.vercel.app); the repository carries full setup instructions.

## Status

Version 5.1.x, CCS methodology v2.7. The three modes are live, with the unified IDE layout, six annotation types, AI auto-annotation, and colour-coded file handling. See the repository for the current state of each capability and its known limitations.

## Siblings

[Source Variorum](/tools/source-variorum.html) takes the collation method, setting two or more witnesses side by side and reading the movement between them. A locus of divergence flagged by Source Variorum is exactly the place where the Workbench's close reading is most rewarded.
