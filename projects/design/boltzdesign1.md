---
name: BoltzDesign1
field: design
category: all-atom-binder-motif
year: 2025
venue: "bioRxiv (2025); 'BoltzDesign1: Inverting All-Atom Structure Prediction Model'"
doi: 10.1101/2025.04.06.647261
repo: https://github.com/jwohlwend/boltz
stars: "~4.1k"
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
citations: 37
citations_source: semantic-scholar
citations_as_of: 2026-07-06
license: MIT
tags: [all-atom, binder]
status: draft
institution: "MIT CSAIL / Jameel Clinic (Hannes Stärk et al.)"
---

## Key innovation
**Inverts the Boltz-1** (open-source AlphaFold3) model for **protein binder design** — showing that
AF3-class co-folders can be turned into all-atom design engines. The direct predecessor to
BoltzGen, it established the "invert an all-atom predictor for design" recipe in the open ecosystem.

## Limitations / disadvantages
- Superseded by BoltzGen (which adds a full generative model on Boltz-2).
- Inversion-based (not a native generative model); binders need validation.
- Sensitive to the underlying co-folder's accuracy/confidence.

## Benchmarks
- All-atom binder design by inverting Boltz-1 (per preprint). (Source: BoltzDesign1, bioRxiv 2025.)

## Sources
- Preprint: https://doi.org/10.1101/2025.04.06.647261
- Code: https://github.com/jwohlwend/boltz
