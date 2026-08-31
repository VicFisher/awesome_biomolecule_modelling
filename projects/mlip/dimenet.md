---
name: DimeNet
field: mlip
category: arch-invariant
year: 2020
venue: "ICLR 2020"
doi: null
doi_note: "ICML paper; S2 lookup did not resolve a DOI — to backfill"
arxiv: 2003.03123
citations: 1118
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/gasteigerjo/dimenet
stars: 357
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-invariant, directional, spherical-bessel, angular]
pioneering: true
status: verified
---

## Key innovation
Introduced **directional message passing**: messages flow not only along atom pairs but along directed atom triples (i, j, k), explicitly incorporating **bond angles** through spherical-Bessel / spherical-harmonic bases. Although the final energy is rotationally invariant, the *intermediate* representations are rotationally equivariant — DimeNet was the first widely-adopted model to show that encoding directional/angle information dramatically cuts error on MD17 and QM9, **bridging the invariant and equivariant eras**. It established spherical-Bessel bases as a staple of geometric GNNs.

## Limitations / disadvantages
- **Computationally expensive**: directional message passing over triples scales as O(N · neighbors²), far heavier than pairwise SchNet.
- Still emits an invariant output; full SE(3)-equivariance came only with later models (NequIP, PaiNN).
- Superseded in speed and accuracy by DimeNet++ and then by fully equivariant MPNNs (GemNet, MACE).

## Benchmarks
- **QM9**: roughly halved SchNet's error on several targets (e.g., U0 MAE ≈ 8–9 meV, εHOMO ≈ 28 meV). (Source: Klicpera et al., ICML 2020.)
- **MD17**: substantial energy/force RMSE reductions versus SchNet across all molecules.

## Sources
- Preprint: https://arxiv.org/abs/2003.03123
- Code: https://github.com/gasteigerjo/dimenet
