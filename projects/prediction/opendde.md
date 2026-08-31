---
name: OpenDDE
field: prediction
category: all-atom-cofolding
year: 2026
venue: "Preview release / technical report (Jul 2026); 'An Open-source Drug Discovery Engine'"
doi: null
doi_note: "No formal paper/preprint yet — technical report referenced in repo"
arxiv: null
repo: https://github.com/aurekaresearch/OpenDDE
stars: 151
stars_source: shields.io (approx)
stars_as_of: 2026-07-06
citations: null
citations_note: "No paper published yet (preview software release) — to backfill"
license: Apache-2.0
tags: [all-atom, cofolding, diffusion]
pioneering: false
status: draft
institution: Aureka Research (aurekaresearch)
---

## Key innovation
An **open-source, all-atom biomolecular foundation model** that turns **co-folding into a scalable
engine for structure prediction, design, and drug-discovery optimization**. Built on the AlphaFold-3
ecosystem (AF3, Protenix, OpenFold, ColabFold), it ships a general-purpose checkpoint
(`opendde.pt`) and an **antibody-antigen-tuned** checkpoint (`opendde_abag.pt`), handles proteins,
DNA, RNA, ligands, and ions, and supports MSA/template/RNA-MSA preprocessing plus multi-GPU
(Fold-CP) inference. The repo emphasizes a scaling-law-driven training regime.

## Limitations / disadvantages
- **Preview release** — CLI/IO/checkpoints may change; predictions **not reproducible across
  versions**; not yet for production.
- **No peer-reviewed paper/preprint** (only an in-repo technical report) — claims await independent
  validation.
- Inherits AF3-class diffusion artifacts (stereochemistry, static output); training pipeline is
  closed (open weights/code only).

## Benchmarks
- None published in a paper yet; the repo provides a scaling-law figure. (Source: OpenDDE repo,
  2026-07-03 release.)

## Sources
- Code: https://github.com/aurekaresearch/OpenDDE
- Checkpoints: Hugging Face (`opendde.pt`, `opendde_abag.pt`)
