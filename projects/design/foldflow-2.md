---
name: FoldFlow-2
field: design
category: diffusion-flow
year: 2024
venue: "NeurIPS 2024; 'Sequence-Augmented SE(3)-Flow Matching for Conditional Protein Backbone Generation'"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: null
tags: [diffusion-flow, flow-matching]
status: draft
institution: "Mila / HEC Montréal / DreamFold (Huguet, Vuckovic, et al.)"
---

## Key innovation
**Sequence-conditioned SE(3) flow matching** for conditional protein backbone generation — bridging
sequence priors with flow-based structure generation, enabling controllable backbone design from a
sequence input.

## Limitations / disadvantages
- **Backbone-only**; conditional generation requires a sequence prompt.
- Newer; smaller validation base than RFdiffusion.
- Needs sequence design + folding validation.

## Benchmarks
- Conditional backbone generation with improved control vs unconditional flow matching. (Source:
  FoldFlow-2, NeurIPS 2024.)

## Sources
- Paper: https://neurips.cc/virtual/2024/poster/93544
