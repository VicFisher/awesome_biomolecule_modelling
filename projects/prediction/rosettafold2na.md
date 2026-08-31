---
name: RoseTTAFold2NA (RF2NA)
field: prediction
category: all-atom-cofolding
year: 2023
venue: "Nature Methods 20, 464–471 (2024)"
citations: 300
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/uw-ipd/RoseTTAFold2NA
stars: 378
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Baker Lab (UW / IPD)
tags: [msa-based, all-atom, cofolding, nucleic-acid]
status: verified
---

## Key innovation
An AF2-class network specialized for **protein–nucleic-acid complexes** (protein + DNA/RNA),
predicting their joint structure from sequence/MSA. Filled a gap left by AlphaFold2 (which handled
only protein) before AlphaFold3 generalized all-atom co-folding.

## Limitations / disadvantages
- Focused on **protein–nucleic acid** (not full small-molecule ligands).
- MSA-dependent; accuracy below AlphaFold3 on some complex benchmarks.
- Single static structure.

## Benchmarks
- Improved protein–DNA/RNA interface prediction over AF2/AF-Multimer. (Source: Baek et al., Nat
  Methods 2024.)

## Sources
- Paper: https://www.nature.com/articles/s41592-024-02257-9
- Code: https://github.com/uw-ipd/RoseTTAFold2NA
