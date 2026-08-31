---
name: NequIP (Neural Equivariant Interatomic Potentials)
field: mlip
category: arch-equivariant
year: 2021
venue: "Nature Communications 13, 3829 (2022)"
doi: 10.1038/s41467-022-29939-5
arxiv: 2101.03164
citations: 2151
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/mir-group/nequip
stars: 933
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, e3, data-efficient, message-passing, biomolecular]
pioneering: true
status: verified
---

## Key innovation
An **E(3)-equivariant (including inversion/parity) message-passing NN** built from spherical-harmonic Clebsch–Gordan tensor products (the e3nn formulation). NequIP's headline result was **remarkable data efficiency**: reaching ab-initio accuracy from orders of magnitude fewer training frames than invariant models, by virtue of encoding the full rotation/parity symmetry of the PES. It became the workhorse for materials and biomolecular MLPs and the reference for the modern equivariant-MPNN recipe (later extended to Allegro and SevenNet).

## Limitations / disadvantages
- Tensor products at higher angular momenta / larger cutoffs are **expensive**; training cost grows with body order.
- **Message passing** limits scaling to very large systems — motivating the local, parallel Allegro design.
- Still requires per-system training for the very highest accuracy (foundation models came later).

## Benchmarks
- Demonstrated DFT-level accuracy on **liquid water and LiPS** using ~hundreds to thousands of frames, versus tens of thousands for invariant baselines. (Source: Batzner et al., Nature Commun. 2022.)

## Sources
- Paper: https://doi.org/10.1038/s41467-022-29939-5
- Preprint: https://arxiv.org/abs/2101.03164
- Code: https://github.com/mir-group/nequip
- Library (e3nn): https://github.com/e3nn/e3nn
