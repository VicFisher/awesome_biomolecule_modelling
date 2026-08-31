---
name: AlphaLink-Multimer (AlphaLink2)
field: prediction
category: msa-based
year: 2024
venue: "Nature Communications (2024)"
doi: 10.1038/s41467-024-51771-2
arxiv: null
citations: 73
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/Rappsilber-Laboratory/AlphaLink2
stars: 68
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: null
tags: [msa-based, multimer, experimental-restraints, crosslinking-ms]
pioneering: false
status: verified
---

## Key innovation
Integrates **crosslinking mass-spectrometry (XL-MS) distance restraints** into AlphaFold-Multimer
(via the Uni-Fold implementation), from the Rappsilber Laboratory (TU Berlin / Edinburgh). This is a
clean demonstration that **experimental restraints can be folded into a learned multimer predictor** to
resolve ambiguous heteromeric topologies, outperforming unrestrained AF-Multimer on difficult
crosslink-rich targets.

## Limitations / disadvantages
- Requires XL-MS data, which is not always available and adds an experimental burden.
- Improvements concentrate on restraint-informable cases; little gain when crosslinks are sparse.
- Built on AF-Multimer, so inherits its MSA-pairing and complex-confidence limitations.

## Benchmarks
- Outperformed AF-Multimer on hard heteromeric CASP15 targets when crosslink restraints were provided.
  (Source: Yu et al., Nature Communications 2024, 10.1038/s41467-024-51771-2.)

## Sources
- Paper: https://doi.org/10.1038/s41467-024-51771-2
- Code: https://github.com/Rappsilber-Laboratory/AlphaLink2
