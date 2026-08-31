---
name: OmegaFold
field: prediction
category: msa-free-plm
year: 2022
venue: "bioRxiv (2022); 'High-resolution de novo structure prediction from primary sequence'"
doi: 10.1101/2022.07.21.500999
citations: 519
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/HeliXonProtein/OmegaFold
stars: 623
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [msa-free, plm]
status: verified
---

## Key innovation
Concurrent with ESMFold, showed that **single-sequence protein language model** embeddings
(OmegaPLM) plus a **geometric transformer** can produce high-resolution structures **without an
MSA**. Demonstrated the PLM-as-implicit-coevolution idea as an alternative MSA-free paradigm.

## Limitations / disadvantages
- Accuracy below AlphaFold2 (and roughly below ESMFold on many benchmarks).
- Single structure; weaker on large/hard targets.
- Less widely adopted than ESMFold; heavier model footprint.

## Benchmarks
- Reported competitive single-sequence folding on CAMEO/CASP targets; behind AF2 but above
  earlier MSA-free baselines. (Source: Wu & Li, bioRxiv 2022.)

## Sources
- Preprint: https://doi.org/10.1101/2022.07.21.500999
- Code: https://github.com/HeliXonProtein/OmegaFold
