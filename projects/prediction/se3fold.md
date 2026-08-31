---
name: SE(3)-Fold
field: prediction
category: msa-free-equivariant
year: 2021
venue: "bioRxiv (2021)"
doi: 10.1101/2021.06.06.447297
arxiv: null
citations: 11
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
stars: null
stars_source: null
stars_as_of: 2026-07-04
license: null
tags: [msa-free-equivariant, energy-based, se3-equivariant, single-sequence]
pioneering: true
status: verified
---

## Key innovation
An early **end-to-end, single-sequence protein folder formulated as an SE(3)-equivariant energy-based
model** (Tencent AI Lab / ETH / Texas A&M). It uses an SE(3)-equivariant graph neural network to define
an energy over backbone coordinates and samples structures with continuously-annealed Langevin dynamics
— **no MSA and no protein language model**, a coordinate-native equivariant approach predating much of
the MSA-free literature.

## Limitations / disadvantages
- Accuracy lags AlphaFold2-class MSA-based folders; the energy-sampling formulation is computationally
  heavier and less stable than direct regression of coordinates.
- Small community footprint (low citations, no public code release).
- Demonstrated on a limited benchmark set; generalization to large multimeric proteins not shown.

## Benchmarks
- Reported plausible single-sequence folding on a curated benchmark, framing structure prediction as
  Boltzmann-like sampling rather than point estimation. (Source: Wu et al., bioRxiv 2021,
  10.1101/2021.06.06.447297.)

## Sources
- Paper: https://doi.org/10.1101/2021.06.06.447297
