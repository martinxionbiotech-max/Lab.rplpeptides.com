---
description: "On-resin chemical modifications — acetylation, biotinylation, fluorescent labeling, phosphorylation, and other common peptide modifications."
---

# On-Resin Modifications

## TL;DR

On-resin modifications introduce functional groups to the peptide while it remains attached to the solid support, enabling regioselective derivatization that would be difficult or impossible in solution. Common modifications include N-terminal acetylation, biotinylation, fluorescent labeling (FITC, FAM, Cy5), and phosphorylation of Ser/Thr/Tyr side chains.

---

## Advantages of On-Resin Modification

| Advantage | Description |
|---|---|
| **Regioselectivity** | Only the resin-bound N-terminus (or selectively deprotected side-chain) is modified |
| **Purification by washing** | Excess reagent is simply washed away |
| **High yield** | Large reagent excess drives modification to completion |
| **Automation** | Modification steps can be integrated into automated SPPS |
| **Minimal handling** | No intermediate purification between synthesis and modification |

---

## Common On-Resin Modifications

### 1. N-Terminal Acetylation

The most common on-resin modification. Blocks the N-terminal amine to neutralize charge and improve stability.

| Parameter | Standard Protocol |
|---|---|
| Reagent | Acetic anhydride (Ac₂O) |
| Base | DIEA or NMM |
| Solvent | DMF or DCM |
| Reagent concentration | 5–10% Ac₂O, 5–10% DIEA in DMF |
| Reaction time | 10–20 min at RT |
| Completion check | Kaiser test (should be negative/yellow) |

**Note**: Same protocol as capping — capping IS acetylation. When performing intentional N-terminal acetylation, use a fresh solution and sufficient time (20 min) for complete conversion.

### 2. Biotinylation

Biotin labeling enables streptavidin-based detection, purification, and immobilization.

| Biotin Reagent | Coupling Method | Notes |
|---|---|---|
| D-Biotin | DIC/HOBt or HATU/DIEA activation | Standard, requires pre-activation 10–15 min |
| Biotin-OSu (NHS-biotin) | Direct coupling, no activation needed | Faster, pre-activated ester |
| Biotin-PEG₄-OSu | Direct coupling | Adds PEG spacer to reduce steric hindrance |
| Biotin-PEG₁₂-COOH | HATU/DIEA activation | Longer spacer for surface binding |

**Protocol**:
1. Deprotect N-terminal Fmoc (standard method)
2. Activate 3 eq of D-biotin with 2.9 eq DIC in DMF (10 min, RT)
3. Add to resin, react 1–2 h at RT
4. Check Kaiser test; repeat if positive

### 3. Fluorescent Labeling (FITC, FAM, Cyanine Dyes)

Used for imaging, flow cytometry, and FRET-based assays.

| Dye | Reagent | Excitation/Emission | Coupling Conditions |
|---|---|---|---|
| FITC | FITC isomer I | 495/519 nm | 3 eq FITC + 6 eq DIEA in DMF, 2–4 h, dark |
| 5(6)-FAM | 5(6)-FAM-OSu | 494/521 nm | 2 eq FAM-OSu + 4 eq DIEA, 1 h, dark |
| TAMRA | TAMRA-OSu | 555/580 nm | 2 eq + 4 eq DIEA, 1 h, dark |
| Cy3 | Cy3-NHS ester | 550/570 nm | 1.5 eq + 3 eq DIEA, 30 min, dark |
| Cy5 | Cy5-NHS ester | 649/670 nm | 1.5 eq + 3 eq DIEA, 30 min, dark |

**Critical considerations**:
- Perform fluorescent modifications in the dark (aluminum foil wrap)
- Use NMM instead of DIEA for pH-sensitive dyes
- Check dye stability — some NHS esters hydrolyze quickly
- Add a spacer (e.g., β-Ala, Ahx, PEG) between peptide and dye to reduce quenching

### 4. Phosphorylation

On-resin phosphorylation of Ser, Thr, or Tyr side chains using protected phosphoramidite chemistry or phosphates.

| Method | Reagent | Deprotection | Notes |
|---|---|---|---|
| Phosphoramidite | Bis(tert-butyl)-N,N-diisopropylphosphoramidite | TFA (global deprotection) | Requires oxidation step (I₂/H₂O) |
| Boc-protected phosphate | Fmoc-Ser(PO(OBzl)OH)-OH | HF (Boc strategy) | Pre-built amino acid |
| Commercially available | Fmoc-Ser(PO(OAll)OH)-OH | Pd(0) + TFA | Orthogonal approach |

**Phosphoramidite protocol**:
1. Synthesize peptide with unprotected Ser/Thr/Tyr (no side-chain protection for the target residue)
2. Couple 10 eq bis(tert-butyl)phosphoramidite + 5 eq tetrazole in THF (30 min)
3. Oxidize with I₂/H₂O/pyridine/THF (0.02 M, 30 min)
4. Global deprotection with TFA (phosphates deprotected to free PO₄)

---

## Less Common But Useful On-Resin Modifications

| Modification | Reagent | Application |
|---|---|---|
| Peptide Nucleic Acid (PNA) | PNA monomer activation | Peptide-PNA conjugates |
| Glycosylation | Fmoc-AA-(glycan)-OH (pre-built) | Glycopeptide synthesis |
| Pegylation | Fmoc-NH-PEGₙ-COOH | Peptide-PEG conjugates |
| Sulfation | Fmoc-Tyr(SO₃Na)-OH | Tyrosine sulfate peptides |
| Palmitoylation | Palmitic acid/DIC/HOBt | Lipopeptides, membrane anchoring |
| Maleimide conjugation | N-(β-maleimidopropyloxy)succinimide ester | Thiol-reactive peptides |

---

## General On-Resin Modification Protocol

1. **Verify** the target functional group is free (N-terminal, or selectively deprotected Lys, Cys, etc.)
2. **Wash** resin thoroughly with the modification solvent (usually DMF)
3. **Add modification reagent** (3–5 eq, pre-activated if needed)
4. **React** for the specified time at RT (or 40–50 °C for difficult modifications)
5. **Wash** thoroughly (DMF × 3, DCM × 3)
6. **Check completion** by Kaiser test or colorimetric assay
7. **Proceed** to cleavage or next synthesis step

---

## Key Takeaways

- On-resin modifications exploit the purification-by-washing advantage of SPPS
- Biotinylation and fluorescent labeling are the most requested custom modifications
- Fluorescent dyes require light protection; use NMM for pH-sensitive conjugations
- On-resin phosphorylation requires phosphoramidite or pre-protected phosphate chemistry
- A short spacer (β-Ala, Ahx, PEG) improves detection and reduces steric interference for large labels

> 🔗 Related: [Capping Strategies](../manufacturing/capping-strategies.md) | [Coupling Reaction](./coupling-reaction.md) | [Custom Synthesis](./custom-synthesis.md) | [Difficult Sequences](./difficult-sequences.md) | [Protecting Group Strategies](../manufacturing/protecting-group-strategies.md) | [Peptide Synthesizer](../equipment/peptide-synthesizer.md)
