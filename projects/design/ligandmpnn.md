---
name: LigandMPNN
field: design
category: inverse-folding
year: 2023
venue: "bioRxiv (2023); 'LigandMPNN: a structure-based sequence design neural network for proteins and protein-ligand complexes'"
doi: 10.1101/2023.12.13.571563
citations: 221
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/dauparas/LigandMPNN
stars: 596
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT
tags: [inverse-folding, all-atom]
status: verified
---

## Key innovation
Extends ProteinMPNN to design sequences **in the presence of ligands, cofactors, ions, and nucleic
acids** — making inverse folding **all-atom aware**. Enables binding-site-context-aware design and
residue constraints, and is now standard in enzyme/binder design pipelines that involve non-protein
components.

## Limitations / disadvantages
- Still conditioned on a fixed input complex geometry (not de novo).
- Backbone/ligand pose assumed correct; sensitive to input quality.
- Sequence-only output (no simultaneous structure redesign).

## Benchmarks
- Improved sequence recovery / binding-site design over ProteinMPNN in ligand contexts.
  (Source: Shuvo et al., bioRxiv 2023.)

## Sources
- Preprint: https://doi.org/10.1101/2023.12.13.571563
- Code: https://github.com/dauparas/LigandMPNN
