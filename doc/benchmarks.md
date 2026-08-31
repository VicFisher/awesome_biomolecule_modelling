# Benchmark Index

Cross-field reference for the benchmarks cited across the records. For each: **what it measures**, the **metric(s)**, and the **representative SOTA / reference point**. Numbers are indicative (the field moves fast) — always check the cited paper.

> Maintained alongside the records. Add entries as records reference new benchmarks.

---

## 1. Structure prediction

| Benchmark | Measures | Metric(s) | Notes |
|---|---|---|---|
| **CASP** (14/15/16) | Blind protein/complex structure prediction | GDT_TS, lDDT, DockQ (interfaces), TM-score | Biennial community assessment. CASP14 (2020) was AlphaFold2's debut (median GDT_TS ≈ 92); CASP16 (2024) added more complex/ligand categories. |
| **CAMEO** | Continuous (weekly) structure prediction | lDDT, GDT_TS | Easier than CASP; used to track folding servers over time. |
| **PoseBusters** | Protein–ligand pose validity (AF3-era) | pose RMSD, % valid (stereochemistry/clash checks) | The standard for judging AF3-class co-folding ligand poses; used by Boltz/Chai/Protenix. |
| **FoldBench** | All-atom complex benchmark | structure + interaction accuracy | Referenced by SeedFold (claims AF3-beating). |
| **PDB recent / time-cut** | Generalization to unseen PDB | lDDT, DockQ | Standard hold-out evaluation for new folders. |

## 2. Structure design

| Benchmark | Measures | Metric(s) | Notes |
|---|---|---|---|
| **Sequence recovery** | Inverse-folding quality | % native residues recovered | ProteinMPNN ≈ 52% (vs ~32–44% Rosetta). |
| **Designability** (AF2/MPNN round-trip) | Whether a design folds to the target | scTM, pLDDT of redesigned structure, MPNN recovery | The standard "does it fold" check; scTM ≥ 0.5 + pLDDT ≥ 70 typical pass. |
| **Binder success** | De novo binder functionality | % binders by SPR / BLI, Kd | RFdiffusion/Chroma binders; usually needs post-design screening + maturation. |
| **Activity assays** | Enzyme design function | kcat/KM, specificity | De novo luciferase (Yeh 2023) as a landmark. |

## 3. Machine-learning interaction potentials (MLIPs)

| Benchmark / dataset | Measures | Metric(s) | Notes |
|---|---|---|---|
| **MD17 / rMD17** | Small-molecule PES from short MD | energy RMSE (meV), force RMSE (meV/Å) | The classic MLIP benchmark; rMD17 is the corrected/revised version (more reliable). |
| **MD22** | Larger biomolecules (peptides, sugars, etc.) | energy/force RMSE | Tests long-range + larger systems than MD17. |
| **QM9** | Small organic molecule QM properties | MAE on energy, HOMO-LUMO, μ, α, etc. | 134k molecules; standard property-prediction benchmark. |
| **3BPA / ACE-PRED / MALU** | Out-of-distribution / drug-like transferability | force RMSE, free-energy/ΔΔG | Tests generalization beyond training distribution. |
| **SPICE** | Drug-like conformer energies/forces | energy/force RMSE | Designed for biomolecular/organic MLIP training (OpenMM). |
| **OC20 / OC22** | Catalytic surfaces (adsorbate+slab) | IS2RS (structure), IS2RE (energy), S2EF | Large-scale catalysis; OC22 adds oxides. |
| **rMD17 leaderboard** | Cross-model comparison | energy/force RMSE | The community comparison table for architecture quality. |

### Indicative MLIP SOTA context
- **Equivariant** models (NequIP, Allegro, MACE) generally dominate MD17/rMD17/QM9 accuracy per-parameter vs invariant ones (SchNet, DimeNet).
- **Foundational / universal** potentials (MACE-MP-0, SevenNet, Orb, AIMNet2, GNoME) trade some per-system accuracy for breadth across the periodic table / chemistry.

---

## Cross-cutting notes
- **Accuracy vs coverage** is the central tension in all three fields: AF2-class predictors are most accurate but need MSAs; MSA-free (PLM) models are faster but less accurate; foundational MLIPs are broad but less precise per-system.
- **Static vs dynamic**: structure predictors output single structures — methods like AF-Cluster, AFsample2, and MLIP-driven MD address conformational diversity.
- Benchmark numbers in individual records cite their origin (paper's own table or community re-evaluation); flag any that are community-reproduced rather than author-reported.
