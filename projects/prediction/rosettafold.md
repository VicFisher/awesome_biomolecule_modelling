---
name: RoseTTAFold
field: prediction
category: msa-based
year: 2021
venue: "Science 373, 871–876 (2021)"
doi: 10.1126/science.abj8754
citations: 3347
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/RosettaCommons/RoseTTAFold
stars: "~2.2k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: free for non-commercial (Rosetta license)
tags: [msa-based]
pioneering: true
status: verified
---

## Key innovation
A **three-track neural network** that reasons simultaneously over 1D (sequence), 2D
(distance/orientation), and 3D (coordinate) representations, with information flowing between
all three tracks at each layer. This "2D↔3D feedback" was the conceptual alternative to
AlphaFold2's Evoformer and placed a strong second at CASP14. The paper also extended the idea
to **protein-complex prediction** (RoseTTAFold-I) before AlphaFold-Multimer weights were
available.

## Limitations / disadvantages
- Single-chain accuracy **below AlphaFold2**.
- **MSA-dependent**; degrades for shallow alignments.
- Outputs a single structure; complex mode initially limited to dimers.
- Heavier post-processing (Rosetta relaxation) than ESMFold-style fast folders.

## Benchmarks
- **CASP14**: consistently competitive, behind AlphaFold2 (GDT_TS within a few points on most
  targets; ranked among top methods). (Source: Baek et al., Science 2021.)

## Sources
- Paper: https://doi.org/10.1126/science.abj8754
- Code: https://github.com/RosettaCommons/RoseTTAFold
