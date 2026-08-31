---
name: ProteinSGM
field: design
category: diffusion-flow
year: 2022
venue: "bioRxiv (2022); 'Score-based generative modeling for de novo protein design'"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: https://github.com/mjslee0921/proteinsgm
repo_note: "repo slug unverified"
tags: [diffusion-flow]
status: draft
institution: "University of Toronto (Lee & Kim)"
---

## Key innovation
**Score-based diffusion on image-based structure representations** (distance/angle maps) — an early
diffusion approach to de novo protein design that also supports **inpainting of functional sites**.

## Limitations / disadvantages
- **Image-based** (distance/angle) representation rather than coordinate-native — less natural for
  all-atom geometry.
- Backbone-centric; older; superseded by SE(3)-equivariant diffusion (FrameDiff/FoldFlow).
- Needs sequence design + validation.

## Benchmarks
- De novo generation and functional-site inpainting vs baselines. (Source: Lee & Kim, bioRxiv 2022.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.1101/2022.07.13.499967v2
- Code: https://github.com/mjslee0921/proteinsgm
