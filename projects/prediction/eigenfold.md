---
name: EigenFold
field: prediction
category: msa-free-equivariant
year: 2023
venue: "arXiv (2023)"
doi: 10.48550/arXiv.2304.02198
arxiv: 2304.02198
citations: 113
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/bjing2016/EigenFold
stars: 179
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [msa-free-equivariant, diffusion, generative, ensemble]
pioneering: false
status: verified
_note: "Conditioned on OmegaFold (PLM) embeddings, so it straddles the msa-free-plm / msa-free-equivariant boundary; placed here because the generative core is an equivariant diffusion model over SE(3) eigenmodes."
---

## Key innovation
A **generative diffusion model for protein structure** (MIT CSAIL) that samples a *distribution* of
conformations rather than a single structure. It models the protein as a **harmonic oscillator** by
diffusing along the eigenmodes of a graph Laplacian, letting it produce diverse, physically plausible
ensembles and naturally capture structural uncertainty — an early argument for distributional / ensemble
folding.

## Limitations / disadvantages
- Relies on **OmegaFold (PLM) embeddings** as conditioning, so it is not purely PLM-free despite the
  equivariant generative core.
- Accuracy of individual samples is below AlphaFold2-class point predictors; value lies in diversity,
  not single-structure GDT.
- Eigenmode decomposition scales poorly with chain length and complex topologies.

## Benchmarks
- Demonstrated ensemble diversity and reasonable sample quality on CATH/ProteinMPNN-designability
  benchmarks, with the designability of generated structures validated by ProteinMPNN/ESMFold round-trips.
  (Source: Jing et al., arXiv:2304.02198, 2023.)

## Sources
- Paper: https://arxiv.org/abs/2304.02198
- Code: https://github.com/bjing2016/EigenFold
