---
name: Allegro
field: mlip
category: arch-equivariant
year: 2022
venue: "Nature Communications 14, 3645 (2023)"
doi: 10.1038/s41467-023-36329-y
arxiv: 2204.05249
citations: 800
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/mir-group/allegro
stars: 490
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, local, scalable]
pioneering: false
status: verified
---

## Key innovation
A **strictly local (non-message-passing) equivariant potential**: each atom's representation is built from its own neighborhood via equivariant operations, so the computation is **embarrassingly parallel** across atoms and GPUs. Allegro combines NequIP-level accuracy with scalability to **100-million-atom simulations** on GPUs, decoupling equivariance from graph propagation. It demonstrated that one can keep the accuracy benefits of E(3)-equivariance while escaping the scaling limits of message-passing nets.

## Limitations / disadvantages
- Receptive field is capped by a **single local layer** (larger cutoffs are needed to compensate).
- Memory-hungry at extreme scale; per-system training still required for best accuracy.
- Strictly local — no explicit long-range electrostatics/dispersion.

## Benchmarks
- Matched NequIP accuracy on benchmark systems while scaling to **>100M atoms** (LiPS MD); strong performance on oxide and metal systems. (Source: Musaelian et al., Nature Commun. 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41467-023-36329-y
- Preprint: https://arxiv.org/abs/2204.05249
- Code: https://github.com/mir-group/allegro
