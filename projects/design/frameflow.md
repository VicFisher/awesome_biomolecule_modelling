---
name: FrameFlow
field: design
category: diffusion-flow
year: 2023
venue: "MLSB @ ICML 2023; 'Fast protein backbone generation with SE(3) flow matching'"
citations: null
citations_note: "Workshop paper — S2 lookup did not resolve — to backfill"
repo: null
tags: [diffusion-flow, flow-matching]
status: draft
institution: "University of Oxford / Valence Labs (Yim et al.)"
---

## Key innovation
Adapted **FrameDiff to stochastic SE(3) flow matching** for markedly faster protein backbone
generation — the **first flow-matching backbone model**, establishing flow matching as an
alternative to diffusion for structure generation.

## Limitations / disadvantages
- **Backbone-only**; workshop paper (limited formal validation).
- Needs sequence design + folding validation.
- Superseded by FoldFlow / FoldFlow-2 in subsequent work.

## Benchmarks
- Faster backbone generation than FrameDiff at comparable designability. (Source: FrameFlow, MLSB
  2023.)

## Sources
- Paper: https://www.mlsb.io/papers_2023/Fast_protein_backbone_generation_with_SE3_flow_matching.pdf
