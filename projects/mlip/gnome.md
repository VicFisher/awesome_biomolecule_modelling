---
name: GNoME
field: mlip
category: foundational-universal
year: 2023
venue: "Nature 624, 95–102 (2023)"
doi: 10.1038/s41586-023-06735-9
arxiv: null
arxiv_note: "No arXiv preprint — published directly in Nature"
citations: 1437
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/google-deepmind/materials_discovery
stars: 1200
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
tags: [foundational-universal, foundational, universal, inorganic, materials-discovery]
pioneering: false
status: verified
---

## Key innovation
A scaled GNN for predicting **inorganic crystal stability** that discovered **2.2 million new crystals (~380k stable)** — an order-of-magnitude expansion of humanity's known stable materials. GNoME demonstrated **scaling laws for stable-structure prediction**: with enough data and compute, learned potentials/formation-energy models generalize across the inorganic compositional space. It is a **materials-discovery flagship, NOT a biomolecular method** — included here as a foundational-universal atomistic model whose impact and scale set the agenda for universal MLPs.

## Limitations / disadvantages
- **Strictly inorganic / materials** — not applicable to biomolecules, organics, or MD of soft matter.
- Focuses on **thermodynamic stability** of crystals (formation energy), not on dynamics or accurate forces for MD.
- Closed training pipeline and dataset assembly; reproducibility depends on the released structures, not the full pipeline.

## Benchmarks
- 2.2M candidate structures, ~380k stable on the convex hull; independently corroborated by DFT and by experimental databases. (Source: Merchant et al., Nature 2023.)

## Sources
- Paper: https://doi.org/10.1038/s41586-023-06735-9
- Discovered structures: https://github.com/google-deepmind/materials_discovery
- Nature news: https://www.nature.com/articles/d41586-023-03645-6
