---
name: DTNN (Deep Tensor Neural Network)
field: mlip
category: arch-invariant
year: 2016
venue: "Nature Communications 7, 13890 (2016)"
doi: 10.1038/ncomms13890
arxiv: 1609.08259
citations: 1409
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "No official standalone repo; conceptual basis later released via SchNetPack"
stars: null
stars_note: "No canonical repo to count"
tags: [arch-invariant, invariant, message-passing, end-to-end]
pioneering: false
status: verified
---

## Key innovation
The first **end-to-end deep tensor neural network** for molecular energies: atom embeddings are updated through interaction blocks that combine pairwise distances via tensor operations, producing a size-extensive total energy as a sum of atomic contributions. It removed the need for handcrafted descriptors (Behler–Parrinello / ANI style), **learning the representation directly from interatomic distances**. Reaching roughly 1 kcal/mol atomization-energy error on organic molecules, it is the **direct conceptual precursor to SchNet** and established the distance-based message-passing paradigm for MLIPs.

## Limitations / disadvantages
- **Rotationally invariant but angularly implicit** — uses only distances, so bond-angle information is captured only indirectly (SchNet, and especially DimeNet, later showed explicit angles help substantially).
- Trained on **energies only** in the original; forces obtained via numerical differentiation.
- Demonstrated only on small reference molecules; no condensed-phase or biomolecular evaluation.

## Benchmarks
On **QM9**, atomization-energy MAE in the ~1 kcal/mol-class range across targets, competitive with or better than descriptor- and kernel-based methods of the era. (Source: Schütt et al., Nature Commun. 2017, Table 1.)

## Sources
- Paper: https://doi.org/10.1038/ncomms13890
- Preprint: https://arxiv.org/abs/1609.08259
