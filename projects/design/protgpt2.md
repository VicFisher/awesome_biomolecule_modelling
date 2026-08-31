---
name: ProtGPT2
field: design
category: hallucination
year: 2022
venue: "Nature Communications (2022)"
doi: 10.1038/s41467-022-32007-7
citations: 857
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/nferruz/ProtGPT2
repo_note: "shields.io could not resolve slug; verify exact repo path"
stars: null
license: MIT
tags: [sequence-generative, plm]
pioneering: true
status: draft
---

## Key innovation
A **GPT-2-style autoregressive protein language model** trained on UniRef50 that generates novel,
plausibly-folded protein sequences. A pioneer of **sequence-only generative design** (controllable
generation in sequence space), alongside ProGen.

> **Taxonomy note:** placed under `hallucination` but is really **sequence-only generative**
> (autoregressive LM) — a `sequence-generative` sub-category would be more accurate (see ProGen
> note).

## Limitations / disadvantages
- **Sequence-only** — no explicit 3D structure control.
- Generated sequences need folding/validation; novelty/solubility must be checked.
- Less controllable than structure-conditioned methods.

## Benchmarks
- Generated sequences with high predicted structure plausibility; analyzed artificial protein
  sequence spaces. (Source: Ferruz et al., Nat Commun 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41467-023-38246-8
- Code: https://github.com/nferruz/ProtGPT2
