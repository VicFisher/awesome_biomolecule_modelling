---
name: dyMEAN
field: design
category: specialized
year: 2023
venue: "ICML 2023; 'End-to-end Full-Atom Antibody Design with dynamic Multichannel Equivariant graph Network'"
repo: https://github.com/THUNLP-MT/dyMEAN
repo_note: "repo path as listed in discovery; institution is Xiamen U"
stars: 133
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
tags: [antibody, inverse-folding, all-atom]
status: draft
institution: "Xiamen University (Kong, Huang, Liu)"
---

## Key innovation
**End-to-end full-atom, epitope-conditioned antibody design** — adaptively co-designs sequence and
structure at all-atom resolution given an antigen. Extends MEAN to full-atom, end-to-end design.

## Limitations / disadvantages
- **Antibody-only**; depends on a provided antigen structure.
- Designed binders typically need affinity maturation / experimental validation.
- Equivariant co-design is compute-heavy.

## Benchmarks
- Full-atom epitope-conditioned antibody design vs prior co-design baselines. (Source: dyMEAN, ICML
  2023.)

## Sources
- Paper: https://icml.cc/virtual/2023/poster/24962
- Code: https://github.com/THUNLP-MT/dyMEAN
