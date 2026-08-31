---
name: FoldFlow
field: design
category: diffusion-flow
year: 2023
venue: "ICLR 2024; 'FoldFlow: Simplifying and Improving Flow Matching for Protein Backbones'"
citations: 178
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/DreamFold/FoldFlow
stars: 291
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [diffusion-flow, flow-matching]
status: verified
---

## Key innovation
Replaces discrete diffusion with **SE(3) flow matching / continuous normalizing flows** over
backbone frames, giving a simpler-to-train, more sample-efficient generative process than FrameDiff.
FoldFlow-2 adds stability (Riemannian/OT variants) and improves designability.

## Limitations / disadvantages
- **Backbone-only**; newer ecosystem than RFdiffusion.
- Needs sequence design + validation; success varies by target.

## Benchmarks
- Improved designability over FrameDiff; efficient sampling (fewer steps). (Source: Bose et al.,
  ICLR 2024.)

## Sources
- Paper: https://doi.org/10.48550/arXiv.2306.17782
- Code: https://github.com/DreamFold/FoldFlow
