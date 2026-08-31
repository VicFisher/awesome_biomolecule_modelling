---
name: rMD17 (Revised MD17)
field: mlip
category: qm-datasets
year: 2020
venue: "figshare dataset (2020); accompanying analysis arXiv 2002.02393"
doi: 10.6084/m9.figshare.12672038
arxiv: null
arxiv_note: "Dataset record (figshare); related analysis at arXiv 2002.02393"
citations: null
citations_note: "S2 lookup did not resolve a paper object — to backfill"
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: null
repo_note: "Dataset distributed via figshare / SchNetPack"
stars: null
stars_note: "No canonical repo to count"
tags: [qm-datasets, qm-data, benchmark-fix]
pioneering: false
status: draft
---

## Key innovation
A **re-evaluation of 10 MD17 molecules** with negligible numerical noise in the force and energy labels. The recompute exposed that the original MD17 forces contained DFT-convergence noise that acted as an **error floor** — many apparent accuracy gains on MD17 were below that floor and thus illusory. rMD17 is now the **preferred MD17 variant** for fair model comparison and is reported by most modern MLIP papers in place of legacy MD17.

## Limitations / disadvantages
- Same **small-molecule scope and single-trajectory sampling** as MD17 — only the *labels* were fixed, not the chemistry.
- Not a new dataset; comparability with older MD17 numbers is broken (numbers are not interchangeable).
- Still does not exercise large, flexible, or condensed-phase systems.

## Benchmarks
Same task as MD17 (energy/force MAE). Modern models (PaiNN, Allegro, MACE) report **lower and more reliable** rMD17 numbers than legacy MD17; the relative ranking of methods can shift versus noisy MD17. (Source: Christensen & von Lilienfeld, figshare 2020; analysis arXiv 2002.02393.)

## Sources
- Dataset: https://figshare.com/articles/dataset/Revised_MD17_dataset_rMD17_/12672038
- Analysis: https://arxiv.org/abs/2002.02393
