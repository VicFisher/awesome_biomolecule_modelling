---
name: FARFAR2
field: prediction
category: rna
year: 2020
venue: "Rosetta; Nature Methods (2020); de novo RNA modeling"
citations: null
citations_note: "S2 lookup throttled — to backfill"
repo: null
tags: [rna, pre-dl-contact]
pioneering: true
status: draft
institution: "Das lab (Univ. Washington) / Baker lab lineage"
---

## Key innovation
The standard **fragment-based de novo RNA 3D modeling** tool in the Rosetta suite — assembles RNA
structures from fragment libraries (FARFAR = Fragment Assembly of RNA) for structures up to ~250
nucleotides, also supporting homology modeling. The dominant **pre-deep-learning** RNA structure
approach and still competitive for small RNAs.

## Limitations / disadvantages
- **Fragment-assembly** — compute-heavy and stochastic; needs many decoys.
- Largely superseded by DL RNA folders (RhoFold+, DRFold) on larger/novel RNAs.
- Single-chain focus.

## Benchmarks
- RNA-Puzzles benchmarks; competitive on small motifs. (Source: RosettaCommons FARFAR2 docs.)

## Sources
- Docs: https://docs.rosettacommons.org/docs/latest/FARFAR2
