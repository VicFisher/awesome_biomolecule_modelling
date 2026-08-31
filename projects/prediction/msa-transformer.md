---
name: MSA Transformer
field: prediction
category: msa-based
year: 2021
venue: "ICML 2021; bioRxiv (2021)"
citations: 724
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/facebookresearch/esm
stars: "~4.2k"
stars_source: "shields.io (approx) — shared ESM repo"
stars_as_of: 2026-07-04
institution: Meta (FAIR)
tags: [msa-based]
pioneering: true
status: verified
---

## Key innovation
A **Transformer over multiple sequence alignments** (interleaved row/column attention) that produces
rich **MSA-aware representations** for contact prediction, structure, and downstream fitness
prediction. Highly influential as a learned MSA representation, even though it was not an end-to-end
folder.

## Limitations / disadvantages
- **Representation-focused** — not an end-to-end structure predictor.
- Depends on a deep MSA.
- As a folder/contact predictor, superseded by AlphaFold2; its main legacy is in representation
  learning.

## Benchmarks
- Strong contact-prediction and fitness-prediction performance; widely used as a frozen feature
  extractor. (Source: Rao et al., ICML 2021.)

## Sources
- Paper: https://doi.org/10.48550/arXiv.2101.08743
- Code: https://github.com/facebookresearch/esm
