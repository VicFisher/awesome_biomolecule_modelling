---
name: OMol25 / eqV2
field: mlip
category: foundational-universal
year: 2025
venue: "arXiv preprint (2025)"
doi: null
doi_note: "Preprint; no journal DOI yet"
arxiv: 2505.08762
citations: 83
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/facebookresearch/fair-chem
stars: null
stars_note: "shields.io count did not resolve at lookup time — to backfill"
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [foundational-universal, foundational, universal, equivariant, large-scale-data, molecular]
pioneering: false
status: verified
---

## Key innovation
A flagship open release pairing a **100M+-calculation DFT dataset (OMol25)** at ωB97M-V/def2-TZVPD across 83 elements (systems up to ~350 atoms) with baseline **eqV2 equivariant models** that exhibit **power-law scaling** of accuracy with data and parameters. OMol25 dramatically expands the size and quality of openly available molecular QM data, and the eqV2 potentials are strong transferable molecular foundation models — among the most relevant large-scale open releases for organic and (by extension) biomolecular MLIPs.

## Limitations / disadvantages
- **Huge dataset and model** — meaningful compute is required to fine-tune or even run the largest variants.
- Preprint (2025); downstream benchmark coverage is still maturing.
- Molecular / organic focus; condensed-phase and materials behavior less central.

## Benchmarks
- Power-law accuracy improvement with data/model scale on the OMol25 evaluation suite; leading transferable molecular MLP quality at release. (Source: Levine et al., FAIR-Chem, arXiv 2505.08762, 2025.)

## Sources
- Preprint: https://arxiv.org/abs/2505.08762
- Code & models: https://github.com/facebookresearch/fair-chem
