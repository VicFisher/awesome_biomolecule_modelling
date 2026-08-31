---
name: RoseTTAFold3 (RF3)
field: prediction
category: all-atom-cofolding
year: 2025
venue: "bioRxiv (2025); RoseTTAFold3"
doi: 10.1101/2025.08.14.670328
citations: 31
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/RosettaCommons/foundry
stars: 867
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
institution: Baker Lab (UW / IPD)
license: free for non-commercial
tags: [msa-based, all-atom, cofolding, diffusion]
status: draft
---

## Key innovation
The Baker lab's open-source **AF3-class all-atom co-folding** model, released as part of the
"Foundry" stack. Provides a fully open (non-commercial) alternative to AlphaFold3 for joint
protein/nucleic-acid/ligand prediction and design.

## Limitations / disadvantages
- Very recent; limited independent benchmarking.
- Non-commercial license; inherits diffusion-module artifacts (stereochemistry, symmetry).
- Compute-heavy.

## Benchmarks
- Reported competitive with AF3/Boltz on complex benchmarks (per preprint). (Source: RF3 preprint,
  bioRxiv 2025.)

## Sources
- Preprint: https://doi.org/10.1101/2025.08.14.670328
- Code: https://github.com/RosettaCommons/foundry
