---
name: MIFST
field: design
category: inverse-folding
year: 2022
venue: "bioRxiv (2022); 'Masked inverse folding with sequence transfer for protein structure-based design'"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: null
tags: [inverse-folding, plm]
status: draft
institution: "Stanford University / Synthetic Genomics"
---

## Key innovation
A **masked inverse-folding structured graph network** trained with **sequence-transfer
(evolutionary) signals** — a representative PLM-augmented inverse-folding baseline that leverages
homolog information beyond a single backbone.

## Limitations / disadvantages
- Older baseline; largely superseded by ProteinMPNN / ESM-IF1.
- Single-backbone; depends on extra evolutionary input.
- No all-atom/multistate.

## Benchmarks
- Competitive sequence recovery using sequence-transfer features. (Source: MIFST, bioRxiv 2022.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.1101/2022.05.25.493516v2
