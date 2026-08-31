---
name: BALMFold
field: prediction
category: msa-free-plm
year: 2024
venue: "Nature Communications (2024)"
doi: 10.1038/s41467-024-46444-5
arxiv: null
citations: null
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
stars: null
stars_source: null
stars_as_of: 2026-07-04
license: null
tags: [msa-free-plm, antibody, language-model]
pioneering: false
status: draft
_note: "DOI/year/venue taken from discovery source; citation and star counts unavailable in metrics file."
---

## Key innovation
An **antibody-specific, MSA-free structure predictor** built on **BALM** (Bio-inspired Antibody Language
Model). BALM stacks a deep (~30-layer) transformer with a custom **BAformer** attention module and a
structure head, learning antibody structure directly from antibody sequences without MSAs — an
IgFold-class approach specialized to the immunoglobulin fold.

## Limitations / disadvantages
- **Antibody-only**: generalizes poorly outside Fv/scFv contexts.
- MSA-free, so it cannot exploit paratope-specific coevolutionary signal when deep homologs exist.
- Closed/inaccessible code and weights limit independent benchmarking.

## Benchmarks
- Reports antibody structure accuracy competitive with IgFold and other MSA-free antibody predictors on
  standard antibody benchmark sets. (Source: Bao et al., Nature Communications 2024,
  10.1038/s41467-024-46444-5.)

## Sources
- Paper: https://doi.org/10.1038/s41467-024-46444-5
