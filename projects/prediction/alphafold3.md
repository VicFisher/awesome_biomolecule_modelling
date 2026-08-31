---
name: AlphaFold3
field: prediction
category: all-atom-cofolding
year: 2024
venue: "Nature 630, 493–500 (2024)"
doi: 10.1038/s41586-024-07487-w
citations: 11843
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/google-deepmind/alphafold3
stars: "~8.3k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
website: https://alphafoldserver.com
license: "restricted (code released 2024; weights/server under terms of use)"
tags: [msa-based, all-atom, cofolding, diffusion]
pioneering: true
status: verified
---

## Key innovation
Extends structure prediction to **joint all-atom complexes** — proteins, nucleic acids,
small-molecule ligands, and ions — in a single model. Replaces the Evoformer with a
**Pairformer** and, crucially, replaces the deterministic structure module with a **generative
diffusion module** over atom positions. This markedly improved accuracy for protein–ligand and
protein–nucleic-acid interactions over AF2/AF-Multimer, and changed the field's paradigm toward
diffusion-based co-folding.

## Limitations / disadvantages
- **Closed weights at launch** — only the AlphaFold Server was available initially (code released
  later under a restrictive license), which triggered open-source reproductions (Boltz, Protenix,
  Chai-1).
- Diffusion module introduces **stereochemistry/clash errors** and **symmetry/hallucination
  artifacts** (e.g. repeated chains, spurious symmetry).
- Ligand-pose accuracy still trails dedicated docking for some cases; **confidence (ipTM/pTM)
  calibration** for complexes is imperfect.
- Static output (no dynamics); certain chemistries (e.g. covalent drugs, modified residues)
  handled poorly at launch.

## Benchmarks
- Improved protein–ligand pose accuracy and protein–nucleic-acid DockQ/iTM over AF-Multimer on
  the PoseBusters and community complex benchmarks; reported gains on the paper's joint
  benchmark set. (Source: Abramson et al., Nature 2024.)

## Sources
- Paper: https://doi.org/10.1038/s41586-024-07487-w
- Code: https://github.com/google-deepmind/alphafold3
- Server: https://alphafoldserver.com
