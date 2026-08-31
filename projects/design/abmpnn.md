---
name: AbMPNN
field: design
category: inverse-folding
year: 2023
venue: "bioRxiv (2023); antibody-specific fine-tuned ProteinMPNN"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: null
tags: [inverse-folding, antibody]
status: draft
institution: "Adaptyv Bio / ETH Zurich (Dreyer et al.)"
---

## Key innovation
An **antibody-specific inverse-folding model fine-tuned from ProteinMPNN** on antibody structures,
specializing the general sequence designer for CDR sequence design. Widely used as a lightweight
antibody design component.

## Limitations / disadvantages
- **Antibody-only**; depends on the ProteinMPNN base.
- Fixed-backbone; no simultaneous structure redesign.
- Newer antibody IFs (AntiFold, IgMPNN) report higher CDR accuracy.

## Benchmarks
- Improved antibody CDR recovery over base ProteinMPNN. (Source: Dreyer et al., bioRxiv 2023.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.1101/2024.12.16.628614v1
