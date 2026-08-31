---
name: Symmetric-assembly hallucination
field: design
category: hallucination
year: 2022
venue: "Science / Nature family (2022); 'Hallucinating symmetric protein assemblies'"
citations: 218
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/bwicky/oligomer_hallucination
stars: 38
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Wicky, Stiff-Roberts, Bera, Baker (UW)
tags: [hallucination, binder]
pioneering: true
status: draft
---

## Key innovation
Extended **AF2 hallucination to symmetric design** — constraining the generation to Cn / dihedral /
icosahedral symmetry to create de novo **symmetric oligomeric assemblies** (rings, cages, cyclic
assemblies). A pioneer of generative symmetric assembly design.

## Limitations / disadvantages
- **Optimization/search-based** (gradient descent through AF2) — slow and stochastic.
- Limited to the symmetry types implemented; success varies.
- Largely superseded by RFdiffusion's symmetric design mode.

## Benchmarks
- Designed and structurally validated symmetric assemblies (cages/rings). (Source: Wicky et al.,
  2022.)

## Sources
- Code: https://github.com/bwicky/oligomer_hallucination
