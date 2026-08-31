---
name: RoseTTAFold2 (RF2)
field: prediction
category: msa-based
year: 2023
venue: "bioRxiv (2023)"
doi: 10.1101/2023.05.24.542179
arxiv: null
citations: 129
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/uw-ipd/RoseTTAFold2
stars: 212
stars_source: github-api
stars_as_of: 2026-07-04
license: MIT
tags: [msa-based, three-track, evoformer]
pioneering: false
status: verified
---

## Key innovation
An **upgraded three-track (1D/2D/3D) successor to RoseTTAFold** from the Baker/DiMaio labs. It is more
efficient and more accurate than the original RoseTTAFold and broadly competitive with AlphaFold2, while
serving as the **backbone network that RFdiffusion, RF2NA and RoseTTAFold All-Atom are built on** — making
it one of the most consequential "second-generation" MSA-based folders in the open ecosystem.

## Limitations / disadvantages
- Still **MSA-dependent**: accuracy degrades on orphan / low-MSA sequences.
- Single static structure output; does not model conformational ensembles or dynamics.
- Superseded for all-atom / cofolding tasks by its own descendants (RF2NA, RFAA) and by AF3-class models.

## Benchmarks
- Reported accuracy on par with or better than AlphaFold2 on standard CASP/CAMEO protein targets at
  lower inference cost. (Source: Baek et al., bioRxiv 2023, 10.1101/2023.05.24.542179.)

## Sources
- Paper: https://doi.org/10.1101/2023.05.24.542179
- Code: https://github.com/uw-ipd/RoseTTAFold2
