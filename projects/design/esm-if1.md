---
name: ESM-IF1
field: design
category: inverse-folding
year: 2022
venue: "ICML 2022; 'Learning inverse folding from millions of predicted structures'"
citations: null
citations_note: "S2 lookup throttled (429) during batch fetch — to backfill"
repo: https://github.com/facebookresearch/esm
stars: "~4.2k"
stars_source: "shields.io (approx) — shared ESM repo"
stars_as_of: 2026-07-04
license: MIT
tags: [inverse-folding, plm]
pioneering: true
status: draft
---

## Key innovation
An inverse-folding model (structure → sequence) trained on **~12M predicted structures** rather
than just experimental PDB, via a GNN structure encoder + autoregressive decoder. Demonstrated that
predicted-structure training **scales** inverse folding, and the resulting model doubles as a
structure-aware representation for **fitness/mutation prediction**.

## Limitations / disadvantages
- **Single-backbone**, sequence-only output; trained on predicted (lossy) structures.
- No all-atom / multistate design in the base model.
- Hugging Face-compatible weights were later restricted; reproducibility changed over time.

## Benchmarks
- Improved sequence recovery over prior inverse folders; strong DMS fitness prediction.
  (Source: Hsu et al., ICML 2022.)

## Sources
- Paper: https://doi.org/10.48550/arXiv.2206.01796
- Code: https://github.com/facebookresearch/esm
