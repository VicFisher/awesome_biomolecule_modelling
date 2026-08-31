---
name: EGNN (E(n)-Equivariant GNN)
field: mlip
category: arch-equivariant
year: 2021
venue: "ICML 2021"
doi: null
doi_note: "ICML paper — no journal DOI; see arXiv 2102.09844"
arxiv: 2102.09844
citations: 1539
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/vgsatorras/egnn
stars: 538
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, lightweight, n-dimensional]
pioneering: false
status: verified
---

## Key innovation
A lightweight **E(n)-equivariant GNN** that updates coordinates directly in the message-passing step (squaring distances gives a coordinate update) **without the costly spherical-harmonic / Clebsch–Gordan machinery** of TFN or Cormorant. Simpler and faster than its predecessors and generalizing to arbitrary n-dimensional spaces, EGNN became one of the most-reused building blocks in geometric deep learning — for dynamics, normalizing flows, and especially generative models (diffusion, EBMs) — despite modest accuracy as a force field.

## Limitations / disadvantages
- Uses effectively only scalar (L=0) plus vector (L=1) information; **no explicit higher-order angular features**, so PES/force accuracy trails higher-order equivariant nets.
- Not designed or tuned as a production interatomic potential; gains on MD17 are limited.
- Coordinate updates can be unstable for some generative tasks without careful scheduling.

## Benchmarks
- **QM9**: property-prediction MAE competitive with or better than Cormorant/SE(3)-Transformer at lower cost.
- Achieves equivariant performance at a fraction of the compute of higher-order methods. (Source: Satorras, Hoogeboom, Welling, ICML 2021.)

## Sources
- Preprint: https://arxiv.org/abs/2102.09844
- Code: https://github.com/vgsatorras/egnn
