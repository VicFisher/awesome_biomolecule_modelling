---
name: PhysNet
field: mlip
category: arch-invariant
year: 2019
venue: "Journal of Chemical Theory and Computation 15, 3678 (2019)"
doi: 10.1021/acs.jctc.9b00181
arxiv: 1902.08408
citations: 1049
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/MMunke/PhysNet
stars: null
stars_note: "Repo exists but shields.io count did not resolve — to backfill"
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
tags: [arch-invariant, invariant, electrostatics, long-range, message-passing]
pioneering: false
status: verified
---

## Key innovation
An invariant message-passing net that adds **explicit physics terms** — learned per-atom partial charges giving rise to electrostatic energies and predicted dipole moments — on top of a local energy head, yielding a physically consistent, long-range-aware potential. It achieved **state-of-the-art accuracy on QM9, MD17, and ISO17** at release and notably demonstrated transferability from dipeptide fragments to a deca-alanine helix never seen in training — an early demonstration that NNPs could generalize across molecular size.

## Limitations / disadvantages
- Local descriptor backbone remains **invariant** (distance-based); directional information only implicit.
- The partial-charge electrostatics model is a simplification of true polarization/response.
- Transferability, while encouraging, still degrades far from the training distribution.

## Benchmarks
- **QM9 / MD17 / ISO17**: SOTA or near-SOTA at release; ISO17 generalization to unseen conformations of deca-alanine within chemical accuracy. (Source: Unke & Meuwly, JCTC 2019.)
- Predicted dipole moments and partial charges validated against ab-initio reference.

## Sources
- Paper: https://doi.org/10.1021/acs.jctc.9b00181
- Preprint: https://arxiv.org/abs/1902.08408
- Code: https://github.com/MMunke/PhysNet
