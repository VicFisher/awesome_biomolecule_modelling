---
name: AIMNet2
field: mlip
category: foundational-universal
year: 2025
venue: "Chemical Science (2025)"
doi: 10.1039/d4sc08572h
arxiv: null
arxiv_note: "No arXiv preprint; chemRxiv 10.26434/chemrxiv-2023-296ch, published Chem. Sci. 2025"
citations: 112
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/aiqm/aimnet2
stars: null
stars_note: "shields.io count did not resolve at lookup time — to backfill"
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [foundational-universal, foundational, universal, organic, biomolecular, atoms-in-molecules]
pioneering: false
status: verified
---

## Key innovation
A second-generation **atoms-in-molecules neural network potential** covering 14 elements and neutral, charged, and radical organic / element-organic species. AIMNet2 predicts **energies, forces, partial charges, dipoles, stress tensors, and Hessians** at DFT quality across both molecules and periodic systems, generalizing AIMNet's charge-equilibration-informed design to a broad, transferable foundation model for organic and biomolecular chemistry. It is a direct successor to the ANI line from the same group.

## Limitations / disadvantages
- **Organic / elemental-organic focus**; not intended for metals or extended inorganic systems.
- Short-range (atoms-in-molecules locality); long-range handled approximately via learned charges.
- Single DFT reference level (ωB97M-D3 / def2-TZVPPD family); transfer to other levels requires care.

## Benchmarks
- DFT-quality energies, forces, and dipoles across neutral/charged/radical test sets; Hessian predictions near DFT reference. (Source: Anstine, Zubatyuk, Isayev, Chem. Sci. 2025.)

## Sources
- Paper: https://doi.org/10.1039/d4sc08572h
- chemRxiv preprint: https://doi.org/10.26434/chemrxiv-2023-296ch
- Code: https://github.com/aiqm/aimnet2
