---
name: JAX-MD
field: mlip
category: differentiable-md-qmmm
year: 2019
venue: "arXiv preprint (2019); NeurIPS MLSAML workshop"
doi: null
doi_note: "Preprint / workshop paper — no journal DOI"
arxiv: 1912.04232
citations: 41
citations_source: semantic-scholar
citations_as_of: 2026-07-04
citations_note: "S2 count (41) appears to substantially undercount this widely-used framework — to cross-check"
repo: https://github.com/jax-md/jax-md
stars: 1400
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [differentiable-md-qmmm, differentiable-md, jax, gpu-tpu, end-to-end]
pioneering: false
status: verified
---

## Key innovation
An **end-to-end differentiable, GPU/TPU-accelerated MD library** built on JAX, providing neighbor lists, pair and many-body potentials forms, and NVE/NVT/NPT integrators all as composable, autodiff-able functions. Because the entire simulation is written in JAX, force-field parameters — and even functional forms — can be **learned by backpropagating straight through the dynamics**. JAX-MD became a foundational differentiable-physics framework underpinning much of Google's and the broader community's work on learned potentials and differentiable simulation.

## Limitations / disadvantages
- **Python/JAX overhead** for very large classical systems relative to hand-tuned engines (OpenMM, LAMMPS).
- Ecosystem is smaller than OpenMM/GROMACS; fewer prebuilt force fields and analysis tools.
- A **framework**, not a force field — it must be paired with a model/data to be useful.

## Benchmarks
No single headline benchmark; value demonstrated via differentiable optimization of LJ parameters and learned potentials end-to-end through MD. (Source: Schoenholz & Cubuk, arXiv 1912.04232, 2019.)

## Sources
- Preprint: https://arxiv.org/abs/1912.04232
- Code: https://github.com/jax-md/jax-md
- Colab notebooks (docs): https://github.com/jax-md/jax-md
