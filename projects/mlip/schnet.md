---
name: SchNet
field: mlip
category: arch-invariant
year: 2017
venue: "NeurIPS 2017"
doi: null
doi_note: "NeurIPS paper — no journal DOI; see arXiv 1706.08566"
arxiv: 1706.08566
citations: 1431
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/atomistic-machine-learning/schnetpack
stars: 934
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-invariant, invariant, message-passing, continuous-filter]
pioneering: true
status: verified
---

## Key innovation
Replaced discrete filter bins with **continuous-filter convolutions**: the convolution filter is generated on the fly by an MLP from the interatomic distance, so the model is smooth and differentiable everywhere and naturally respects rotational/translational invariance. Built as a message-passing graph net over atoms with distances as edges, SchNet jointly predicts energy and forces (forces via analytic gradients) and became the **dominant invariant MPNN baseline** for years. Its packaging as **SchNetPack** made it the reference implementation the field standardized on.

## Limitations / disadvantages
- **Invariant only** — distance features discard explicit directional/angular information, so force accuracy lags equivariant models (DimeNet, NequIP, MACE) on anisotropic systems.
- Fixed local cutoff; no built-in long-range electrostatics or dispersion.
- Modest accuracy on large/flexible molecules (MD22) and on condensed-phase systems versus later equivariant or many-body designs.

## Benchmarks
- **QM9**: U0 MAE ≈ 14 meV and HOMO MAE ≈ 41 meV — among the best invariant models at release. (Source: Schütt et al., NeurIPS 2017.)
- **MD17**: benzene energy MAE ≈ 0.3 kcal/mol, but high force error on flexible molecules such as aspirin, exposing the invariant limit. (Source: SchNet paper / MD17 benchmark.)

## Sources
- Preprint: https://arxiv.org/abs/1706.08566
- Code (SchNetPack): https://github.com/atomistic-machine-learning/schnetpack
