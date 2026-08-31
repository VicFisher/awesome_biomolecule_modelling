---
name: AF-Cluster
field: prediction
category: msa-based
year: 2024
venue: "Nature 625, 112–115 (2024)"
citations: 451
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "analysis code via authors; no single canonical repo"
tags: [msa-based, conformational-ensemble]
status: verified
---

## Key innovation
Addresses AlphaFold2's **single-structure** limitation by **clustering the input MSA** into
sub-alignments and predicting a structure per cluster — thereby recovering **multiple
conformational states** (alternative folds/active vs inactive states) from a single sequence. A
simple, influential idea for conformational-ensemble prediction.

## Limitations / disadvantages
- Only captures states **represented in the MSA**; depends on deep, diverse alignments.
- No explicit ligand/state conditioning; clusters are unsupervised.
- Less accurate on conformational detail than dedicated multi-state methods.

## Benchmarks
- Recovered known alternative conformations (e.g. transporter states) on benchmark proteins.
  (Source: AF-Cluster, Nature 2024.)

## Sources
- Paper: https://doi.org/10.1038/s41586-023-06832-9
