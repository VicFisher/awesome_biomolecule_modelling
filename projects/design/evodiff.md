---
name: EvoDiff
field: design
category: diffusion-flow
year: 2023
venue: "bioRxiv (2023); 'Protein generation with evolutionary diffusion'"
citations: null
citations_note: "S2 lookup throttled (429) — to backfill"
repo: https://github.com/microsoft/evodiff
stars: 672
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT (Microsoft)
tags: [diffusion-flow, sequence-generative]
status: draft
---

## Key innovation
Diffusion in **sequence space** (and structure) — generates proteins from sequence alone using
evolutionary-scale diffusion, complementary to structure-space diffusion (RFdiffusion/Chroma). Shows
that sequence-based generative diffusion can produce controllable, designable proteins.

## Limitations / disadvantages
- Sequence-space diffusion gives limited explicit **3D structure control**.
- Outputs need folding/validation; novelty/structure plausibility must be checked.
- Less widely adopted than structure-diffusion or ProteinMPNN pipelines.

## Benchmarks
- Controllable generation; functional protein examples reported. (Source: Alamdari et al., bioRxiv
  2023.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.1101/2023.09.11.556817
- Code: https://github.com/microsoft/evodiff
