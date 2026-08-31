---
name: Cormorant
field: mlip
category: arch-equivariant
year: 2019
venue: "NeurIPS 2019"
doi: null
doi_note: "NeurIPS paper — no journal DOI; see arXiv 1906.04015"
arxiv: 1906.04015
citations: 496
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/risilab/cormorant
stars: 60
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, covariant, clebsch-gordan, spherical-harmonics]
pioneering: false
status: verified
---

## Key innovation
A rotationally **covariant** molecular network whose activations are spherical-harmonic tensors combined via Clebsch–Gordan tensor products operating largely in Fourier space. Cormorant was among the first fully covariant molecular NNs to demonstrate that built-in SO(3) covariance improves learning of the potential-energy surface, delivering strong results on MD17 and competitive accuracy on QM9. It validated the equivariant design philosophy that later dominated the field.

## Limitations / disadvantages
- Clebsch–Gordan tensor products are **expensive** and the model is heavier than contemporaneous invariant nets.
- Superseded on both accuracy and efficiency by later equivariant designs (PaiNN, NequIP, MACE).
- Gains over well-tuned invariant baselines were present but modest on some targets.

## Benchmarks
- **MD17**: energy/force errors competitive with or better than SchNet/DimeNet-era invariant models. (Source: Anderson, Hy, Kondor, NeurIPS 2019.)
- **QM9**: competitive property-prediction MAE across multiple targets.

## Sources
- Preprint: https://arxiv.org/abs/1906.04015
- Code: https://github.com/risilab/cormorant
