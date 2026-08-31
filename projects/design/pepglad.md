---
name: PepGLAD
field: design
category: specialized
year: 2024
venue: "NeurIPS 2024; 'Full-Atom Peptide Design with Geometric Latent Diffusion'"
arxiv: 2402.13555
repo: https://github.com/THUNLP-MT/PepGLAD
stars: 127
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
citations: 37
citations_source: semantic-scholar
citations_as_of: 2026-07-06
tags: [peptide, diffusion-flow]
status: verified
institution: "Tsinghua University (Kong, Jia et al.)"
---

## Key innovation
**Full-atom peptide design** conditioned on a binding site via **geometric latent diffusion**: an
autoencoder learns a latent structure representation, then a latent diffusion model generates
peptide structures (also modeling latent distances between consecutive residues).

## Limitations / disadvantages
- **Peptide-only**; binding-site-conditioned (needs a pocket).
- Sequence/structure co-design at peptide scale; not full-protein.
- Newer; limited experimental validation.

## Benchmarks
- Full-atom peptide generation quality vs baselines. (Source: PepGLAD, NeurIPS 2024.)

## Sources
- Paper: https://arxiv.org/abs/2402.13555
- Code: https://github.com/THUNLP-MT/PepGLAD
