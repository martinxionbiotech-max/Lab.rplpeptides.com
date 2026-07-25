---
description: "Comprehensive resin comparison guide for Fmoc SPPS — Wang, Rink Amide, Rink Acid, Sieber, and 2-Cl-Trt resins with loading capacities, swelling, and cleavage condition tables."
---

# Resin Comparison Guide for Fmoc Solid-Phase Peptide Synthesis

## Introduction

Resin selection determines both the C-terminal functionality of the synthesized peptide and the synthetic strategy. The resin serves as the solid support — it must swell adequately in the reaction solvents, provide accessible reaction sites with appropriate loading, and release the peptide cleanly under conditions compatible with side-chain protecting groups. This guide compares the five most common resins used in Fmoc SPPS.

## Resin Chemistry Overview

### Wang Resin

**Structure:** 4-(hydroxymethyl)phenoxymethyl-copoly(styrene-1% DVB)  
**Linker:** p-alkoxybenzyl alcohol  
**Peptide-resin bond:** Ester bond via C-terminal carboxyl group

Wang resin is the most widely used support for peptides with C-terminal carboxylic acids.

| Property | Value |
|----------|-------|
| Typical loading | 0.3–1.2 mmol/g |
| Swelling (DMF) | 4–6 mL/g |
| Swelling (DCM) | 6–8 mL/g |
| Swelling (MeOH) | 2–3 mL/g |
| Cleavage | TFA 95% (1–2 h) |
| C-terminal product | Carboxylic acid (–COOH) |
| Pore size (if Tentagel) | 90–130 µm |
| Cost | Low |

**Best for:** C-terminal acid peptides, standard Fmoc SPPS, routine synthesis

**Caution:** The ester bond is susceptible to diketopiperazine (DKP) formation during the second amino acid coupling. DKP is minimized by coupling the second amino acid with HATU and using short coupling times.

### Rink Amide Resin

**Structure:** 4-[(2,4-dimethoxyphenyl)(Fmoc-amino)methyl]phenoxy-copoly(styrene-1% DVB)  
**Linker:** Rink amide linker  
**Peptide-resin bond:** Amide bond

Rink Amide resin produces C-terminal amide peptides — the most common form for therapeutic and research peptides.

| Property | Value |
|----------|-------|
| Typical loading | 0.2–0.7 mmol/g |
| Swelling (DMF) | 5–7 mL/g |
| Swelling (DCM) | 7–9 mL/g |
| Cleavage | TFA 95% (1–2 h) |
| C-terminal product | Primary amide (–CONH₂) |
| Acid sensitivity | Very acid-labile linker |
| Cost | Moderate |

**Best for:** C-terminal amide peptides (majority of therapeutic peptides), standard synthesis

**Note:** The Rink linker is based on a benzhydrylamine scaffold. It is very acid-labile — use 95% TFA for 1–2 h. Avoid TFA traces during synthesis as premature cleavage can occur.

### Rink Acid Resin

**Structure:** Similar to Rink Amide with a carboxyl group at the attachment point  
**Linker:** Rink acid linker  
**Peptide-resin bond:** Ester bond

Rink Acid resin allows amidation of the N-terminus and produces C-terminal acid peptides.

| Property | Value |
|----------|-------|
| Typical loading | 0.4–0.8 mmol/g |
| Cleavage | TFA 95% (1–2 h) |
| C-terminal product | Carboxylic acid (–COOH) |
| Cost | Moderate |

**Best for:** C-terminal acid peptides requiring very mild cleavage

### Sieber Resin

**Structure:** Xanthenyl-amide linked to polystyrene  
**Linker:** Sieber amide linker (xanthenyl-amine)  
**Peptide-resin bond:** Amide bond

Sieber resin is unique — it is the most acid-labile resin in common use. It allows side-chain deprotection while keeping the peptide on-resin, enabling fragment synthesis and protected peptide intermediate strategies.

| Property | Value |
|----------|-------|
| Typical loading | 0.2–0.7 mmol/g |
| Swelling (DMF) | 4–6 mL/g |
| Cleavage | TFA 1–5% in DCM |
| C-terminal product | Primary amide (–CONH₂) |
| Acid sensitivity | Extremely acid-labile |
| Cost | Higher |

**Best for:** Protected peptide fragments (convergent synthesis), Nⁿ-alkylated peptides, cyclic peptides, side-chain-protected peptide intermediates

**Critical note:** Sieber resin cleavage requires only 1–5% TFA in DCM, leaving all side-chain protecting groups (tBu, Boc, Pbf, Trt) intact. This makes it the resin of choice for fragment condensation strategies.

### 2-Chlorotrityl Chloride (2-Cl-Trt) Resin

**Structure:** 2-chlorotrityl chloride bound to polystyrene  
**Linker:** Trityl chloride

2-Cl-Trt resin is the most versatile support for producing C-terminal protected peptides. It allows the peptide to be cleaved with very mild acid, preserving side-chain protecting groups.

| Property | Value |
|----------|-------|
| Typical loading | 0.4–1.6 mmol/g |
| Swelling (DMF) | 5–7 mL/g |
| Swelling (DCM) | 8–10 mL/g |
| Cleavage (protected) | AcOH/TFE/DCM (1:1:3) or TFA 1% in DCM |
| Cleavage (deprotected) | TFA 95% (1–2 h) |
| C-terminal product | Free acid or protected acid |
| Cost | Moderate |

**Best for:** Protected peptide fragments, side-chain-protected peptides, C-terminal-modified peptides (esters, thioesters), head-to-side-chain cyclic peptides

**Key advantage:** The chloride group on the trityl linker reacts directly with the C-terminal Fmoc-amino acid without pre-activation. The first amino acid loading is typically performed with DIEA in DCM.

## Resin Property Comparison Table

| Property | Wang | Rink Amide | Rink Acid | Sieber | 2-Cl-Trt |
|----------|------|------------|-----------|--------|----------|
| **Linker type** | p-Alkoxybenzyl alcohol | Rink amide | Rink acid | Xanthenyl-amide | Trityl chloride |
| **C-terminal product** | COOH | CONH₂ | COOH | CONH₂ | COOH or protected COOH |
| **Loading range (mmol/g)** | 0.3–1.2 | 0.2–0.7 | 0.4–0.8 | 0.2–0.7 | 0.4–1.6 |
| **Swelling DMF (mL/g)** | 4–6 | 5–7 | 4–6 | 4–6 | 5–7 |
| **Swelling DCM (mL/g)** | 6–8 | 7–9 | 6–8 | 6–8 | 8–10 |
| **Cleavage reagent (standard)** | 95% TFA | 95% TFA | 95% TFA | 1–5% TFA/DCM | 1% TFA/DCM or AcOH/TFE/DCM |
| **Cleavage time (rt)** | 1–2 h | 1–2 h | 1–2 h | 5–30 min | 30–60 min |
| **Protected peptide cleavage** | No | No | No | Yes | Yes |
| **Side-chain PGs retained?** | No | No | No | Yes | Yes |
| **DKP risk** | Moderate | Low | Moderate | Low | Very low |
| **First AA loading method** | Symmetrical anhydride / DIC | Pre-loaded from vendor | Pre-loaded from vendor | Pre-loaded from vendor | DIEA/DCM direct loading |
| **Cost (relative)** | $ | $$ | $$ | $$$ | $$ |

## Cleavage Conditions by Resin Type

| Resin | Cleavage Cocktail | Time | Temperature | Product |
|-------|-------------------|------|-------------|---------|
| **Wang** | TFA/TIS/H₂O (95:2.5:2.5) | 1.5–2 h | rt | Fully deprotected acid peptide |
| **Rink Amide** | TFA/TIS/H₂O (95:2.5:2.5) | 1.5–2 h | rt | Fully deprotected amide peptide |
| **Rink Acid** | TFA/TIS/H₂O (95:2.5:2.5) | 1.5–2 h | rt | Fully deprotected acid peptide |
| **Sieber (deprotected)** | TFA/TIS/H₂O (95:2.5:2.5) | 1 h | rt | Fully deprotected amide peptide |
| **Sieber (protected)** | TFA/DCM (1–5:99–95) | 5–30 min | rt | Side-chain-protected amide peptide |
| **2-Cl-Trt (deprotected)** | TFA/TIS/H₂O (95:2.5:2.5) | 1–2 h | rt | Fully deprotected acid peptide |
| **2-Cl-Trt (protected)** | AcOH/TFE/DCM (1:1:3) or TFA/DCM (1:99) | 30–60 min | rt | Side-chain-protected acid peptide |

## Resin Selection by Application

| Application | Recommended Resin | Rationale |
|-------------|------------------|-----------|
| **Standard therapeutic peptide (C-term amide)** | Rink Amide | Most common — amide is physiological C-terminus |
| **Standard therapeutic peptide (C-term acid)** | Wang | Simple, low cost, well-characterized |
| **Protected peptide fragment** | 2-Cl-Trt or Sieber | Mild cleavage preserves side-chain PGs |
| **Head-to-tail cyclic peptide** | 2-Cl-Trt | Cleave protected, cyclize in solution |
| **Peptide thioester (NCL)** | 2-Cl-Trt | C-terminal thioester formation |
| **C-terminal modified peptide (ester, amide derivative)** | 2-Cl-Trt | Loading flexibility, mild conditions |
| **Side-chain-protected intermediate** | Sieber | Most acid-labile — best PG retention |
| **Fragment condensation** | Sieber | Protected fragment with C-terminal amide |
| **DKP-prone sequences (Pro-X)** | 2-Cl-Trt | Minimal DKP during second coupling |
| **High-throughput parallel synthesis** | Wang or Rink Amide | Robust, inexpensive, predictable |

## Swelling Behavior and Solvent Compatibility

Resin swelling is critical for reagent access to the growing peptide chain:

| Solvent | Wang | Rink Amide | 2-Cl-Trt | Sieber |
|---------|------|------------|----------|--------|
| **DMF** | 5.0 mL/g | 6.0 mL/g | 6.0 mL/g | 5.0 mL/g |
| **DCM** | 7.0 mL/g | 8.0 mL/g | 9.0 mL/g | 7.0 mL/g |
| **NMP** | 5.5 mL/g | 6.5 mL/g | 6.5 mL/g | 5.5 mL/g |
| **THF** | 6.0 mL/g | 7.0 mL/g | 7.5 mL/g | 6.0 mL/g |
| **MeOH** | 2.0 mL/g | 2.5 mL/g | 2.0 mL/g | 2.0 mL/g |
| **H₂O** | 1.5 mL/g | 2.0 mL/g | 1.5 mL/g | 1.5 mL/g |

**General rule:** Polystyrene-based resins swell well in DMF, DCM, and NMP (the standard SPPS solvents). Poor swelling in MeOH and water means thorough solvent exchange is needed before aqueous steps.

## Loading Considerations

### Choosing Loading Capacity

| Loading | Best For | Trade-offs |
|---------|----------|------------|
| **Low (0.2–0.4 mmol/g)** | Long peptides (>30 AA), difficult sequences | Lower impurity; requires more resin per synthesis |
| **Medium (0.5–0.8 mmol/g)** | Most standard peptides (10–30 AA) | Good balance of yield and purity |
| **High (1.0–1.6 mmol/g)** | Short peptides (<10 AA), high-throughput | Higher risk of aggregation and deletion sequences |

### Loading Measurement

Common methods to determine resin loading:
- **Fmoc release assay:** Treat with 20% piperidine/DMF, measure UV absorbance at 290 or 301 nm (ε = 5250 or 7800 M⁻¹cm⁻¹)
- **Weight gain:** Gravimetric determination after first AA coupling
- **Picric acid test:** For non-Fmoc resins

## Practical Tips

1. **Pre-swell resin** in DCM for 15–30 min before starting synthesis — maximizes access to reactive sites
2. **Do not exceed the recommended loading** — overloading causes aggregation and poor coupling efficiency
3. **Test a small amount of resin** with the cleavage cocktail before performing full cleavage — especially for Sieber or 2-Cl-Trt to confirm protected cleavage conditions are correctly balanced
4. **Store resin at 4 °C** in a desiccator — moisture degrades reactive handles (especially 2-chlorotrityl chloride)
5. **Pre-wash new resin** with DMF (3×) before the first Fmoc removal to remove any loose linker fragments

> **🔗 Related:** [Fmoc Amino Acid Side Chains](./fmoc-amino-acid-side-chains.md) | [Coupling Reagent Comparison](./coupling-reagent-comparison.md) | [Scavenger Selection Guide](./scavenger-selection-guide.md) | [Solvent Purity Guide](./solvent-purity-guide.md)
