---
name: Chai-1
field: prediction
category: all-atom-cofolding
year: 2024
venue: "bioRxiv (2024); 'Chai-1: Decoding the molecular interactions of life'"
doi: 10.1101/2024.10.10.615955
citations: 370
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/chaidiscovery/chai-lab
stars: "~2k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: Apache-2.0 (weights)
tags: [msa-based, all-atom, cofolding, diffusion]
status: verified
---

## Key innovation
A **multi-modal foundation model** for all-atom biomolecular structure prediction (proteins,
nucleic acids, small-molecule ligands, ions). Reported **state-of-the-art on several
benchmarks**, including antibody–antigen and chemically-modified components, with **open
weights** — a direct commercial/open competitor to AF3 and Boltz.

## Limitations / disadvantages
- Very recent → limited **independent** validation; ~AF3-class limitations (diffusion
  artifacts, static output).
- Compute-heavy; confidence calibration for ligand/complex pose accuracy still developing.

## Benchmarks
- Reported SOTA on the paper's multi-task benchmark (proteins, complexes, ligands, nucleic
  acids). (Source: Boitreaud et al., bioRxiv 2024.)

## Sources
- Preprint: https://doi.org/10.1101/2024.10.10.615955
- Code: https://github.com/chaidiscovery/chai-lab
