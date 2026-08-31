---
name: "Deep network hallucination (trRosetta/AF2)"
field: design
category: hallucination
year: 2021
venue: "Nature 596, 141–145 (2021); 'De novo design of protein structure and function with deep network hallucination'"
doi: 10.1038/s41586-021-04149-2
citations: null
citations_note: "S2 lookup returned 404 on this DOI — to backfill (paper is highly cited)"
repo: null
tags: [hallucination]
pioneering: true
status: draft
institution: "Baker Lab (UW / IPD) — Anishchenko et al."
---

## Key innovation
Inverted structure-predictor networks (trRosetta, then AlphaFold2) by **gradient descent in sequence
space** to "hallucinate" novel folds that the network scores as highly confident. Many designs were
experimentally validated — defining the **hallucination paradigm** for de novo protein design and
seeding constrained/symmetric hallucination and motif-scaffolding variants.

## Limitations / disadvantages
- **Optimization-based** — slow, stochastic, and hard to constrain precisely.
- Sequence-space search offers limited explicit control over 3D structure/function.
- Largely superseded for de novo generation by diffusion models (RFdiffusion, Chroma).

## Benchmarks
- De novo designs solved by X-ray/cryo-EM matched the hallucinated models. (Source: Anishchenko et
  al., Nature 2021.)

## Sources
- Paper: https://doi.org/10.1038/s41586-021-04149-2
