---
name: MULTICOM4
field: prediction
category: all-atom-cofolding
year: 2025
venue: "bioRxiv (2025)"
doi: 10.1101/2025.03.06.641913
arxiv: null
citations: 5
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/BioinfoMachineLearning/MULTICOM4
stars: 17
stars_source: github-api
stars_as_of: 2026-07-04
license: null
tags: [all-atom-cofolding, multimer, ensemble]
pioneering: false
status: verified
---

## Key innovation
An **AF2/AF3-augmented multimer and complex prediction pipeline** from the Cheng lab (University of
Missouri) that combines multiple structure predictors with a ranking/MSA-pairing strategy. It ranked
**#1 in protein-complex prediction at CASP16** (TM=0.752, DockQ=0.584), demonstrating that careful
ensembling and input engineering around AlphaFold-family models can still beat single-model approaches
on difficult multimer targets.

## Limitations / disadvantages
- An **ensemble/pipeline** rather than a single learned model — heavier compute and engineering effort
  per target than running one network.
- Strength comes from aggregating AF2/AF3-class outputs, so its ceiling is tied to those base models.
- CASP performance is on a limited benchmark set; generalization to arbitrary heteromeric assemblies
  is not guaranteed.

## Benchmarks
- CASP16 protein-complex category: **#1 ranked team**, TM-score 0.752 and DockQ 0.584 on the
  complex targets. (Source: Cheng et al., bioRxiv 2025, 10.1101/2025.03.06.641913.)

## Sources
- Paper: https://doi.org/10.1101/2025.03.06.641913
- Code: https://github.com/BioinfoMachineLearning/MULTICOM4
