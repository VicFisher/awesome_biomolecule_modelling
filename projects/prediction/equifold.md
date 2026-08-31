---
name: EquiFold
field: prediction
category: msa-free-equivariant
year: 2022
venue: "bioRxiv (2022); 'EquiFold: Protein Structure Prediction with a Novel Equivariant Architecture'"
doi: 10.1101/2022.10.07.511322
citations: 51
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/Genentech/equifold
stars: 129
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Genentech / Prescient Design
tags: [msa-free, equivariant-framework, all-atom]
status: verified
---

## Key innovation
A **purely SE(3)-equivariant**, end-to-end **diffusion-based** protein folder that predicts
all-atom coordinates directly — a canonical member of the **MSA-free / equivariant-framework**
family (no protein language model, no deep MSA). Demonstrated that an equivariant coordinate
diffusion architecture can fold proteins without the Evoformer+IPA paradigm.

## Limitations / disadvantages
- Single-chain/all-atom folding accuracy below AlphaFold2/AF3 in most settings.
- Commercial origin (Genentech) — limited adoption; fewer downstream users.
- Diffusion sampling is slower than single-forward-pass folders.

## Benchmarks
- Competitive on single-chain benchmarks among non-AF2 architectures; below AF2 overall.
  (Source: EquiFold preprint, bioRxiv 2022.)

## Sources
- Preprint: https://doi.org/10.1101/2022.10.07.511322
- Code: https://github.com/Genentech/equifold
