---
name: BindCraft
field: design
category: all-atom-binder-motif
year: 2025
venue: "Nature (2025); 'One-shot design of functional protein binders with BindCraft'"
doi: 10.1038/s41586-025-09429-6
repo: https://github.com/martinpacesa/BindCraft
stars: "~1.2k"
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
citations: 190
citations_source: semantic-scholar
citations_as_of: 2026-07-06
license: open-source (MIT-style)
tags: [binder, flow-matching]
pioneering: true
status: verified
institution: "Martin Pacesa / Correia Lab (EPFL)"
---

## Key innovation
An **open-source, automated pipeline for de novo protein binder design** that runs an
**AlphaFold-Multimer-guided design loop** with ProteinMPNN and RFdiffusion-style components,
filtering in the loop. Produces **"one-shot" functional binders** with high experimental success
(**10–100%**, target-dependent) — currently the most effective open binder-design engine and the
field's practical standard.

## Limitations / disadvantages
- A **pipeline** (not a new architecture); inherits AF-Multimer's interface limits (see
  [`doc/shortcomings.md`](../../doc/shortcomings.md) §1.4 — antibody/complex docking).
- Success is **target-dependent**; difficult targets still need many designs.
- Closed/filtered loop can bias toward AF-favored interfaces.

## Benchmarks
- 10–100% experimental (SPR-validated) binder success across targets, generally outperforming
  RFdiffusion-only campaigns. (Source: Pacesa et al., Nature 2025.)

## Sources
- Paper: https://doi.org/10.1038/s41586-025-09429-6
- Code: https://github.com/martinpacesa/BindCraft
