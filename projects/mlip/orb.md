---
name: Orb
field: mlip
category: foundational-universal
year: 2024
venue: "arXiv preprint (2024)"
doi: null
doi_note: "Preprint; arXiv-only DOI 10.48550/arXiv.2410.22570"
arxiv: 2410.22570
citations: 147
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/orbital-materials/orb-models
stars: 602
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [foundational-universal, foundational, universal, scalable, fast, diffusion-pretrained]
pioneering: false
status: verified
---

## Key innovation
A family of **universal interatomic potentials 3–6× faster than prior universal potentials** while achieving SOTA on the Matbench-Discovery benchmark. Orb uses **diffusion pretraining** on structures to initialize the potential, then trains on DFT — connecting generative-model insights with force-field learning for materials geometry optimization and MD. Developed by a commercial vendor (Orbital Materials) with openly released weights, it is a leading example of industry-produced open universal MLPs.

## Limitations / disadvantages
- Focused on **inorganic materials** discovery; not biomolecule-oriented.
- Preprint lineage; benchmark coverage skews to materials-discovery tasks (Matbench).
- Diffusion pretraining adds training-stage complexity.

## Benchmarks
- **Matbench-Discovery**: SOTA among universal potentials at release.
- 3–6× faster inference than competing universal models (MACE-MP-0, CHGNet, M3GNet-class). (Source: Neumann et al., arXiv 2410.22570, 2024.)

## Sources
- Preprint: https://arxiv.org/abs/2410.22570
- Code & weights: https://github.com/orbital-materials/orb-models
