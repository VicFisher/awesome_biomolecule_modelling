---
name: DPLM
field: design
category: inverse-folding
year: 2024
venue: "ICML 2024; 'DPLM: Diffusion Language Models Are Versatile Protein Learners'"
repo: https://github.com/bytedance/dplm
stars: 338
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
license: Apache-2.0
tags: [inverse-folding, sequence-generative, diffusion]
status: draft
institution: ByteDance
---

## Key innovation
A **discrete diffusion model over protein language-model tokens** — showing that a diffusion PLM
gives strong unconditional sequence generation and can be repurposed (e.g. via LM-Design-style
structure injection) for **structure-conditioned sequence design**. Unifies generative sequence
modeling with the PLM prior.

## Limitations / disadvantages
- **Sequence-space** diffusion — limited explicit 3D structure control without conditioning.
- Needs a separate structure module/predictor for inverse-folding use.
- Newer; smaller validation base than ProteinMPNN/RFdiffusion pipelines.

## Benchmarks
- Strong unconditional generation quality; competitive structure-conditioned design when paired
  with structure features. (Source: DPLM, ICML 2024.)

## Sources
- Paper: https://icml.cc/virtual/2024/poster/34203
- Code: https://github.com/bytedance/dplm
