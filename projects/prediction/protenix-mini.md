---
name: Protenix-Mini
field: prediction
category: all-atom-cofolding
year: 2025
venue: "arXiv (2025)"
doi: 10.48550/arXiv.2507.11839
arxiv: 2507.11839
citations: 5
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/bytedance/Protenix
stars: 1977
stars_source: github-api
stars_as_of: 2026-07-04
license: Apache-2.0
tags: [all-atom-cofolding, cofolding, diffusion, efficient-inference]
pioneering: false
status: verified
_note: "Stars shared with the parent Protenix repository."
---

## Key innovation
A **compact variant of Protenix** (ByteDance's open AlphaFold3-style cofolder) that pairs a
reduced-capacity architecture with a **2-step ODE diffusion sampler** and a switchable protein
language-model module. The goal is to **drastically cut inference cost** while retaining most of
Protenix's accuracy across protein, ligand, nucleic-acid and ion complexes — making all-atom
co-folding practical on lighter hardware.

## Limitations / disadvantages
- Reduced architecture trades some accuracy for speed; can lag the full Protenix/AlphaFold3 on the
  hardest protein–ligand pose and protein–nucleic-acid cases.
- Inherits the diffusion-head artifacts of the AF3 family (clashes, stereochemistry issues).
- Benchmark depth is still limited (recent preprint, few external evaluations).

## Benchmarks
- Reports near-parity with full Protenix across FoldBench-style protein/complex tasks at substantially
  lower compute (few diffusion steps). (Source: Protenix-Mini, arXiv:2507.11839, 2025.)

## Sources
- Paper: https://arxiv.org/abs/2507.11839
- Code: https://github.com/bytedance/Protenix
