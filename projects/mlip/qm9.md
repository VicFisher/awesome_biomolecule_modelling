---
name: QM9
field: mlip
category: qm-datasets
year: 2014
venue: "Scientific Data 1, 140022 (2014)"
doi: 10.1038/sdata.2014.22
arxiv: null
arxiv_note: "No arXiv preprint — published directly in Scientific Data"
citations: 2362
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "Distributed via quantum-machine.org / DeepChem; no single canonical repo"
stars: null
stars_note: "No canonical repo to count"
tags: [qm-datasets, qm-data, small-molecules, property-prediction]
pioneering: false
status: verified
---

## Key innovation
A benchmark of **~134k DFT-optimized small organic molecules** (C, N, O, H, F; up to 9 heavy atoms, "GDB-17" subset) with a full slate of B3LYP/6-31G(2df,p) properties — energies, enthalpies, free energies, HOMO/LUMO, gap, dipole moment, polarizability, and heat capacity. QM9 became the **canonical quantum-chemical property-prediction benchmark** for a decade: nearly every geometric GNN reports QM9 MAE as a headline result.

## Limitations / disadvantages
- Molecules are **tiny** (≤ 9 heavy atoms) and at **equilibrium only** (no MD/displaced conformers).
- DFT level (B3LYP/6-31G(2df,p)) is now dated; some labels carry systematic error.
- Benchmarks are **saturated**: top models sit near the label-noise floor, so QM9 no longer discriminates architectures well.

## Benchmarks
Task: **property MAE** (U0, U0_atom, H, G, εHOMO, εLUMO, gap, μ, α, Cv, ZPVE). Representative: SchNet U0 ≈ 14 meV; DimeNet U0 ≈ 8–9 meV; MACE reaches the low-meV range and SOTA on most targets. (Source: Ramakrishnan et al., Sci. Data 2014; subsequent model papers.)

## Sources
- Paper: https://doi.org/10.1038/sdata.2014.22
- Data: http://quantum-machine.org/datasets/
- MoleculeNet entry: https://moleculenet.org/datasets-1
