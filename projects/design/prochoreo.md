---
name: ProChoreo
field: design
category: all-atom-binder-motif
year: 2026
venue: "bioRxiv (2026); de novo binder design from conformational ensembles"
citations: null
citations_note: "S2 lookup throttled / very recent — to backfill"
repo: null
tags: [binder, conformational-ensemble]
status: draft
---

## Key innovation
A binder-design framework that conditions generation on **conformational ensembles** of the target
(rather than a single static structure), using **ESM-2 3B** for sequence features — explicitly
targeting the single-static-structure gap noted in [`doc/shortcomings.md`](../../doc/shortcomings.md).

## Limitations / disadvantages
- Very recent preprint; limited independent validation.
- Needs ensemble inputs (costly to generate).
- Binder success not yet benchmarked at scale.

## Benchmarks
- Binder design conditioned on target ensembles (per preprint). (Source: ProChoreo, bioRxiv 2026.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.64898/2026.01.23.701298v2
