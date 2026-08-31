---
name: SE(3)-Transformer
field: mlip
category: arch-equivariant
year: 2020
venue: "NeurIPS 2020"
doi: null
doi_note: "NeurIPS paper — no journal DOI; see arXiv 2006.10503"
arxiv: 2006.10503
citations: 938
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/FabianFuchsML/se3-transformer-public
stars: 580
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [arch-equivariant, equivariant, attention, transformer, se3]
pioneering: false
status: verified
---

## Key innovation
Made **self-attention SE(3)-equivariant** by attending over degree-l spherical-harmonic tensor features with attention coefficients computed from invariant norms, so the transformer's outputs transform equivariantly under rotations and translations. It showed that attention and equivariance combine cleanly, and became an **influential attention-based equivariant design** feeding into TorchMD-Net and (conceptually) GemNet. It also introduced a notable speedup over earlier higher-rank equivariant nets via degree-wise neighbors.

## Limitations / disadvantages
- Self-attention is **O(N²)** in atoms, limiting large-system use.
- Accuracy on QM9/MD17 is competitive but not field-leading versus dedicated MPNNs.
- Requires careful angular-momenta/cutoff tuning.

## Benchmarks
- **QM9**: competitive property-prediction MAE; strong on the SCAN benchmark used in the paper (point-cloud classification/segmentation) and on QM9.
- Reportedly SOTA among equivariant attention models at release. (Source: Fuchs et al., NeurIPS 2020.)

## Sources
- Preprint: https://arxiv.org/abs/2006.10503
- Code: https://github.com/FabianFuchsML/se3-transformer-public
