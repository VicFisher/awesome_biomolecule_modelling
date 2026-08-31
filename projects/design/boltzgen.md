---
name: BoltzGen
field: design
category: all-atom-binder-motif
year: 2025
venue: "bioRxiv (2025); 'BoltzGen: Toward Universal Binder Design'"
doi: 10.1101/2025.11.20.689494
repo: https://github.com/jwohlwend/boltz
stars: "~4.1k"
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
citations: 70
citations_source: semantic-scholar
citations_as_of: 2026-07-06
license: MIT
tags: [all-atom, binder, diffusion]
status: draft
institution: "MIT CSAIL / Jameel Clinic (Hannes Stärk et al.)"
---

## Key innovation
An **all-atom generative model for universal binder design**, built on **Boltz-2**. It unifies the
co-design of binder sequence + 3D structure across modalities (proteins and peptides) to bind a
wide range of biomolecular targets, and generalizes to **novel/unseen targets without
target-specific retraining** — using a purely geometry-based generative objective.

## Limitations / disadvantages
- Very recent (Nov 2025); binders require experimental validation.
- Inherits diffusion/co-folder artifacts (stereochemistry, static output).
- Compute-heavy; confidence/affinity calibration still maturing.

## Benchmarks
- Universal binder design across diverse target types and modalities (per preprint). (Source:
  BoltzGen, bioRxiv 2025.)

## Sources
- Preprint: https://doi.org/10.1101/2025.11.20.689494
- Code: https://github.com/jwohlwend/boltz
