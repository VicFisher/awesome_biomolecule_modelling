---
name: SPICE
field: mlip
category: qm-datasets
year: 2022
venue: "Scientific Data 9, 776 (2022)"
doi: 10.1038/s41597-022-01882-6
arxiv: 2209.10702
citations: 236
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/openmm/spice-dataset
stars: 198
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: CC-BY-4.0
tags: [qm-datasets, qm-data, biomolecular, organic, drug-like, training-set]
pioneering: false
status: verified
---

## Key innovation
A dataset of **1.1 million conformations** of drug-like molecules, peptides, and amino-acid dimers covering 17 elements at ωB97M-D3(BJ)/def2-TZVPPD, computed with OpenMM-based workflows. SPICE is the **de-facto training set for organic and biomolecular MLPs** — MACE-OFF, AIMNet2, and others train on it directly — because it was purpose-designed for transferable force-field learning: broad conformer and chemical coverage at a consistent, modern DFT level, with partial charges included.

## Limitations / disadvantages
- **Neutral, closed-shell** focus; radicals, charged species, and bond-breaking chemistry under-represented.
- A **single DFT level**; transferability to other theory levels is the model's problem, not the dataset's.
- Conformer diversity bounded by the conformer-generation/sampling scheme; no periodic or condensed-phase data.

## Benchmarks
Primarily a **training set**; downstream models report SPICE test-set energy/force MAE (typically sub-meV–meV energies and low kcal/mol/Å forces for well-trained MACE/OFF models). (Source: Eastman et al., Sci. Data 2022.)

## Sources
- Paper: https://doi.org/10.1038/s41597-022-01882-6
- Preprint: https://arxiv.org/abs/2209.10702
- Data & code: https://github.com/openmm/spice-dataset
