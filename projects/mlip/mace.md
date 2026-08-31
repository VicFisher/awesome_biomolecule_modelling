---
name: MACE
field: mlip
category: arch-equivariant
year: 2022
venue: "NeurIPS 2022"
doi: null
doi_note: "NeurIPS paper — no journal DOI; arXiv-only DOI 10.48550/arXiv.2206.07697"
arxiv: 2206.07697
citations: 1155
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/ACEsuit/mace
stars: 1300
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, many-body, ace, message-passing, foundational]
pioneering: true
status: verified
---

## Key innovation
An equivariant MPNN that injects **higher-body-order messages via an Atomic Cluster Expansion (ACE)** inside each message, so that **only two message-passing layers** suffice to reach state-of-the-art accuracy at high throughput. MACE resolved the central tradeoff of the field: many-body body-order (previously requiring many deep MPNN layers) is captured in a single equivariant layer, giving both the accuracy of high body order and the speed of shallow nets. It is now the **architectural base of most current foundation MLIPs** (MACE-MP-0, MACE-OFF).

## Limitations / disadvantages
- Higher angular momenta remain **costly**; the ACE readout adds implementation complexity.
- Foundation-model variants are **data-hungry** and benefit from large curated training sets.
- Two-layer design can under-fit extremely heterogeneous element spaces without careful tuning.

## Benchmarks
- **rMD17 / MD17**: SOTA energy/force RMSE at release, often halving prior errors.
- **QM9**: leading property-prediction MAE (e.g., U0 in the low-meV range). (Source: Batatia et al., NeurIPS 2022 / arXiv 2206.07697.)

## Sources
- Preprint: https://arxiv.org/abs/2206.07697
- Code: https://github.com/ACEsuit/mace
