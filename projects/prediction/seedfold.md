---
name: SeedFold
field: prediction
category: all-atom-cofolding
year: 2025
venue: "arXiv 2512.24354 (2025)"
arxiv: 2512.24354
citations: 5
citations_source: semantic-scholar
citations_as_of: 2026-07-04
institution: ByteDance
repo: null
repo_note: "no public repo yet"
tags: [msa-based, all-atom, cofolding]
status: draft
---

## Key innovation
A **width-scaled Pairformer** (scaling the AlphaFold3 trunk wider) for all-atom complex
prediction; the preprint claims to **beat AlphaFold3 on the FoldBench** benchmark. Represents the
"scale-the-trunk" hypothesis for improving AF3-class models.

## Limitations / disadvantages
- Very new preprint with **no public code/weights** yet — not independently reproducible.
- Low citation/validation so far; claims await community confirmation.
- Compute requirements for the width-scaled trunk are large.

## Benchmarks
- Reports state-of-the-art on FoldBench (per preprint); needs independent reproduction.
  (Source: SeedFold, arXiv 2512.24354.)

## Sources
- Preprint: https://arxiv.org/abs/2512.24354
