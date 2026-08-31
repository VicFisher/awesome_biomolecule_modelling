---
name: OpenMM-ML (ML potential plugin for OpenMM)
field: mlip
category: differentiable-md-qmmm
year: 2023
venue: "code-first project (OpenMM plugin); no single flagship paper"
doi: null
doi_note: "Code-first project — no canonical paper/DOI"
arxiv: null
arxiv_note: "No preprint"
citations: null
citations_note: "No paper object to cite — metrics N/A"
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/openmm/openmm-ml
stars: 175
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [differentiable-md-qmmm, differentiable-md, openmm, plugin, mixed-ml]
pioneering: false
status: draft
---

## Key innovation
A **software layer that runs ML potentials inside the OpenMM MD engine** with a uniform interface and the ability to mix ML and classical force terms (e.g., ML for the active site, classical for the rest). It wraps backends such as ANI, MACE, and TorchMD-Net as OpenMM `Force` objects, so a researcher can plug a modern MLP into an established, GPU-accelerated biomolecular simulation stack with minimal glue code. This is a **code-first, infrastructure project** rather than a method paper — its value is interoperability and adoption.

## Limitations / disadvantages
- **Not a method or paper** — there is no benchmark to cite; its impact is measured by downstream usage.
- Performance is bounded by the underlying ML potential and the host-device data movement.
- Coupling ML short-range terms with OpenMM's long-range PME / constraints requires care to remain energy-conserving.

## Benchmarks
No standalone benchmark; OpenMM-ML is exercised through downstream simulations (e.g., ANI/MACE in explicit solvent, mixed QM/MM-style setups). Functionally validated by its use in MLP-in-OpenMM workflows. (Source: openmm/openmm-ml repository & docs.)

## Sources
- Code & docs: https://github.com/openmm/openmm-ml
- OpenMM (host engine): https://github.com/openmm/openmm
