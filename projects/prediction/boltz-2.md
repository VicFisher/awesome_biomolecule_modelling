---
name: Boltz-2
field: prediction
category: all-atom-cofolding
year: 2025
venue: "bioRxiv (2025); Boltz-2"
doi: 10.1101/2025.06.14.659707
citations: 422
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/jwohlwend/boltz
stars: 4090
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT
institution: MIT / Recursion
tags: [msa-based, all-atom, cofolding, diffusion]
status: verified
---

## Key innovation
Successor to Boltz-1 — an open-source **diffusion-based all-atom co-folding** model (proteins,
nucleic acids, ligands, ions) that notably **adds binding-affinity prediction approaching FEP-level
accuracy**, plus improved complex/pose accuracy. Strengthens the open-source AF3-class option set
alongside Chai-1 and Protenix.

## Limitations / disadvantages
- Very recent → limited independent validation; inherits AF3-style diffusion artifacts.
- Affinity prediction is still approximate (not a replacement for rigorous FEP).
- Compute-heavy; confidence calibration for complexes still developing.

## Benchmarks
- Reported gains over Boltz-1 / AlphaFold3 on complex-structure and affinity benchmarks.
  (Source: Boltz-2 preprint, bioRxiv 2025.)

## Sources
- Preprint: https://doi.org/10.1101/2025.06.14.659707
- Code: https://github.com/jwohlwend/boltz
