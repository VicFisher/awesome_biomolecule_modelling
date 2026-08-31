---
name: MatterSim
field: mlip
category: foundational-universal
year: 2024
venue: "arXiv preprint (2024); later Nature (2025)"
doi: null
doi_note: "S2 lookup did not resolve a journal DOI at fetch time — to backfill (Nature 2025 publication)"
arxiv: 2405.04967
citations: 232
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/microsoft/mattersim
stars: 570
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [foundational-universal, foundational, universal, materials, active-learning]
pioneering: false
status: verified
---

## Key innovation
An **actively-learned deep atomistic model** covering the periodic table across 0–5000 K and pressures up to 1000 GPa, trained on a large Microsoft-generated dataset of DFT calculations spanning a wide temperature/pressure/element range. MatterSim reports roughly **10× higher precision than prior best-in-class** universal models and is **fine-tunable to arbitrary theory levels**, positioning it as Microsoft's universal atomistic foundation model for materials simulation.

## Limitations / disadvantages
- Focus is on **inorganic / materials** simulation rather than biomolecules.
- Preprint-to-publication lineage; broad coverage trades off some peak accuracy.
- Large model footprint; fine-tuning to a target benefits from substantial compute.

## Benchmarks
- ~10× lower energy/force error than prior best-in-class on the MatterSim evaluation suite (elements, T, P); fine-tuning demonstrated to other DFT levels. (Source: Yang et al., arXiv 2405.04967, 2024.)

## Sources
- Preprint: https://arxiv.org/abs/2405.04967
- Code: https://github.com/microsoft/mattersim
