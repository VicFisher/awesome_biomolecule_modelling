---
name: DimeNet++
field: mlip
category: arch-invariant
year: 2020
venue: "arXiv preprint (2020)"
doi: null
doi_note: "ICML-affiliated preprint; S2 lookup did not resolve a DOI — to backfill"
arxiv: 2011.14115
citations: 427
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/gasteigerjo/dimenet
stars: 357
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-invariant, directional, angular, efficient]
pioneering: false
status: verified
---

## Key innovation
An efficient redesign of DimeNet that **reuses embeddings across interaction blocks** and reorganizes the directional message computation, delivering roughly **8× speedup** and about 10% lower error on QM9 over the original. It also introduced an **uncertainty-aware variant**. This efficient form is the version most practitioners actually ran, and it remained the standard invariant/directional baseline until overtaken by fully equivariant models.

## Limitations / disadvantages
- Inherits DimeNet's triple-based cost (only amortized, not eliminated).
- Invariant output; angular information baked in via fixed bases rather than learned equivariant features.
- Largely displaced by equivariant MPNNs (PaiNN, GemNet, MACE) on accuracy-per-FLOP.

## Benchmarks
- **QM9**: ~10% improvement over DimeNet across most targets at ~8× the throughput. (Source: Klicpera et al., arXiv 2011.14115, 2020.)
- Remained a strong **MD17** baseline through 2021.

## Sources
- Preprint: https://arxiv.org/abs/2011.14115
- Code: https://github.com/gasteigerjo/dimenet
