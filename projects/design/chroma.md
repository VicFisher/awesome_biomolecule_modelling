---
name: Chroma
field: design
category: diffusion-flow
year: 2022
venue: "Nature 619, 660–668 (2023); 'Illuminating protein space with a programmable generative model'"
doi: 10.1038/s41586-023-06728-8
citations: 592
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/generatebio/chroma
stars: 822
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: non-commercial research (Generate Biomedicines)
tags: [diffusion-flow]
pioneering: true
status: verified
---

## Key innovation
A **programmable** generative model for protein backbones that diffuses in a low-dimensional
representation, enabling conditioning on **symmetry, shape, size, and properties**. It scales to
thousand-residue proteins and samples diverse, designable structures — the other major backbone
diffusion landmark alongside RFdiffusion, with a stronger emphasis on controllability.

## Limitations / disadvantages
- **Backbone-only**; needs a separate sequence-design step.
- **Conditioning can be finicky**; experimental validation breadth smaller than the RFdiffusion
    ecosystem.
- Commercial origin (Generate Biomedicines) — license is non-commercial.

## Benchmarks
- Demonstrated controllable generation (symmetry/shape) with high designability (AF2/MPNN
  round-trip). (Source: Ingraham et al., Nature 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41586-023-06428-3
- Code: https://github.com/generatebio/chroma
