---
name: FoldFlow-2
field: prediction
category: msa-free-equivariant
year: 2024
venue: "NeurIPS (2024)"
doi: 10.48550/arXiv.2405.20313
arxiv: 2405.20313
citations: 52
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/DreamFold/FoldFlow
stars: 291
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: null
tags: [msa-free-equivariant, flow-matching, generative]
pioneering: false
status: draft
_note: "Same paper as the design entry (design/foldflow-2). Listed here because it is an SE(3)-equivariant sequence-conditioned model, but it is primarily a generative backbone DESIGN method rather than a deterministic structure predictor — hence the primary record lives under design."
---

## Key innovation
A **sequence-conditioned SE(3)-equivariant flow-matching model** (Mila / DreamFold) that generates
protein backbones on the SE(3) manifold, augmented with sequence information so that a sequence prior
conditions the flow. It bridges sequence-conditioned structure generation and flow-based design, and is
the successor to the FoldFlow family of SE(3) stochastic flow-matching backbone models.

## Limitations / disadvantages
- **Generative design framing**, not a deterministic structure predictor for natural sequences; the
  prediction-field listing is borderline.
- Backbone-only; requires ProteinMPNN-style sequence recovery for full design pipelines.
- Single-chain focus; limited all-atom / multimer / ligand handling.

## Benchmarks
- Improved motif-scaffolding and conditional backbone generation over prior FoldFlow / FrameFlow models
  on standard designability benchmarks. (Source: Huguet et al., NeurIPS 2024 / arXiv:2405.20313.)

## Sources
- Paper: https://arxiv.org/abs/2405.20313
- Code: https://github.com/DreamFold/FoldFlow
- See primary record: [projects/design/foldflow-2.md](../design/foldflow-2.md)
