---
name: OpenFold3
field: prediction
category: all-atom-cofolding
year: 2025
venue: ""
doi: null
arxiv: null
repo: https://github.com/aqlaboratory/openfold-3
stars: 776
stars_source: github-api
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [all-atom-cofolding, cofolding, open-source]
pioneering: false
status: draft
_note: "No formal paper / preprint released at time of writing (preview reproduction); citation count unavailable."
---

## Key innovation
A **fully open-source reproduction of AlphaFold3** led by the OpenFold Consortium (AlQuraishi Lab, Columbia).
It extends co-folding to protein–protein, protein–DNA/RNA and protein–ligand complexes with permissive
licensing and is distributed via NVIDIA NIM, aiming to give the community a transparent, trainable
AlphaFold3-equivalent where DeepMind's release was server-only / restrictively licensed. As a bitwise
reproduction rather than a new method, its scientific contribution is openness and reproducibility rather
than a novel architecture.

## Limitations / disadvantages
- **Preview / no accompanying paper** — model and training details are not yet formally published, so
  independent evaluation is limited to the released weights/code.
- Follows AlphaFold3's design, so inherits the same diffusion-module artifacts (stereochemistry/clash
  errors, symmetry hallucination) and imperfect complex-confidence calibration.
- Reproduction parity, not accuracy leadership: positioned as an open baseline rather than a SOTA push.

## Benchmarks
- Reported to match AlphaFold3 on the complex-prediction tasks covered by its preview; no independent
  benchmark numbers available at time of writing. (Source: OpenFold3 preview release.)

## Sources
- Code: https://github.com/aqlaboratory/openfold-3
- Portal: https://portal.openfold.omsf.io
