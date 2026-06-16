---
layout: default
title: Computational Hermeneutics
---

<section class="lede">

A text and the code that now so often accompanies it have more in common than we usually allow. Indeed, both are written and rewritten, copied, forked, and revised and both accumulate variants and witnesses as they go. This means that they can be read closely, or compared across their versions. Computational Hermeneutics treats text and code alike as research objects. Yet the methods and approaches that philology built over centuries for this work, the witness, the siglum, the copy-text, the <em>apparatus criticus</em>, the collation, have not been fully brought to bear on code, on corpora, or on machine-generated text. The interpretive traditions and the computational artefacts could be said to have stayed in separate rooms.

Computational Hermeneutics is an attempt to bring them together. The tools here treat computational artefacts as objects of reading rather than only of execution or measurement, that is, code as a cultural text, the corpus as a field of witnesses, the generated output as a text with a provenance. The tools are local-first, interpretively powerful, and built for close reading rather than distant measurement.

There are currently two tools. The close-reading tool opens a single artefact for intensive interpretation. The comparative-analysis tool sets witnesses side by side and reads the differences between them. The first tool supplies depth of interpretation; the second supplies the comparative ground on which textual and critical claims can be made.

</section>

## The family

<div class="mermaid">
graph TB
  subgraph reading["Close reading (single artefact)"]
    C["CCS-WB\ncode as cultural text"]
  end

  subgraph collation["Comparative analysis (multiple witnesses)"]
    S["Source Variorum\nwitnesses side by side"]
  end

  C -.shared annotation layer.-> S
  S -.loci for close reading.-> C

  classDef reading fill:#ffffff,stroke:#b8862e,color:#1a1a1a,stroke-width:1.2px;
  classDef collation fill:#ffffff,stroke:#3563a8,color:#1a1a1a,stroke-width:1.2px;
  class C reading;
  class S collation;
</div>

### Close reading

<div class="tools-grid">

<article class="tool-card scope">
  <img class="tool-icon" src="/assets/images/tools/ccs-wb.svg" alt="">
  <h3><a href="/tools/ccs-wb.html">CCS Workbench</a></h3>
  <p class="object">Object: a single artefact of code.</p>
  <p>Close reading, annotation, and interpretation of software in the critical code studies tradition. Three modes: critique, interpret, create. The interpretive tool of the family.</p>
  <p class="launch"><a href="https://ccs-wb.vercel.app">Open the live app ↗</a> · <a href="/tools/ccs-wb.html">Deep dive</a></p>
</article>

</div>

### Comparative analysis
<div class="tools-grid">

<article class="tool-card comparative">
  <img class="tool-icon" src="/assets/images/tools/source-variorum.svg" alt="">
  <h3><a href="/tools/source-variorum.html">Source Variorum</a></h3>
  <p class="object">Object: two or more witnesses of a text, code or prose.</p>
  <p>A braided collation workbench. Additions, deletions, substitutions, and transpositions are read in a central braid of ribbons, with an auto-generated critical apparatus. The comparative tool of the family.</p>
  <p class="launch"><a href="https://sourcevariorum.vercel.app">Open the live app ↗</a> · <a href="/tools/source-variorum.html">Deep dive</a></p>
</article>

</div>

## Theoretical background

Computational Hermeneutics is a set of methods that work on the principle that the interpretation of computational artefacts is continuous with, rather than separate from, the long traditions of textual scholarship and critical theory. Critical code studies argued that software deserves the same close reading we give literature; textual criticism developed the techniques for tracking how a text changes across its witnesses; hermeneutics gave an account of how understanding moves between part and whole. These traditions have rarely been combined, and they have almost never been instrumented.

The deficit is one of tools as much as of theory. It is one thing to assert that a fork enacts an interpretation, that a refactoring is an emendation, that a generated text has a textual condition; it is another to be able to show it, line by line, witness against witness, with an apparatus that records every decision. The tools here are built to close that gap, to make the apparatus of philology operable on computational material, and to keep interpretation and attestation bound together so that no reading is offered without the evidence that supports it.

The commitment is to the local and the legible. Where so much computational analysis runs at a distance, summarising corpora into aggregate measures, these tools work at the resolution of the line, the token, the annotation, and the variant. They are designed for the scholar who wants to read a particular artefact, or collate particular witnesses, and to be answerable to the detail.

## How the tools relate

The two methods are complementary. Close reading opens a single artefact at depth: the CCS Workbench reads a body of code through annotation, critique, and interpretation, recovering the cultural and technical work that a piece of software performs. Comparative analysis works across witnesses: Source Variorum sets two or more versions of a text side by side and reads the movement between them, the additions, deletions, substitutions, and transpositions that constitute its textual history.

A finding surfaced in one method sharpens the other. A locus of divergence flagged by a collation is exactly the place where close reading is most rewarded; an interpretation developed through close reading tells you which variants matter and why. The annotation layer is deliberately shared between the tools so that a reading made in one can travel to the other.

The two tools are the first of a family. Further tools extending the same posture to concordance, witness relations, and paratext are in preparation.

## Further reading

The tools operationalise commitments developed across critical code studies, textual scholarship, and the critical theory of computation. The literature below sets the conceptual ground; the tools are the working apparatus.

### Critical code studies and software theory

- Berry, D.M. (2011) *The Philosophy of Software: Code and Mediation in the Digital Age*. Basingstoke: Palgrave Macmillan.
- Marino, M.C. (2020) *Critical Code Studies*. Cambridge, MA: MIT Press.
- Montfort, N., Baudoin, P., Bell, J., Bogost, I., Douglass, J., Marino, M.C., Mateas, M., Reas, C., Sample, M. and Vawter, N. (2014) *10 PRINT CHR$(205.5+RND(1)); : GOTO 10*. Cambridge, MA: MIT Press.
- Chun, W.H.K. (2011) *Programmed Visions: Software and Memory*. Cambridge, MA: MIT Press.

### Textual scholarship and hermeneutics

- McGann, J.J. (1991) *The Textual Condition*. Princeton, NJ: Princeton University Press.
- McKenzie, D.F. (1999) *Bibliography and the Sociology of Texts*. Cambridge: Cambridge University Press.
- Gadamer, H.-G. (2004) *Truth and Method*. 2nd revised ed. London: Continuum.

### Critical theory of computation and AI

- Berry, D.M. (2014) *Critical Theory and the Digital*. New York: Bloomsbury.
- Berry, D.M. and Fagerjord, A. (2017) *Digital Humanities: Knowledge and Critique in a Digital Age*. Cambridge: Polity.
- Berry, D.M. (2025) 'Synthetic media and computational capitalism: towards a critical theory of artificial intelligence', *AI & SOCIETY*, 40(7), pp. 5257–5269.
- Ciston, S., Berry, D.M., Hay, A., Marino, M.C., Millican, P., Shrager, J., Schwarz, A. and Weil, P. (2026) *Inventing ELIZA: How the First Chatbot Shaped the Future of AI*. Software Studies series. Cambridge, MA: MIT Press.

## Using the tools

Each repository contains full documentation, dependencies, and setup instructions. The tools are offered as-is under permissive licences. If Computational Hermeneutics tools support published research, please cite the specific tool and version, and cite the relevant scholarship where the methods being applied are developed.

{% include mermaid.html %}
