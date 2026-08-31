---
name: Protenix
field: prediction
category: all-atom-cofolding
year: 2025
venue: "bioRxiv (2025); 'Protenix – Advancing Structure Prediction Through a Comprehensive AlphaFold3 Reproduction'"
doi: 10.1101/2025.01.08.631967
citations: 145
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/bytedance/Protenix
stars: "~2k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [msa-based, all-atom, cofolding, diffusion]
status: verified
---

## Key innovation
ByteDance's **open-source, trainable PyTorch reproduction of AlphaFold3**, claimed to be the
first fully open-source model to **match/outperform AF3** on key benchmarks. Removes the
AlphaFold Server's ligand-type restrictions and ships with full training code, enabling
community fine-tuning and extension.

## Limitations / disadvantages
- A **reproduction**; inherits AF3's diffusion limitations (stereochemistry artifacts, static
  output).
- Training is compute-heavy; newest entry, so limited independent benchmarking.
- Slightly behind Boltz/Chai in community adoption so far.

## Benchmarks
- Reported AF3-parity or better on PoseBusters and complex benchmarks. (Source: Protenix team,
  bioRxiv 2025.)

## Sources
- Preprint: https://doi.org/10.1101/2025.01.08.631967
- Code: https://github.com/bytedance/Protenix
