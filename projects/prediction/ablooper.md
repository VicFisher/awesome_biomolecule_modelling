---
name: ABlooper
field: prediction
category: msa-free-equivariant
year: 2021
venue: "Bioinformatics 38, 1875–1877 (2022)"
citations: 94
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/oxpig/Ablooper
stars: 52
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Oxford (Deane lab / OPIG)
tags: [msa-free, equivariant-framework, antibody]
status: verified
---

## Key innovation
A fast **equivariant graph neural network** that predicts antibody **CDR loop structures** directly
— an early, clean example of an **MSA-free, PLM-free, SE(3)-equivariant** coordinate predictor
(hence its place in the `msa-free-equivariant` bucket), specialized to antibody loops.

## Limitations / disadvantages
- **Antibody-CDR-only** (not a full protein folder).
- Superseded for full-antibody structure by IgFold/AlphaFold2.
- Depends on a provided antibody framework.

## Benchmarks
- Fast, accurate CDR-loop prediction (notably H3) vs Rosetta/Antibody-Packer. (Source: Abanades et
  al., Bioinformatics 2022.)

## Sources
- Paper: https://doi.org/10.1093/bioinformatics/btac016
- Code: https://github.com/oxpig/Ablooper
