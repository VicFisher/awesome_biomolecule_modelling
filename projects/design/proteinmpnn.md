---
name: ProteinMPNN
field: design
category: inverse-folding
year: 2022
venue: "Science 378, 49–56 (2022); 'Robust deep learning-based protein sequence design using ProteinMPNN'"
doi: 10.1126/science.add2187
citations: 1851
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/dauparas/ProteinMPNN
stars: "~1.8k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT
tags: [inverse-folding]
pioneering: true
status: verified
---

## Key innovation
A message-passing graph neural network for **fixed-backbone inverse folding** (backbone → sequence)
that is robust to imperfect/non-ideal backbones. It became the default sequence-design component
across nearly every modern design pipeline (paired downstream of RFdiffusion/Chroma), displacing
Rosetta-based sequence design. Fast, simple, and remarkably effective.

## Limitations / disadvantages
- **Sequence-only** output — no all-atom/ligand context in the base model (LigandMPNN addresses
  this).
- Assumes a **fixed input backbone**; does not redesign structure.
- Designed sequences still require **folding/validation** (AF2/MPNN round-trip) and can occasionally
  fail designability checks.
- No explicit multi-state or controllability.

## Benchmarks
- Sequence recovery ~**52%** on native backbones (vs ~32–44% for Rosetta). (Source: Dauparas et
  al., Science 2022.)

## Sources
- Paper: https://doi.org/10.1126/science.add2187
- Code: https://github.com/dauparas/ProteinMPNN
