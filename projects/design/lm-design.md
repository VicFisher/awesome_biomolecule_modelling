---
name: LM-Design
field: design
category: inverse-folding
year: 2023
venue: "ICML 2023; 'Structure-informed Language Models Are Protein Designers'"
citations: null
citations_note: "S2 lookup did not resolve — to backfill"
repo: null
tags: [inverse-folding, plm]
status: draft
institution: ByteDance
---

## Key innovation
A generic method to **reprogram a pretrained protein language model into a structure-conditioned
designer** by injecting structural information — marrying the PLM's powerful sequence prior with
inverse folding. Showed that PLMs can be efficiently adapted for structure-based sequence design
without training from scratch.

## Limitations / disadvantages
- Inherited PLM biases; structure-conditioning is a light adapter, not a full redesign.
- Single-backbone; no all-atom/multistate.
- Less widely adopted than ProteinMPNN as a production sequence designer.

## Benchmarks
- Improved sequence recovery over the base PLM and competitive with inverse-folding baselines.
  (Source: Zheng et al., ICML 2023.)

## Sources
- Paper: https://proceedings.mlr.press/v202/zheng23a/zheng23a.pdf
