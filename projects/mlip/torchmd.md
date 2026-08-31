---
name: TorchMD
field: mlip
category: differentiable-md-qmmm
year: 2020
venue: "J. Chem. Theory Comput. 17, 2355 (2021)"
doi: 10.1021/acs.jctc.0c01343
arxiv: 2012.12106
citations: 225
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/torchmd/torchmd
stars: 711
stars_source: shields.io (approx)
stars_as_of: 2026-07-04
license: MIT
tags: [differentiable-md-qmmm, differentiable-md, pytorch, biomolecular, end-to-end]
pioneering: false
status: verified
---

## Key innovation
A PyTorch **molecular-dynamics engine** that expresses all bonded and nonbonded force terms — bonds, angles, torsions, Lennard-Jones, electrostatics — as **differentiable operators**, so that neural-network potentials (and mixed classical + ML force fields) can be trained and run end-to-end inside a single framework. TorchMD enabled **coarse-grained protein folding** learned from single-molecule trajectories and became the substrate for the TorchMD ecosystem (TorchMD-Net). It lowered the barrier between deep-learning frameworks and production MD for biomolecular simulation.

## Limitations / disadvantages
- **Not as fast** as specialized MD engines (OpenMM, GROMACS) for large-scale classical simulations — Python/PyTorch overhead.
- Learning an NNP end-to-end still requires substantial training data.
- Mixed ML/classical Hamiltonians need careful coupling to avoid integration artifacts.

## Benchmarks
Demonstrated learning of a coarse-grained NNP that **folds a small protein (chignolin) from a single trajectory**, and reproduced classical-FF observables via differentiable ops. (Source: Doerr et al., JCTC 2021.)

## Sources
- Paper: https://doi.org/10.1021/acs.jctc.0c01343
- Preprint: https://arxiv.org/abs/2012.12106
- Code: https://github.com/torchmd/torchmd
