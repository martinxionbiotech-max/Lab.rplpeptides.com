---
description: "Boc amino acid specifications — side-chain protection patterns, Boc vs. Fmoc SPPS comparison, TFA cleavage conditions, historical context, and applications in specialised peptide synthesis."
---

# Boc Amino Acids

## Nᵅ-tert-Butyloxycarbonyl-Protected Amino Acids for Boc SPPS

## Introduction

Boc (tert-butyloxycarbonyl) protected amino acids are the building blocks of Boc SPPS, the original Merrifield solid-phase method first demonstrated in 1963. In this strategy, the temporary Nᵅ-amino protecting group is a Boc carbamate that is removed under mildly acidic conditions (typically 50% TFA/DCM), while semi-permanent side-chain protecting groups are chosen to survive repeated Boc deprotection cycles and are removed only during final HF or TFMSA cleavage. Although Fmoc chemistry dominates contemporary peptide synthesis, Boc SPPS retains critical applications in the production of peptides containing motifs that are problematic under basic conditions, such as C-terminal amides from base-sensitive linkers, peptides with ester bonds, and sequences prone to base-catalysed aspartimide formation.

## Boc vs. Fmoc — Comprehensive Comparison

| Feature | Boc Chemistry | Fmoc Chemistry |
|---------|--------------|----------------|
| **Nᵅ-protecting group** | tert-Butyloxycarbonyl (Boc) | 9-Fluorenylmethoxycarbonyl (Fmoc) |
| **Deprotection mechanism** | Acidolysis (TFA) | β-Elimination (piperidine base) |
| **Deprotection conditions** | 30–50% TFA/DCM, 20–30 min | 20% piperidine/DMF, 2 × 5–15 min |
| **Final cleavage** | HF (anhydrous, 0 °C, 1 h) or TFMSA | 95% TFA, 1.5–3 h |
| **Equipment required** | Anhydrous HF apparatus (specialised, high safety barrier) | Standard glassware, fume hood |
| **Side-chain protection** | Benzyl-based (Bzl, Tos, ClZ, BrZ) — stable to TFA | tBu, Trt, Boc, Pbf — cleaved by TFA |
| **Racemisation risk** | Lower for base-sensitive residues (His, Cys) | Higher for base-sensitive residues; mitigated by additives |
| **Resin types** | Merrifield (chloromethyl), PAM, MBHA | Wang, Rink Amide, Sieber, 2-Cl-Trt |
| **Coupling reagents** | DCC/HOBt, BOP, PyBOP, HBTU | HBTU, HATU, DIC/Oxyma, COMU |
| **Solvent** | DCM (primarily), DMF | DMF (primarily), NMP |
| **Washing** | DCM, DMF, alcohol | DMF, DCM |
| **Aspartimide suppression** | Inherent (neutral/acidic deprotection) | Requires additive (Oxyma, HOBt in deprotection step) |
| **Tyr sulfation** | Compatible (no piperidine) | Incompatible (piperidine removes sulfate) |
| **Phosphopeptide synthesis** | Compatible (acid-stable phosphoesters) | Requires special phosphate protection |
| **Historical usage** | 1963–2000s (original method) | 1990s–present (dominant method) |
| **Safety** | HF is extremely hazardous; TFMSA is very corrosive | TFA is corrosive but manageable |
| **Scale-up feasibility** | Lower (HF limitations) | Excellent (TFA scale-up well-established) |
| **Cost per synthesis** | Lower (cheaper reagents, higher yields) | Higher (Fmoc-amino acids more expensive) |

## Common Side-Chain Protection Patterns in Boc SPPS

| Amino Acid | Standard Side-Chain Protection | Cleavage Condition | Comments |
|-----------|-------------------------------|-------------------|----------|
| Arg | Tos (tosyl) | HF or TFMSA (hard acid, >0 °C) | Most difficult to cleave fully; HF preferred |
| Arg | Mts (mesitylene-2-sulfonyl) | TFMSA/TFA | Alternative to Tos, cleaves under milder conditions |
| Asp | OBzl (benzyl ester) | HF | Susceptible to aspartimide formation at Asp-Gly sequences |
| Cys | pMeBzl (4-methylbenzyl) | HF | Standard for Cys protection in Boc SPPS |
| Cys | Acm (acetamidomethyl) | Hg(II) or I₂ | Enables selective disulfide formation |
| Glu | OBzl (benzyl ester) | HF | Analogue of Asp protection |
| His | Bom (benzyloxymethyl) | HF | Prevents racemisation |
| His | Dnp (dinitrophenyl) | Thiolysis (before HF) | Coloured; must be removed before HF |
| Lys | ClZ (2-chlorobenzyloxycarbonyl) | HF/TFMSA | More acid-labile than Z; preferred |
| Lys | Fmoc | 20% piperidine/DMF | Orthogonal protection for selective modifications |
| Met | None (sulfoxide protection optional) | — | Susceptible to oxidation during workup |
| Ser | Bzl (benzyl) | HF | Minimal racemisation |
| Thr | Bzl (benzyl) | HF | Minimal racemisation |
| Trp | CHO (formyl) | HF (or base treatment) | Protects against alkylation; removed during HF |
| Trp | Boc | HF | Alternative to CHO; less stable |
| Tyr | BrZ (2-bromobenzyloxycarbonyl) | HF | Prevents O-benzylation |
| Tyr | Cl₂Bzl (2,6-dichlorobenzyl) | HF | More stable than BrZ |

## TFA Cleavage Conditions in Boc SPPS

In Boc chemistry, TFA is used for the repeated removal of the Nᵅ-Boc protecting group, not for final peptide cleavage from the resin (which requires HF or TFMSA).

| Application | TFA Concentration | Time | Temperature | Notes |
|------------|------------------|------|-------------|-------|
| Standard Boc deprotection | 50% TFA/DCM (v/v) | 20–30 min | Room temperature | Contains 2% anisole or m-cresol as hydride scavenger |
| Boc deprotection (sensitive sequences) | 30% TFA/DCM | 30–45 min | Room temperature | Slower but gentler for acid-sensitive AAs |
| Boc deprotection (accelerated) | 65% TFA/DCM | 15–20 min | Room temperature | For sterically hindered Boc-amino acids |
| Pre-HF Boc removal (final deprotection) | 100% TFA | 5 min | Room temperature | Single treatment before HF cleavage |
| Boc removal from NH₂-terminal | 33% TFA/DCM | 25 min | 0 °C (ice bath) | Minimises side reactions for very long sequences |

**Scavengers in TFA deprotection:** Anisole (2%, v/v) is the standard scavenger for Boc deprotection cycles. It traps tert-butyl cations released from Boc groups, preventing re-alkylation of sensitive residues (Met, Trp). The coloured t-butyl anisole adducts are removed during subsequent DCM washes.

## Historical Context and Current Relevance

Boc SPPS was the first practical method for automated solid-phase peptide synthesis. R. B. Merrifield's Nobel Prize-winning work (1984) relied entirely on Boc chemistry. Key milestones:

| Year | Milestone |
|------|-----------|
| 1963 | First Boc SPPS published by Merrifield ([Leu]-Ala-Gly-Val) |
| 1969 | First automated peptide synthesiser (Beckman 990) using Boc chemistry |
| 1970s | Routine synthesis of ribonuclease A (124 AA) by Gutte & Merrifield |
| 1980s | Widespread adoption of Boc SPPS for therapeutic peptide discovery |
| 1990s | Gradual transition to Fmoc chemistry as equipment and protecting group costs decreased |
| 2000s–present | Boc reserved for specialised applications |

**Current use cases for Boc SPPS:**
- Peptides with base-sensitive modifications (ester-linked, phosphate, sulfated Tyr)
- Sequences with high Asp-Gly or Asn-Gly motifs (aspartimide-free)
- Production of peptide thioesters (for native chemical ligation)
- Synthesis of D-amino acid-containing peptides (reduced racemisation)
- Peptide–polymer conjugates where base exposure is undesirable
- Historical reference peptides and assay standards

## Specifications for Procurement

| Parameter | Research Grade | GMP Grade |
|-----------|---------------|-----------|
| Purity (HPLC) | ≥98% | ≥99% |
| Optical purity (ee) | ≥99.0% | ≥99.5% |
| Water content (KF) | ≤0.5% | ≤0.2% |
| TFA content | ≤0.1% | ≤0.05% |
| Appearance | White powder | White crystalline powder |
| Storage | 2–8 °C, desiccated | 2–8 °C, desiccated, sealed |

---

> **🔗 Related:** [Fmoc Amino Acids](./fmoc-amino-acids.md) | [SPPS Process](../process/spps-process.md) | [TFA](./tfa.md) | [Resin Comparison Guide](./resin-comparison-guide.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
