---
name: AlphaFold2
field: prediction
category: msa-based
year: 2020
venue: "Nature 596, 583–589 (2021)"
preprint: "2020-07-15, deepmind.com (preprint); CASP14 debut 2020"
doi: 10.1038/s41586-021-03819-2
citations: 36985
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/deepmind/alphafold
stars: "~15k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
website: https://alphafold.ebi.ac.uk
license: Apache-2.0
tags: [msa-based, evoformer, multimer]
pioneering: true
status: verified
---

## Key innovation
First end-to-end differentiable network to predict protein structures to near-experimental
accuracy from sequence + MSA. The architecture pairs the **Evoformer** (which co-evolves a
row/column MSA representation with a residue-pair representation) with a **structure module**
that uses invariant point attention (IPA) over rigid residue frames to output all-atom
coordinates. It introduced **recycling** (iterative refinement) and **calibrated confidences**
— per-residue pLDDT and per-pair PAE. CASP14 (2020) was a step-change: median GDT_TS ≈ 92.4,
effectively "solving" single-chain structure prediction.

## Limitations / disadvantages
- Outputs a **single static structure**, not conformational ensembles or dynamics.
- Weaker for **intrinsically disordered regions** and for proteins with shallow MSAs
  (orphans / low homologs), since accuracy depends on MSA depth.
- **pLDDT/PAE are less calibrated** for multimer interfaces and alternative conformational
  states.
- Occasional **stereochemical errors** (clashes, bond geometry); not designed for non-protein
  atoms (ligands, RNA, ions) — later addressed by AlphaFold-Multimer and AlphaFold3.

## Benchmarks
- **CASP14** (2020): median GDT_TS **92.4**, vs ≈87 for the next-best method; roughly two
  thirds of targets judged within experimental error. (Source: Jumper et al., Nature 2021;
  CASP14 assessor report.)

## Sources
- Paper: https://doi.org/10.1038/s41586-021-03819-2
- Code: https://github.com/deepmind/alphafold
- Database / website: https://alphafold.ebi.ac.uk
- CASP14 results summary: https://predictioncenter.org/casp14/zscores_final.cgi
