---
name: RaptorX-Contact
field: prediction
category: pre-dl-contact
year: 2017
venue: "PLOS Computational Biology 12(12), e1005324 (2016)"
doi: 10.1371/journal.pcbi.1005324
citations: 872
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/j3xugit/RaptorX-Contact
stars: 79
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [pre-dl-contact]
pioneering: true
status: verified
---

## Key innovation
The first **ultra-deep residual convolutional network** for protein **contact-map**
prediction, integrating evolutionary-coupling and sequence-conservation features. It pioneered
deep-learning contact prediction and ranked among the top methods at CASP12, establishing that
deep nets could substantially beat DCA-only contact inference.

## Limitations / disadvantages
- Predicts **binary contacts only** — no distances or orientations, and not end-to-end folding.
- **MSA-dependent**; two-stage (contact map → separate folding).
- Quickly superseded by distance/orientation predictors (trRosetta) and end-to-end models
  (AF2).

## Benchmarks
- Top contact-prediction precision at CASP12; later extended to distance-based folding
  (PNAS 2019, 10.1073/pnas.1821309116). (Source: Wang et al., PLOS Comp Biol 2016.)

## Sources
- Paper: https://doi.org/10.1371/journal.pcbi.1005324
- Code: https://github.com/j3xugit/RaptorX-Contact
