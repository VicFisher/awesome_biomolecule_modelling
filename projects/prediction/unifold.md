---
name: Uni-Fold
field: prediction
category: msa-based
year: 2021
venue: "Software release — no primary paper"
repo: https://github.com/dptech-corp/Uni-Fold
stars: 420
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [msa-based]
status: verified
---

## Key innovation
An **open-source reimplementation of AlphaFold2** with a complete, trainable pipeline (including
**Uni-Fold-Multimer** and later all-atom variants). It gave the community the ability to
retrain and redeploy AF2-class models freely, and added engineering improvements (e.g. better
MSA handling and memory efficiency). Released by DP Technology.

## Limitations / disadvantages
- **Not a new method** — follows AF2; accuracy ~AF2, no algorithmic leap.
- **No peer-reviewed paper** (documentation/community smaller than official AF2/ColabFold).
- Largely superseded for new work by AF3-class co-folding models.

## Benchmarks
- Reproduces AF2-level single-chain and multimer accuracy (per repo documentation); no formal
  benchmark paper.

## Sources
- Code: https://github.com/dptech-corp/Uni-Fold
