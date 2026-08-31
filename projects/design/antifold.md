---
name: AntiFold
field: design
category: specialized
year: 2024
venue: "arXiv 2405.03370 (2024); Bioinformatics Advances"
arxiv: 2405.03370
repo: https://github.com/oxpig/AntiFold
stars: 168
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
citations: 29
citations_source: semantic-scholar
citations_as_of: 2026-07-04
license: MIT
tags: [antibody, inverse-folding, plm]
status: verified
institution: "University of Oxford (OxPIG)"
---

## Key innovation
An **antibody-specific inverse-folding model fine-tuned from ESM-IF1** on both solved and predicted
antibody structures. Reports improved CDR sequence design over AbMPNN/IgMPNN, making it a strong
lightweight choice for antibody sequence design.

## Limitations / disadvantages
- **Antibody-only**; depends on the ESM-IF1 base.
- Sequence-only output; no simultaneous structure redesign.
- Newer; smaller community than ProteinMPNN-family.

## Benchmarks
- Outperforms AbMPNN/IgMPNN on antibody CDR design benchmarks. (Source: AntiFold, arXiv 2405.03370.)

## Sources
- Paper: https://arxiv.org/abs/2405.03370
- Code: https://github.com/oxpig/AntiFold
