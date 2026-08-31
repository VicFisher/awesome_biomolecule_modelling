---
name: ESMFold
field: prediction
category: msa-free-plm
year: 2022
venue: "Science 377, eadc2574 (2023); preprint 2022"
doi: 10.1126/science.ade2574
citations: 4888
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/facebookresearch/esm
stars: "~4.2k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: MIT
tags: [msa-free, plm]
pioneering: true
status: verified
---

## Key innovation
Demonstrated **folding without an MSA**: the **ESM-2** protein language model (trained on
millions of unaligned sequences) produces embeddings that implicitly encode structure and
evolution, fed directly into a folding head. This removes the expensive MSA search, making
ESMFold **~60× faster** than AlphaFold2 and enabling folding at **metagenomic scale** (hundreds
of millions of sequences, e.g. the ESM Metagenomic Atlas).

## Limitations / disadvantages
- Lower accuracy than **AlphaFold2**, especially for proteins with many homologs where an MSA
  would help; the single-sequence signal caps performance on hard targets.
- Outputs a single structure; weaker on large/multidomain proteins.
- pLDDT confidence calibration is slightly worse than AF2's.

## Benchmarks
- Mean TM-score on a held-out test set below AlphaFold2 but far above earlier single-sequence
  baselines; speed ~60× AF2. (Source: Lin et al., Science 2023.)

## Sources
- Paper: https://doi.org/10.1126/science.ade2574
- Code: https://github.com/facebookresearch/esm
- Metagenomic Atlas: https://esmatlas.com
