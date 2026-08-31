---
name: AlphaFold-Multimer
field: prediction
category: msa-based
year: 2021
venue: "bioRxiv (2021); preprint only"
doi: 10.1101/2021.10.04.463034
citations: 3171
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/deepmind/alphafold
stars: "~15k"
stars_source: "shields.io (approx) — shared with AlphaFold2 repo"
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [msa-based, multimer]
pioneering: true
status: verified
---

## Key innovation
Extended AlphaFold2 to **multi-chain protein complexes** by concatenating per-chain MSAs,
introducing a chain-pairing/assembly scheme, and adapting the loss to inter-chain contacts.
Became the standard baseline for protein–protein interaction structure prediction and seeded
the complex-prediction field before AF3.

## Limitations / disadvantages
- Accuracy drops sharply for **large, asymmetric, or heterogeneous** complexes.
- **Symmetry handling** is imperfect; **antibody–antigen and weak/transient** interactions are
  systematically underpredicted.
- Depends heavily on **paired-MSA quality** (cross-species pairing), which is often unavailable.
- Preprint only (no formal journal version), yet extremely widely cited.

## Benchmarks
- Defined the early PPI benchmark (DockQ / interface metrics on dimers/trimers); later
  superseded on complex benchmarks by AF3-class models. (Source: Evans et al., bioRxiv 2021.)

## Sources
- Preprint: https://doi.org/10.1101/2021.10.04.463034
- Code: https://github.com/deepmind/alphafold (v2.1.0+)
