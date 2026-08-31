---
name: tFold
field: prediction
category: msa-based
year: 2022
venue: "bioRxiv (2022)"
doi: 10.1101/2022.11.10.515918
arxiv: null
citations: 22
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/TencentAI4S/tfold
stars: 160
stars_source: github-api
stars_as_of: 2026-07-04
license: null
tags: [msa-based, contact-prediction, antibody]
pioneering: false
status: verified
_note: "Primary paper (doi above) is the tFold-Ab antibody variant; the tFold family spans contact-assisted de novo folding plus antibody/antigen/TCR specializations."
---

## Key innovation
A **contact-assisted de novo protein folding family** from Tencent AI Lab (AI4S) that was strong at
CASP14. Beyond the core folder, Tencent released specialized variants — **tFold-Ab** (antibody
structure), **tFold-Ag** (antibody–antigen complexes) and **tFold-TCR** (T-cell receptor–pMHC) — making
it one of the earlier industrial fold suites to target immune-receptor modelling specifically.

## Limitations / disadvantages
- MSA/contact dependent; weaker for orphan sequences and novel immune loops.
- Antibody-specialized variants were largely outpaced by later PLM-based predictors (IgFold,
  ABodyBuilder3) and dedicated co-design methods.
- Documentation and reproducibility of the full special-purpose variants is limited.

## Benchmarks
- Competitive contact-prediction and de novo folding accuracy at CASP14; tFold-Ab reported strong
  antibody Fv prediction without sequence homologs. (Source: Wu et al., bioRxiv 2022,
  10.1101/2022.11.10.515918.)

## Sources
- Paper: https://doi.org/10.1101/2022.11.10.515918
- Code: https://github.com/TencentAI4S/tfold
