---
name: DRFold
field: prediction
category: rna
year: 2023
venue: "Nature Methods (2023); RNA tertiary structure prediction"
citations: null
citations_note: "S2 lookup throttled — to backfill"
repo: null
tags: [rna, msa-based]
status: draft
institution: "Zhang lab (Li et al.)"
---

## Key innovation
Integrates **end-to-end learning with deep geometric potentials** for **RNA tertiary structure
prediction** — jointly learning local-frame rotations and geometric restraints. Reported **>70%
accuracy improvement** over traditional (physics/template) RNA approaches.

## Limitations / disadvantages
- **RNA-only** and largely single-chain; accuracy still modest (CASP15: RNA 3D prediction is an
  "unsolved problem" — see [`doc/shortcomings.md`](../../doc/shortcomings.md) §1.6).
- MSA/template-dependent; large RNAs and complexes remain hard.

## Benchmarks
- Ranked 2nd among DL RNA folders in an independent systematic benchmark (PLOS Comp Biol 2024).
  (Source: DRFold, Nat Methods 2023.)

## Sources
- Paper: https://pmc.ncbi.nlm.nih.gov/articles/PMC10505173/
