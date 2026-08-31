---
name: trRosetta
field: prediction
category: pre-dl-contact
year: 2020
venue: "PNAS 117(3), 1496–1503 (2020)"
doi: 10.1073/pnas.1914677117
citations: 1268
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/RosettaCommons/trRosetta
stars: 2
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [pre-dl-contact, msa-based]
pioneering: true
status: verified
---

## Key innovation
A deep residual network that predicts **inter-residue distances *and* orientations** (Cβ–Cβ
distance plus φ/θ/ω angles between residue frames) from an MSA, then converts them into
restraints for Rosetta constrained minimization. The key insight — that **orientations, not
just distances, materially improve folding** — directly foreshadowed the pair representations
in AlphaFold2 and RoseTTAFold.

## Limitations / disadvantages
- Two-stage (predict geometry → Rosetta fold), not end-to-end differentiable.
- **MSA-dependent**; accuracy below AF2/RoseTTAFold.
- Slower than modern fast folders (Rosetta minimization); outputs a single structure.

## Benchmarks
- Strong de novo structure prediction on CASP13-hard and CAMEO; demonstrated that adding
  orientations to distances improved models over distance-only methods. (Source: Du et al.,
  PNAS 2020.)

## Sources
- Paper: https://doi.org/10.1073/pnas.1914677117
- Server paper (Nature Protocols 2021): https://doi.org/10.1038/s41596-021-00628-9
- Code: https://github.com/RosettaCommons/trRosetta
