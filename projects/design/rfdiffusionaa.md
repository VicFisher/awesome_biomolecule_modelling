---
name: RFdiffusionAA (RoseTTAFold All-Atom)
field: design
category: all-atom-binder-motif
year: 2023
venue: "bioRxiv (2023); 'Generalized biomolecular modeling and design with RoseTTAFold All-Atom'"
citations: 897
citations_source: semantic-scholar
citations_as_of: 2026-07-04
repo: https://github.com/baker-laboratory/RoseTTAFold-All-Atom
stars: 810
stars_source: "shields.io (approx)"
stars_as_of: 2026-07-04
license: free for non-commercial (Baker lab)
tags: [all-atom, inverse-folding, binder, motif-scaffolding]
pioneering: true
status: verified
---

## Key innovation
The first **all-atom RoseTTAFold** that jointly models proteins, small-molecule ligands, nucleic
acids, and metals — enabling all-atom **cofolding and design** of complexes with non-protein
components. A pre-AlphaFold3 all-atom network that also underpins all-atom design (RFdiffusionAA
sequence/backbone design around ligands and cofactors).

## Limitations / disadvantages
- Compute-heavy; accuracy on protein–ligand interactions below later AF3-class models.
- All-atom design/validation still maturing; stereochemistry of non-protein components can be
  imperfect.
- Non-commercial license limits commercial use.

## Benchmarks
- Demonstrated all-atom modeling of protein–ligand–nucleic-acid complexes and design around
  cofactors/ligands. (Source: Krishna et al., bioRxiv 2023.)

## Sources
- Preprint: https://www.biorxiv.org/content/10.1101/2023.10.21.5638549
- Code: https://github.com/baker-laboratory/RoseTTAFold-All-Atom
