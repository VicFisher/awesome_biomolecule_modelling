---
name: RhoFold+
field: prediction
category: rna
year: 2024
venue: "Nature Methods (2024)"
doi: 10.1038/s41592-024-02485-3
arxiv: 2207.01586
citations: null
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/ml4bio/RhoFold
stars: 242
stars_source: github-api
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [msa-free-plm, rna, language-model]
pioneering: true
status: draft
_note: "DOI/venue/arxiv taken from discovery source; citation count unavailable in metrics file (paper present in S2 but not aggregated)."
---

## Key innovation
An **RNA-only end-to-end 3D structure predictor** from ByteDance that uses an RNA language model plus a
transformer to fold RNA directly from sequence — effectively the **PLM-folding analogue of ESMFold, but
for RNA**. Published in Nature Methods 2024, it was an early demonstration that single-sequence language
models can predict RNA tertiary structure without deep covariance/MSA signal.

## Limitations / disadvantages
- RNA structure data is far scarcer than protein data, limiting how far language-model scaling can go.
- Accuracy still trails well-characterized protein folders; struggles with large, multi-domain RNAs and
  complex pseudoknots / long-range tertiary contacts.
- Single static prediction; no explicit modeling of RNA conformational ensembles.

## Benchmarks
- Competitive with (and in several cases improving on) prior methods on RNA-Puzzles and CASP15/16 RNA
  targets. (Source: Shen et al., Nature Methods 2024, 10.1038/s41592-024-02485-3.)

## Sources
- Paper: https://doi.org/10.1038/s41592-024-02485-3
- Preprint: https://arxiv.org/abs/2207.01586
- Code: https://github.com/ml4bio/RhoFold
