---
name: FrameDiff (SE(3) diffusion)
field: design
category: diffusion-flow
year: 2023
venue: "ICML 2023; 'SE(3) diffusion model with application to protein backbone generation'"
citations: 333
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/jasonkyuyim/se3_diffusion
stars: 423
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [diffusion-flow, flow-matching]
pioneering: true
status: verified
---

## Key innovation
The first **SE(3)-equivariant diffusion model over backbone rigid-body frames** (residue rotations
+ translations), giving a theoretically grounded generative process for protein backbones. It
established the equivariant-backbone-diffusion foundation that FoldFlow, FrameFlow, and others
built on.

## Limitations / disadvantages
- **Backbone-only**; lower empirical designability than RFdiffusion.
- Needs a separate sequence-design step (ProteinMPNN) and folding validation.
- Many sampling steps.

## Benchmarks
- Designability, cluster-coverage, and novelty metrics established for backbone diffusion
  benchmarks. (Source: Yim et al., ICML 2023.)

## Sources
- Paper: https://doi.org/10.48550/arXiv.2301.12485
- Code: https://github.com/jasonkyuyim/se3_diffusion
