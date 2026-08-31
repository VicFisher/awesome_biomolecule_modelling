---
name: MACE-MP-0
field: mlip
category: foundational-universal
year: 2023
venue: "J. Chem. Phys. (2024)"
doi: 10.1063/5.0297006
arxiv: 2401.00096
citations: 626
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/ACEsuit/mace
stars: 1300
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [foundational-universal, foundational, universal, mace, materials]
pioneering: false
status: verified
---

## Key innovation
A **general-purpose MACE foundation model trained on the Materials Project (MP)** — a single model intended to cover molecules, materials, interfaces, and even proteins out of the box. MACE-MP-0 demonstrated that a pretrained equivariant many-body potential can run **stable MD across diverse chemistries without retraining**, and be **fine-tuned to a target system with a handful of frames**. It established the "foundation model for atomistic chemistry" paradigm at practical scale and became the default starting point for most MACE users.

## Limitations / disadvantages
- Trained on the **Materials Project**, which is mostly inorganic solids and carries the DFT-level quirks/biases of that dataset.
- **Short-range**; long-range interactions only approximate.
- Accuracy on organic/biomolecular systems lags purpose-built models (e.g., MACE-OFF) without fine-tuning.

## Benchmarks
- Stable MD and competitive energies/forces across molecules, liquids, and solids; fine-tuning on a few hundred frames reaches dedicated-model accuracy. (Source: Batatia et al., J. Chem. Phys. 2024 / arXiv 2401.00096.)

## Sources
- Paper: https://doi.org/10.1063/5.0297006
- Preprint: https://arxiv.org/abs/2401.00096
- Code & weights: https://github.com/ACEsuit/mace
