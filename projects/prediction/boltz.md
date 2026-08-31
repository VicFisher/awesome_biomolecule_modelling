---
name: Boltz-1
field: prediction
category: all-atom-cofolding
year: 2024
venue: "bioRxiv / arXiv 2411.03866 (2024)"
arxiv: 2411.03866
citations: 405
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/jwohlwend/boltz
stars: "~4.1k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT
tags: [msa-based, all-atom, cofolding, diffusion]
status: verified
---

## Key innovation
An **open-source reproduction and extension of AlphaFold3**'s diffusion-based all-atom
co-folding, released with **freely available weights**. It matches AF3-level accuracy on
complex benchmarks while removing the AlphaFold-Server access/usage restrictions, and became
the most-adopted community AF3-class model.

## Limitations / disadvantages
- A **reproduction** (architecture follows AF3); inherits AF3's diffusion artifacts
  (stereochemistry/clashes, symmetry hallucination).
- Compute-heavy; confidence calibration for complexes is imperfect.
- Newer than AF3, so less independently validated at scale.

## Benchmarks
- Reported AF3-comparable performance on the PoseBusters / complex benchmarks defined in the
  paper. (Source: Wohlwend et al., arXiv 2411.03866.)

## Sources
- Preprint: https://arxiv.org/abs/2411.03866
- Code: https://github.com/jwohlwend/boltz
