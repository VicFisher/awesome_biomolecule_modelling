---
name: Distributional Graphormer (DiG)
field: prediction
category: msa-free-equivariant
year: 2023
venue: "Nature Machine Intelligence (2024)"
doi: 10.1038/s42256-024-00837-3
arxiv: 2306.05445
citations: 152
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/microsoft/Graphormer
stars: "2.5k"
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [msa-free-equivariant, diffusion, distributional, equilibrium]
pioneering: false
status: verified
_note: "Backbone is Graphormer (a spatial-encoding transformer), not strictly SE(3)-equivariant/IPA; placed in msa-free-equivariant because the contribution is distributional structure prediction, single-sequence and coordinate-native."
---

## Key innovation
A Microsoft Research model that **predicts the equilibrium distribution of molecular structures**
rather than a single conformation, using a diffusion model with a Graphormer backbone. By targeting
*distributions* it can capture conformational heterogeneity (e.g. alternative states, flexibility) and
was extended beyond proteins to small molecules and biomolecular assemblies — framing structure
prediction as a distributional / thermodynamic problem.

## Limitations / disadvantages
- Distributional prediction is harder to evaluate and to validate experimentally than point prediction.
- Graphormer is a spatial-attention transformer, **not** a strictly SE(3)-equivariant architecture, so
  equivariance is only approximate.
- Sample quality per-conformation still trails dedicated point predictors like AlphaFold2.

## Benchmarks
- Demonstrated recovery of known alternative conformations and reasonable ensemble statistics on
  protein and molecular benchmarks; designability validated via MPNN/ESMFold round-trips. (Source: Zheng
  et al., Nature Machine Intelligence 2024, 10.1038/s42256-024-00837-3.)

## Sources
- Paper: https://doi.org/10.1038/s42256-024-00837-3
- Preprint: https://arxiv.org/abs/2306.05445
- Code: https://github.com/microsoft/Graphormer
