---
name: MACE-OFF (MACE-OFF23)
field: mlip
category: foundational-universal
year: 2023
venue: "J. Am. Chem. Soc. (2024)"
doi: 10.1021/jacs.4c07099
arxiv: 2312.15211
citations: 227
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/ACEsuit/mace
stars: 1300
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [foundational-universal, foundational, universal, organic, biomolecular, mace]
pioneering: false
status: verified
---

## Key innovation
A family of **short-range transferable organic force fields** (MACE-OFF23) trained on the SPICE dataset at ωB97M-D3(BJ)/def2-TZVPPD, covering ten elements (H, C, N, O, F, P, S, Cl, Br, I). It showed that a **short-range-only MACE can rival classical force fields for biomolecular simulation** while reaching near-DFT accuracy on liquids, crystals, and a solvated protein — positioning MACE-OFF as a drop-in general organic ML force field for drug-like and biomolecular systems.

## Limitations / disadvantages
- **Short-range** by design — no explicit long-range electrostatics or polarization.
- Trained on **neutral closed-shell SPICE** conformers; radical, charged, and excited-state chemistry is less reliable.
- Ten-element coverage; no metals or inorganic chemistry.

## Benchmarks
- Near-DFT accuracy on a solvated protein (chignolin) and a range of liquids/molecular crystals; competitive with general-purpose classical force fields on biomolecular test systems. (Source: Kovacs et al., JACS 2024 / arXiv 2312.15211.)

## Sources
- Paper: https://doi.org/10.1021/jacs.4c07099
- Preprint: https://arxiv.org/abs/2312.15211
- Code: https://github.com/ACEsuit/mace
