---
name: SevenNet
field: mlip
category: foundational-universal
year: 2024
venue: "J. Chem. Theory Comput. (2024)"
doi: 10.1021/acs.jctc.4c00190
arxiv: 2402.03789
citations: 250
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/MDIL-SNU/SevenNet
stars: null
stars_note: "shields.io count did not resolve at lookup time — to backfill"
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: GPL-3.0
tags: [foundational-universal, foundational, universal, equivariant, scalable, nequip-based]
pioneering: false
status: verified
---

## Key innovation
A **NequIP-based equivariant potential** paired with a **CUDA-aware MPI parallelization** scheme that lets message-passing equivariant GNNs run efficient multi-GPU molecular dynamics. The pretrained **SevenNet-latest** model is a competitive universal materials force field. SevenNet demonstrated that the accuracy benefits of equivariant MPNNs need not be sacrificed for production-scale MD throughput, and it has become a widely used open universal potential in the materials community.

## Limitations / disadvantages
- Scalability is still bounded by the **message-passing** communication pattern.
- Peak accuracy is generally below MACE-class models on some benchmarks.
- Smaller community than MACE; GPL license may restrict some commercial use.

## Benchmarks
- Competitive universal-materials accuracy on Matbench-Discovery-class and phonon benchmarks; efficient parallel MD demonstrated up to large cell sizes. (Source: Park et al., JCTC 2024 / arXiv 2402.03789.)

## Sources
- Paper: https://doi.org/10.1021/acs.jctc.4c00190
- Preprint: https://arxiv.org/abs/2402.03789
- Code: https://github.com/MDIL-SNU/SevenNet
