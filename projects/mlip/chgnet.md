---
name: CHGNet
field: mlip
category: foundational-universal
year: 2023
venue: "Nature Machine Intelligence (2023); Crystal Hamiltonian Graph Neural Network"
citations: null
citations_note: "S2 lookup throttled — to backfill"
repo: https://github.com/CederGroupHub/chgnet
repo_note: "canonical repo: CederGroupHub/chgnet"
stars: null
stars_note: "shields did not resolve at lookup — to backfill"
tags: [foundational-universal, universal, inorganic, materials]
status: verified
institution: "Ceder Group (UC Berkeley)"
---

## Key innovation
A **universal neural network potential for inorganic materials** based on a **Crystal Hamiltonian
Graph** — pretrained on the large MPtrjectory dataset (Materials Project MD trajectories) to predict
energies, forces, stresses, and **magnetic moments (charges)**. A widely-used foundational MLIP for
materials discovery.

## Limitations / disadvantages
- **Inorganic/materials** focus — not biomolecular.
- Local message-passing; long-range electrostatics limited.
- Accuracy on out-of-distribution chemistries is uneven.

## Benchmarks
- Strong on Materials Project relaxed-structure and MD tasks; widely used as a pretrained baseline.
  (Source: Deng et al., Nat Mach Intell 2023.)

## Sources
- Paper: https://www.nature.com/articles/s42256-023-00716-x
- Code: https://github.com/CederGroupHub/chgnet
