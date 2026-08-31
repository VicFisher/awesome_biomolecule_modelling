---
name: RFdiffusion
field: design
category: diffusion-flow
year: 2022
venue: "Nature 620, 1089–1100 (2023); 'De novo design of protein structure and function with RFdiffusion'"
doi: 10.1038/s41586-023-06415-8
citations: 1219
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/RosettaCommons/RFdiffusion
stars: 2932
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: free for non-commercial (Baker lab license)
tags: [diffusion-flow, binder, motif-scaffolding]
pioneering: true
status: verified
---

## Key innovation
A **diffusion model fine-tuned from RoseTTAFold** that generates protein backbones de novo. A single
framework handles unconditional folding, **motif scaffolding**, **binder design**, symmetric
oligomers, and niche scaffolding — making it the dominant backbone-generation engine in protein
design (typically paired with ProteinMPNN for sequence).

## Limitations / disadvantages
- **Backbone-only** — needs ProteinMPNN/LigandMPNN for sequence; limited all-atom/small-molecule
  handling (RFdiffusionAA extends it).
- Compute-heavy (many denoising steps); success varies by task — binder design usually needs
  affinity-maturation/experimental optimization.
- Generated designs require downstream validation (folding + binding).

## Benchmarks
- High empirical success for de novo binders and motif scaffolds vs prior methods; experimentally
  validated binders and enzymes reported. (Source: Watson et al., Nature 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41586-023-06415-8
- Code: https://github.com/RosettaCommons/RFdiffusion
