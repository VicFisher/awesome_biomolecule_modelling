---
name: HelixFold-Single
field: prediction
category: msa-free-plm
year: 2022
venue: "Nature Machine Intelligence 5, 503–514 (2023); preprint 2022"
citations: 88
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/PaddlePaddle/PaddleHelix
stars: 1114
stars_source: "shields.io (approx) — shared PaddleHelix repo"
stars_as_of: 2026-07-04
institution: Baidu
license: Apache-2.0
tags: [msa-free, plm]
status: verified
---

## Key innovation
Baidu's **MSA-free, single-sequence protein folder** (PLM-based), an ESMFold-equivalent built on the
PaddlePaddle stack. Demonstrates the PLM-based single-sequence folding paradigm in a separate
framework; useful where MSAs are unavailable.

## Limitations / disadvantages
- Accuracy below AlphaFold2 (and roughly below ESMFold); single structure.
- **PaddlePaddle** ecosystem limits adoption vs PyTorch-based ESMFold.
- Weaker on large / hard targets.

## Benchmarks
- Competitive single-sequence folding on CAMEO/CASP-style sets; behind AF2. (Source: HelixFold-Single, Nat Mach Intell 2023.)

## Sources
- Paper: https://www.nature.com/articles/s42256-023-00666-y
- Code: https://github.com/PaddlePaddle/PaddleHelix
