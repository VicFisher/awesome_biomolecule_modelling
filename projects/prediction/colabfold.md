---
name: ColabFold
field: prediction
category: msa-based
year: 2021
venue: "Nature Methods 18, 979–982 (2022)"
doi: 10.1038/s41592-022-01488-1
citations: 7599
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/sokrypton/ColabFold
stars: "~2.8k"
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: AGPL-3.0 / MIT (mixed)
tags: [msa-based]
status: verified
---

## Key innovation
Not a new folding algorithm but the **accessibility layer** that democratized AlphaFold2:
AF2 (later AF-Multimer, RoseTTAFold) run in a Google Colab notebook, paired with fast
**MMseqs2** MSA generation replacing the slow Jackhmmer pipeline. It became the de-facto way
most researchers first used AF2 and is extremely heavily cited as a result.

## Limitations / disadvantages
- No accuracy gain over the underlying AF2 — it is a deployment wrapper.
- Constrained by Colab/cloud runtime and memory (large complexes need local install).
- Depends on MMseqs2 MSA quality for hard targets.

## Benchmarks
- Reported near-identical accuracy to local AF2 at a fraction of the setup effort; benchmarks
  in the paper focus on MSA-generation speed and usability. (Source: Mirdita et al., Nat
  Methods 2022.)

## Sources
- Paper: https://doi.org/10.1038/s41592-022-01488-1
- Code: https://github.com/sokrypton/ColabFold
- Server: https://colabfold.com
