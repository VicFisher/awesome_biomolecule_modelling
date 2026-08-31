---
name: EquiformerV2
field: mlip
category: arch-equivariant
year: 2024
venue: "ICLR 2024; improved equivariant transformer scaling to higher-degree representations"
citations: null
citations_note: "S2 lookup throttled — to backfill"
repo: https://github.com/atomicarchitects/equiformer_v2
stars: 345
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
tags: [arch-equivariant, equivariant, transformer]
status: verified
institution: "Atomic Architects (Shi, Lin, Wang, Jaakkola, Ringers, Koker, Smidt)"
---

## Key innovation
An **improved equivariant transformer** that scales to **higher-degree equivariant representations**
(feeding higher-L spherical harmonics through attention). A key backbone for large-scale/foundational
MLIPs — e.g., it underpins Meta's **eqV2 / OMol25** model.

## Limitations / disadvantages
- Higher angular degree is **compute-expensive** (scales with L).
- An architecture/backbone — needs a large training set to realize its advantage.
- More complex to implement/tune than simpler equivariant MPNNs (NequIP/Allegro).

## Benchmarks
- SOTA on OC20/OC22 (Open Catalyst) at release. (Source: EquiformerV2, ICLR 2024.)

## Sources
- Code: https://github.com/atomicarchitects/equiformer_v2
