---
name: DiffAb
field: design
category: specialized
year: 2022
venue: "ICLR 2022; 'Antigen-specific antibody design and optimization with DiffAb'"
citations: 302
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/luost26/diffab
stars: 366
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [antibody, diffusion-flow]
pioneering: true
status: verified
---

## Key innovation
An **equivariant diffusion model for antibody CDR design** conditioned on the antigen structure —
a pioneer of structure-conditioned antibody design. Generates diverse CDR loops (orientation +
sequence) and ranks them for antigen binding.

## Limitations / disadvantages
- **Antibody-only**; focuses on CDR-H3 and a few loops.
- Generated binders usually need affinity maturation/experimental optimization.
- Conditioned on a fixed antigen pose.

## Benchmarks
- Improved CDR design over Rosetta/Antibody-design baselines on antigen-bound structures.
  (Source: Luo et al., ICLR 2022.)

## Sources
- Paper: https://doi.org/10.48550/arXiv.2110.09250
- Code: https://github.com/luost26/diffab
