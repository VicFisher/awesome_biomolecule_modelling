---
name: "ANI (ANI-1 / 1x / 2x)"
field: mlip
category: arch-invariant
year: 2016
venue: "Chemical Science 8, 3192 (2017)"
doi: 10.1039/c6sc05720a
arxiv: 1610.08935
citations: 1340
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/aiqm/torchani
stars: 548
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-invariant, invariant, atomic-descriptors, transferable, biomolecular]
pioneering: true
status: verified
---

## Key innovation
A family of per-element **neural network potentials over modified ACSF symmetry-function descriptors**, trained on millions of organic conformations. ANI-1x scaled training via **active learning** (query-by-committee selecting ~5M DFT labels on the ANI-1x dataset), and ANI-2x extended element coverage to H, C, N, O, S, F, Cl. By reaching **near-DFT accuracy at classical-force-field cost** across broad organic chemistry, ANI established the recipe — large transferable training sets + active learning + per-element descriptor NNs — that became standard practice for transferable organic and biomolecular NNPs.

## Limitations / disadvantages
- **Invariant descriptor** basis limits force accuracy versus equivariant models on anisotropic environments.
- Coverage capped at a fixed element set (7 elements in ANI-2x); fails for inorganic, metallic, or ionic chemistry.
- Purely short-range; no explicit charges or dispersion (addressed later by AIMNet2).
- Reliability drops for exotic bonding or charge states outside the training distribution.

## Benchmarks
- **ANI-1x**: sub-kcal/mol mean absolute errors on diverse organic conformer energies versus reference DFT (ωB97X/6-31G*). (Source: Smith, Nebgen, Lubbers, Isayev, Roitberg, Chem. Sci. 2018.)
- **ANI-2x**: an extended-element transferable NNP widely used as a baseline organic MLP and inside OpenMM/TorchMD pipelines.

## Sources
- ANI-1 paper: https://pubs.rsc.org/en/content/articlelanding/2017/sc/c6sc05720a
- Preprint: https://arxiv.org/abs/1610.08935
- Code (TorchANI): https://github.com/aiqm/torchani
- ANI-1x data paper: https://doi.org/10.1038/sdata.2018.312
