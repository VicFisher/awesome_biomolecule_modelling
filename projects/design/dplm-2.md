---
name: DPLM-2
field: design
category: inverse-folding
year: 2024
venue: "ICLR 2025; 'DPLM-2: A Multimodal Diffusion Protein Language Model'"
arxiv: 2410.13782
repo: https://github.com/bytedance/dplm
stars: 338
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
citations: 74
citations_source: semantic-scholar
citations_as_of: 2026-07-04
license: Apache-2.0
tags: [inverse-folding, sequence-generative, diffusion, all-atom]
status: draft
institution: ByteDance
---

## Key innovation
A **multimodal discrete diffusion model** that **jointly generates protein sequence and 3D
structure**, removing the need for a separate structure-prediction module in sequence design.
Extends DPLM from sequence-only to sequence+structure co-generation.

## Limitations / disadvantages
- Very recent; limited independent benchmarking.
- Joint sequence-structure diffusion is compute-heavy and tuning-sensitive.
- Structure accuracy below dedicated predictors (AF3-class).

## Benchmarks
- Competitive joint sequence+structure generation; reported gains on structure-conditioned design
  vs sequence-only diffusion. (Source: DPLM-2, ICLR 2025.)

## Sources
- Paper: https://arxiv.org/abs/2410.13782
- Code: https://github.com/bytedance/dplm
