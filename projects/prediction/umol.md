---
name: UMol
field: prediction
category: all-atom-cofolding
year: 2023
venue: "Nature Communications 15, 5560 (2024); 'Prediction of protein-ligand complex structures'"
citations: 71
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/patrickbryant1/Umol
stars: 240
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Bryant, Clementi, Noé
tags: [msa-based, all-atom, cofolding]
status: verified
---

## Key innovation
Predicts **protein–small-molecule-ligand complex structures from sequence coevolution** — extending
Potts-model / DCA coevolution to infer protein–ligand contacts and fold the holo complex. An
early protein–ligand co-folding approach distinct from the AF3 diffusion paradigm.

## Limitations / disadvantages
- Only works where a **coevolutionary signal** for ligand contacts exists (limited applicability).
- Pose/interaction accuracy below AlphaFold3-class models.
- Small-scale; limited adoption.

## Benchmarks
- Recovered known protein–ligand interactions on benchmark sets. (Source: Bryant et al., Nat Commun
  2024.)

## Sources
- Paper: https://doi.org/10.1038/s41467-024-48837-6
- Code: https://github.com/patrickbryant1/Umol
