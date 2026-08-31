---
name: GemNet
field: mlip
category: arch-equivariant
year: 2021
venue: "NeurIPS 2021 (arXiv preprint)"
doi: null
doi_note: "NeurIPS paper; S2 lookup did not resolve a DOI — to backfill"
arxiv: 2106.08903
citations: 624
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/TUM-DAML/gemnet_pytorch
stars: 221
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, directional, two-hop, universal-approximator]
pioneering: false
status: verified
---

## Key innovation
A directed-edge, **two-hop equivariant message-passing** network shown to be a **universal approximator** for invariant predictions on geometric graphs. GemNet combines DimeNet-style directionality with full equivariance and an angular basis, delivering large gains on COLL, MD17, and OC20 — particularly on hard molecules and tasks where long-range directional coupling matters. It marked the practical convergence of the invariant/directional (DimeNet) and equivariant (NequIP/PaiNN) lineages into a single, more expressive design.

## Limitations / disadvantages
- Complex **two-hop message passing** is compute- and memory-heavy.
- Largely superseded by MACE, which achieves better accuracy-per-cost via many-body ACE messages in fewer layers.
- Heavy to train at scale; less used as a "production" force field than Allegro/MACE today.

## Benchmarks
- **MD17 / COLL / OC20**: substantial error reductions versus PaiNN/DimeNet++ at release, especially on the hardest targets. (Source: Gasteiger, Becker, Günnemann, NeurIPS 2021 / arXiv 2106.08903.)

## Sources
- Preprint: https://arxiv.org/abs/2106.08903
- Code: https://github.com/TUM-DAML/gemnet_pytorch
