---
name: Motif-scaffolding via constrained hallucination
field: design
category: hallucination
year: 2022
venue: "Science 377, 1327–1332 (2022); 'Scaffolding protein functional sites using deep learning'"
doi: 10.1126/science.abn2100
citations: 410
citations_source: semantic-scholar
citations_as_of: 2026-07-04
tags: [hallucination, motif-scaffolding]
pioneering: true
status: verified
---

## Key innovation
Used **constrained AF2/Rosetta hallucination** to design a scaffold that **preserves a functional
motif** (binding/catalytic site) while building a stable supporting structure around it. The first
scalable motif-scaffolding method — it launched functional-site scaffolding before diffusion-based
methods (RFdiffusion) took over.

## Limitations / disadvantages
- **Optimization/search-based** (gradient descent through AF2) — slow and stochastic; needs many
  retries.
- Success and fold accuracy vary by motif.
- Largely superseded by RFdiffusion for motif scaffolding.

## Benchmarks
- Scaffolds for diverse functional motifs (binders, enzymes), experimentally validated.
  (Source: Tischer et al., Science 2022.)

## Sources
- Paper: https://doi.org/10.1126/science.abn2100
