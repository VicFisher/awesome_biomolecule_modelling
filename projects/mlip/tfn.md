---
name: Tensor Field Networks (TFN)
field: mlip
category: arch-equivariant
year: 2018
venue: "arXiv preprint (2018)"
doi: null
doi_note: "Preprint only — no journal DOI"
arxiv: 1802.08219
citations: 1211
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "No official repo; ideas realized downstream via the e3nn library"
stars: null
stars_note: "No canonical repo to count"
tags: [arch-equivariant, equivariant, spherical-harmonics, clebsch-gordan]
pioneering: false
status: verified
---

## Key innovation
The foundational **SE(3)-equivariant network**: convolutions use spherical-harmonic filters whose outputs transform as definite-angular-momentum (L = 0, 1, 2, …) tensors, so scalars, vectors, and higher-rank tensors are carried equivariantly through every layer. By applying learnable radial functions to interatomic distances and coupling channels via Clebsch–Gordan products, TFN made it possible to predict vector/tensor molecular properties (forces, dipoles) with the correct geometric transformation built in. It is the **conceptual root** of Cormorant, the SE(3)-Transformer, NequIP, and the broader e3nn ecosystem.

## Limitations / disadvantages
- Preprint with **no canonical code release** of its own; adoption came through reimplementations.
- Higher-rank tensor products are **computationally heavy**, and the original reported only modest molecular-property numbers.
- Largely a proof-of-concept; later equivariant nets (NequIP, PaiNN, MACE) delivered the practical accuracy and efficiency.

## Benchmarks
Demonstrated equivariant prediction of molecular energies and multipoles on small datasets (e.g., QM7); the contribution is **architectural** rather than benchmark-leading. (Source: Thomas et al., arXiv 1802.08219.)

## Sources
- Preprint: https://arxiv.org/abs/1802.08219
- Downstream library (e3nn): https://github.com/e3nn/e3nn
