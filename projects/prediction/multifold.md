---
name: MultiFOLD
field: prediction
category: msa-based
year: 2023
venue: "Nucleic Acids Research (2023)"
doi: 10.1093/nar/gkad297
arxiv: null
citations: 66
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/mcguffin/multifold
stars: null
stars_source: null
stars_as_of: 2026-07-04
license: null
tags: [msa-based, multimer, ensemble]
pioneering: false
status: verified
_note: "GitHub repo not found via lookup at capture time; star count unavailable."
---

## Key innovation
An **AlphaFold-Multimer-based ensemble multimer pipeline** from the McGuffin lab (University of
Reading) built around a careful model-ranking and MSA-pairing strategy. It consistently ranked among
the **top protein-complex predictors at both CASP15 and CASP16**, showing that strong engineering and
ensembling around AF-Multimer can rival dedicated multimer methods.

## Limitations / disadvantages
- Compute-intensive ensemble approach rather than a single fast network.
- Ceiling is bounded by the underlying AF-Multimer model quality.
- Strengths are on multimer ranking; less differentiated for single-chain prediction.

## Benchmarks
- Among top-ranked groups for protein complex / multimer prediction at CASP15 and CASP16. (Source:
  McGuffin, Edmunds, Genc et al., Nucleic Acids Research 2023, 10.1093/nar/gkad297.)

## Sources
- Paper: https://doi.org/10.1093/nar/gkad297
- Code: https://github.com/mcguffin/multifold
