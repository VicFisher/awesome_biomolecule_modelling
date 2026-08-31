---
name: DeepAb
field: prediction
category: msa-free-plm
year: 2021
venue: "Nature Communications 14, 1862 (2023); preprint 2021"
citations: 188
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/RosettaCommons/DeepAb
stars: 174
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Gray Lab (JHU)
tags: [msa-free, antibody]
status: verified
---

## Key innovation
One of the first **deep-learning antibody Fv structure predictors** (CNN + Rosetta assembly),
pretrained on antibody structures. A precursor to IgFold; demonstrated that antibody-specific DL
beats general methods on CDR loops (notably H3).

## Limitations / disadvantages
- **Antibody-only**; uses CNN + Rosetta assembly (not equivariant/PLM).
- Accuracy below IgFold/AlphaFold2 for full antibodies.
- Single static structure.

## Benchmarks
- Improved H3-loop accuracy over general and earlier antibody methods. (Source: Ruffolo & Gray, Nat
  Commun 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41467-023-35600-3
- Code: https://github.com/RosettaCommons/DeepAb
