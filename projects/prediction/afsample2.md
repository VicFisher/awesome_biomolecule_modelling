---
name: AFsample2
field: prediction
category: msa-based
year: 2025
venue: "Communications Biology (2025)"
citations: 83
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/wallnerlab/AFsample2
stars: 60
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Wallner (Linköping)
tags: [msa-based, conformational-ensemble]
status: verified
---

## Key innovation
Improved **AlphaFold2 sampling** — explores diverse "folding pathways" via alternative MSA
trimming, crop sampling, and cluster-based selection to find higher-accuracy / alternative
conformations. A top-ranked method at **CASP16**, showing that better sampling of AF2 itself
yields large gains without architectural changes.

## Limitations / disadvantages
- **Expensive** — runs AF2 many times (large compute overhead).
- Stochastic; selection heuristics matter.
- Still single-model-family (AF2), not a new architecture.

## Benchmarks
- Top performance at CASP16; gains over stock AF2 on hard/conformational targets. (Source: Wallner,
  Commun Biol 2025.)

## Sources
- Paper: https://www.nature.com/articles/s42003-025-07753-y
- Code: https://github.com/wallnerlab/AFsample2
