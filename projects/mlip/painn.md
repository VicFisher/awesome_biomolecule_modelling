---
name: PaiNN (Polarizable Atom Interaction NN)
field: mlip
category: arch-equivariant
year: 2021
venue: "ICML 2021"
doi: null
doi_note: "ICML paper — no journal DOI; see arXiv 2102.03150"
arxiv: 2102.03150
citations: 789
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/atomistic-machine-learning/schnetpack
stars: 934
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, message-passing, tensorial, spectra]
pioneering: false
status: verified
---

## Key innovation
Extends message passing to maintain **both scalar and vector representations per atom**, updated equivariantly using only simple distance-based messages — achieving equivariance with L = 0,1 features and small, fast models. PaiNN reached **SOTA on MD17** at release and predicted tensorial properties and molecular **spectra** with four-to-five orders of magnitude speedup over DFT. It demonstrated that equivariance does not require the heavy higher-order tensors of Cormorant/TFN, becoming a popular accurate-yet-cheap baseline inside SchNetPack.

## Limitations / disadvantages
- Limited to L ≤ 1 (scalar + vector); no explicit higher-order angular information.
- Local cutoff; no built-in long-range electrostatics/dispersion.
- Superseded on broad benchmarks by many-body designs (MACE) that achieve better accuracy-per-cost.

## Benchmarks
- **MD17**: SOTA energy/force RMSE at release across the molecule set. (Source: Schütt, Unke, Gastegger, ICML 2021.)
- **Spectra/tensorial properties**: DFT-quality predictions at 10⁴–10⁵× the speed.

## Sources
- Preprint: https://arxiv.org/abs/2102.03150
- Code (SchNetPack): https://github.com/atomistic-machine-learning/schnetpack
