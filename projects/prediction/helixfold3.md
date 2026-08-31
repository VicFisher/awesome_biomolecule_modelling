---
name: HelixFold3
field: prediction
category: all-atom-cofolding
year: 2024
venue: "arXiv 2408.16975 (2024)"
arxiv: 2408.16975
citations: 34
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/PaddlePaddle/PaddleHelix
stars: 1114
stars_source: "shields.io (approx) — shared PaddleHelix repo"
stars_as_of: 2026-07-04
institution: Baidu
license: Apache-2.0
tags: [msa-based, all-atom, cofolding, diffusion]
status: draft
---

## Key innovation
An open-source **AlphaFold3 reproduction** built on Baidu's **PaddlePaddle** framework, providing a
competitive all-atom co-folding model with full training/inference code. Part of the AF3-era open
ecosystem (alongside Boltz, Chai-1, Protenix).

## Limitations / disadvantages
- Implemented in **PaddlePaddle** (less mainstream than PyTorch), limiting adoption/integration.
- A reproduction; inherits AF3 diffusion artifacts.
- Compute-heavy.

## Benchmarks
- Reported AF3-comparable accuracy on complex benchmarks (per preprint). (Source: HelixFold3,
  arXiv 2408.16975.)

## Sources
- Preprint: https://arxiv.org/abs/2408.16975
- Code: https://github.com/PaddlePaddle/PaddleHelix
