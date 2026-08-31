---
name: NuFold
field: prediction
category: rna
year: 2025
venue: "Nature Communications (2025)"
doi: 10.1038/s41467-025-56261-7
arxiv: null
citations: 45
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
stars: null
stars_source: null
stars_as_of: 2026-07-04
license: null
tags: [msa-free-plm, rna, single-sequence]
pioneering: false
status: verified
_note: "RNA-focused; category reflects the single-sequence / single-chain family. Listed under prediction as an RNA tertiary-structure predictor."
---

## Key innovation
An **end-to-end deep-learning predictor of RNA tertiary structure** (Kihara lab, Purdue) that uses a
**flexible-nucleotide (base-pair orientation) representation** rather than treating each nucleotide as a
rigid frame. This lets the model capture nucleobase conformational flexibility directly and predict RNA
3D structure competitively on RNA-Puzzles — an RNA-focused analogue of single-sequence protein folders.

## Limitations / disadvantages
- RNA training data is far smaller than protein data, capping achievable accuracy.
- Struggles with large multi-domain RNAs and complex tertiary contacts / pseudoknots.
- Predicts a single structure; does not model RNA conformational ensembles or dynamics.

## Benchmarks
- Competitive with prior RNA tertiary-structure methods on RNA-Puzzles and CASP RNA targets. (Source:
  Li, Chen, Kihara et al., Nature Communications 2025, 10.1038/s41467-025-56261-7.)

## Sources
- Paper: https://doi.org/10.1038/s41467-025-56261-7
