---
name: ABodyBuilder3
field: prediction
category: msa-free-plm
year: 2024
venue: "Bioinformatics (2024)"
doi: 10.1093/bioinformatics/btae576
arxiv: 2405.20863
citations: 33
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/oxicarl/ABodyBuilder3
stars: null
stars_source: null
stars_as_of: 2026-07-04
license: null
tags: [msa-free-plm, antibody, language-model]
pioneering: false
status: verified
_note: "GitHub repo not found via lookup at capture time; star count unavailable."
---

## Key innovation
An **improved, scalable antibody Fv structure predictor** in the ABodyBuilder / ImmuneBuilder lineage
(Oxford OxPIG). It integrates an **ESM-style protein language model** with an **IPA structure module**,
improving accuracy and throughput over its predecessors while remaining a lightweight, deployable tool
for large antibody datasets.

## Limitations / disadvantages
- Antibody-only; does not generalize to other protein classes.
- Predicts a single static Fv; does not model CDR loop ensembles or antigen-bound conformations.
- Outpaced on some benchmarks by newer co-design methods, but remains competitive and efficient.

## Benchmarks
- Reports improved CDR-H3 and overall Fv RMSD over ABodyBuilder2 and other baseline antibody predictors.
  (Source: Abanades et al., Bioinformatics 2024, 10.1093/bioinformatics/btae576.)

## Sources
- Paper: https://doi.org/10.1093/bioinformatics/btae576
- Preprint: https://arxiv.org/abs/2405.20863
- Code: https://github.com/oxicarl/ABodyBuilder3
