---
name: ZymCTRL
field: design
category: specialized
year: 2022
venue: "preprint (2022); controllable enzyme-sequence generation"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: null
tags: [enzyme, sequence-generative, plm]
status: draft
institution: "AI drug-discovery group (Controllable generation)"
---

## Key innovation
**Controllable generation of enzyme sequences conditioned on EC numbers** — a protein language
model trained with control tags specifying the reaction class, enabling targeted generation of
sequences for a desired catalytic function. A pioneer of **controllable, function-conditioned
sequence design** (the enzyme analogue of ProGen's tag-conditioned generation).

## Limitations / disadvantages
- **Sequence-only** — no explicit 3D structure or active-site geometry.
- Generates sequences of the right family but typically **low/no measured activity** without
  screening.
- Older; superseded for structure-aware enzyme design by RFdiffusion-family methods.

## Benchmarks
- Generated enzymes of the target EC class; activity required experimental screening.
  (Source: ZymCTRL, 2022 preprint.)

## Sources
- Reference: controllable-generation / ProGen-lineage enzyme papers (DOI to confirm).
