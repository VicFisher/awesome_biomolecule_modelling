---
name: EVCouplings
field: prediction
category: pre-dl-contact
year: 2019
venue: "Bioinformatics 35(9), 1582–1584 (2019)"
doi: 10.1093/bioinformatics/bty885
citations: 275
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/debbiemarkslab/EVCouplings
stars: 309
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
website: https://evcouplings.org
tags: [pre-dl-contact]
pioneering: true
status: verified
---

## Key innovation
The canonical open-source **coevolution framework**: generate MSAs, run **direct-coupling
analysis (DCA)** to extract evolutionary couplings (ECs), and use them to predict residue
contacts/structure, mutation effects, and interactions. It is the mature, packaged expression
of the coevolution→structure idea (Morcos/Marks 2011 lineage) that motivated all later
contact- and distance-based predictors.

## Limitations / disadvantages
- **Contact-only** output (sparse restraints), far below modern end-to-end folders in
  structure accuracy.
- Requires **deep, diverse MSAs**; fails or degrades for small / under-sampled families.
- DCA inference scales ~quadratically with sequence length / MSA depth.

## Benchmarks
- Contact-prediction precision on standard CASP/CAMEO contact benchmarks; used widely for
  mutation-effect and structure-restraint pipelines. (Source: Hopf et al., Bioinformatics 2019.)

## Sources
- Paper: https://doi.org/10.1093/bioinformatics/bty885
- Code: https://github.com/debbiemarkslab/EVCouplings
- Server: https://evcouplings.org
