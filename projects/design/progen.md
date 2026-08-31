---
name: ProGen
field: design
category: hallucination
year: 2023
venue: "Nature Biotechnology 41, 561–570 (2023); 'Large language models generate functional protein sequences across diverse families'"
doi: 10.1038/s41587-022-01618-2
citations: 1067
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/salesforce/progen
stars: 704
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: BSD-3-Clause (Salesforce)
tags: [sequence-generative, plm]
pioneering: true
status: verified
---

## Key innovation
An **autoregressive protein language model** trained on ~280M sequences with conditioning tags
(function, family, taxonomy), enabling **controllable, sequence-only generative design** across
diverse families. Generated lysozymes and dehydrogenases with measured activity — a landmark for
sequence-space generative design.

> **Taxonomy note:** categorized under `hallucination` (probability/generative-space design), but
> ProGen is really **sequence-only generative** (autoregressive LM) — distinct from AF2-style
> structure hallucination. A dedicated `sequence-generative` sub-category may be warranted (also
> covers ProtGPT2, EvoDiff).

## Limitations / disadvantages
- **Sequence-only** — no explicit structure; limited control over 3D fold.
- Outputs need filtering/validation; can drift from natural distributions.
- Conditioning-tag coverage limits controllability for novel functions.

## Benchmarks
- Generated functional enzymes (lysozyme, malate dehydrogenase) with wild-type-level activity.
  (Source: Madani et al., Nat Biotechnol 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41587-022-01618-2
- Code: https://github.com/salesforce/progen
