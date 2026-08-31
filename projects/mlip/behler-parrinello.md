---
name: Behler-Parrinello NN potential (HDNNP)
field: mlip
category: arch-invariant
year: 2007
venue: "Physical Review Letters 98, 146401 (2007)"
doi: 10.1103/PhysRevLett.98.146401
arxiv: null
arxiv_note: "No arXiv preprint — published directly in PRL"
citations: 3438
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "No canonical repo — many independent implementations (n2p2, RuNNer, SIMPLE-NN)"
stars: null
stars_note: "No single canonical repo to count"
tags: [arch-invariant, invariant, atomic-descriptors, high-dimensional]
pioneering: true
status: verified
---

## Key innovation
Introduced **high-dimensional neural network potentials (HDNNPs)**: the total energy of a system is decomposed into a sum of per-atom contributions, each computed by a feed-forward NN over local atom-centered symmetry-function descriptors. This **locality decomposition** broke the dimensionality ceiling that had restricted earlier NN potentials to systems of only a few atoms, making DFT-accurate potentials trainable for arbitrary-size condensed systems. Combined with the Behler–Parrinello pair/angular symmetry functions, it set the template — atomic energy decomposition + local invariant descriptors — that nearly every modern MLIP still inherits.

## Limitations / disadvantages
- Strictly **local** within a cutoff: no long-range electrostatics or dispersion unless added by hand.
- Requires **handcrafted descriptor engineering** (symmetry functions) and per-element NN weights rather than end-to-end representation learning.
- Limited **transferability** across chemical environments or new elements without training new networks.
- Accuracy is capped by the quality of the chosen symmetry-function basis.

## Benchmarks
Predates the MD17/QM9 benchmarks. The original PRL and follow-ups demonstrated **DFT-level reproduction** of energies and forces for silicon and sodium systems and enabled molecular-dynamics timescales infeasible with direct DFT. (Source: Behler & Parrinello, PRL 2007; Behler, J. Chem. Phys. 134, 074106, 2011.)

## Sources
- Paper: https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.146401
- Descriptor review: https://doi.org/10.1063/1.3553717
- Community implementation (n2p2): https://github.com/CompPhysVienna/n2p2
