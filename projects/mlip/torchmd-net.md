---
name: TorchMD-Net
field: mlip
category: arch-equivariant
year: 2022
venue: "arXiv preprint (2022); published J. Chem. Theory Comput. (2023)"
doi: null
doi_note: "S2 lookup did not resolve the paper — to backfill (later JCTC publication)"
arxiv: 2202.02541
citations: 285
citations_source: semantic-scholar
citations_as_of: 2026-07-06
repo: https://github.com/torchmd/torchmd-net
stars: 478
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, transformer, attention, biomolecular]
pioneering: false
status: verified
---

## Key innovation
An **SE(3)/E(3)-equivariant transformer** that applies attention over scalar + vector atom features to produce molecular potentials, unifying equivariant attention with practical force-field design. TorchMD-Net reached SOTA on MD17, the ANI-1 benchmark, and many QM9 targets at release and is the **backbone of the TorchMD-Net production package** used for biomolecular simulation within the TorchMD ecosystem. Its accessible, well-engineered code made equivariant transformers the default architecture for many applied MLP projects.

## Limitations / disadvantages
- Attention is **O(N²)** in atoms, restricting very large systems without approximation.
- Preprint lineage (formally published in JCTC 2023); some reported numbers shifted between versions.
- Per-task hyperparameter tuning needed for best results.

## Benchmarks
- **MD17**: best or near-best energy/force RMSE among equivariant models at release.
- **ANI-1** and **QM9**: leading accuracy on most targets. (Source: Tholke & De Fabritiis, arXiv 2202.02541.)

## Sources
- Preprint: https://arxiv.org/abs/2202.02541
- Code: https://github.com/torchmd/torchmd-net
