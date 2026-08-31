---
name: IgFold
field: prediction
category: msa-free-plm
year: 2022
venue: "Nature Communications 14, 2389 (2023); preprint 2022"
doi: 10.1038/s41467-023-38063-x
citations: 335
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/Graylab/IgFold
stars: 422
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
tags: [msa-free, plm, antibody]
status: verified
---

## Key innovation
**Antibody-specific** structure prediction: the **AntiBERTy** language model (pretrained on
**558M natural antibody sequences**) feeds a graph network that directly predicts backbone
coordinates. Enables fast, high-throughput antibody Fv structure prediction — useful for
therapeutic antibody pipelines at a fraction of AF2's cost.

## Limitations / disadvantages
- **Antibody-only**; predicts the Fv, not full Ig / antigen context.
- Accuracy below AlphaFold2 for full antibodies, especially **VH–VL relative orientation** and
  some CDR loops (H3).
- Static single structure; no paratope/epitope reasoning.

## Benchmarks
- Comparable or faster than AF2 on antibody Fv benchmarks while orders of magnitude quicker;
  H3-loop accuracy remained the hardest region. (Source: Ruffolo et al., Nat Commun 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41467-023-38063-x
- Code: https://github.com/Graylab/IgFold
