---
description: "Guide to solvent grades for peptide synthesis — HPLC grade, anhydrous, peptide synthesis grade — including water content thresholds, specification tables, and use-case recommendations."
---

# Solvent Purity Guide for Peptide Synthesis

## Introduction

Solvent quality is one of the most underappreciated variables in peptide synthesis. Water content, stabilizers, trace metals, and organic impurities in "off-grade" solvents cause failed couplings, side reactions, and irreproducible HPLC results. This guide explains the solvent grades relevant to peptide synthesis and provides specifications for selecting the appropriate grade for each application.

## Solvent Grades Overview

| Grade | Typical Purity | Water Content | Key Specifications | Cost Index |
|-------|---------------|---------------|-------------------|------------|
| **HPLC Grade** | ≥99.9% | ≤0.05% (500 ppm) | UV cutoff, non-volatile residue | 1× (baseline) |
| **HPLC Plus / Gradient** | ≥99.9% | ≤0.02% (200 ppm) | Lower UV absorbance, degassed | 1.5× |
| **Anhydrous (Sure/Seal)** | ≥99.8% | ≤0.005% (50 ppm) or less | Molecular sieve dried; septum-sealed | 3–5× |
| **Peptide Synthesis Grade** | ≥99.9% | ≤0.01% (100 ppm) | Low amine content, low metal content | 2–3× |
| **ACS Reagent Grade** | ≥99.5% | ≤0.1% (1000 ppm) | General laboratory grade | 0.7× |
| **Technical Grade** | ≥95% | Variable | Industrial use only | 0.3× |

## Water Content Specifications by Solvent

| Solvent | HPLC Grade (%H₂O) | Anhydrous (%H₂O) | Peptide Synthesis Grade (%H₂O) | Impact of Excessive H₂O |
|---------|------------------|-------------------|-------------------------------|------------------------|
| **DMF** | ≤0.05% | ≤0.005% | ≤0.01% | Hydrolyzes activated amino acids; reduces coupling efficiency |
| **DCM** | ≤0.02% | ≤0.001% | ≤0.005% | Hydrolyzes acid chlorides; poor SPPS results |
| **NMP** | ≤0.05% | ≤0.005% | ≤0.01% | Similar to DMF — coupling efficiency drops |
| **ACN** | ≤0.02% | ≤0.003% | ≤0.01% | Gradient reproducibility issues in HPLC |
| **MeOH** | ≤0.05% | ≤0.005% | ≤0.02% | Competing ester formation in some reactions |
| **TFA** | N/A (acid) | ≤0.01% | ≤0.01% | Variable cleavage efficiency; side reactions |
| **THF** | ≤0.05% | ≤0.005% | ≤0.02% | Peroxide formation accelerated by moisture |
| **IPA** | ≤0.05% | ≤0.005% | ≤0.02% | Minor — used mainly for washing |

## Grade Specifications and Use Cases

### N,N-Dimethylformamide (DMF)

DMF is the primary solvent for Fmoc SPPS — it is used in every coupling and deprotection step.

| Specification | HPLC Grade | Peptide Synthesis Grade | Why It Matters |
|--------------|-----------|------------------------|----------------|
| **Assay** | ≥99.9% | ≥99.9% | Baseline |
| **Water** | ≤0.05% | ≤0.01% | Water competes with amine for activated ester |
| **Free amine (as dimethylamine)** | ≤5 ppm | ≤2 ppm | Amines prematurely remove Fmoc groups |
| **UV (at 275 nm)** | ≤0.05 AU | ≤0.03 AU | Indicates general purity |
| **Non-volatile residue** | ≤5 ppm | ≤3 ppm | Contaminants that embed in resin |

**Recommendation:** Use peptide synthesis grade DMF for SPPS. At minimum, use HPLC grade. Never use ACS or technical grade.

### Dichloromethane (DCM)

DCM is used for resin washing, some coupling steps, and as a carrier for TFA in cleavage cocktails.

| Specification | HPLC Grade | Anhydrous | Why It Matters |
|--------------|-----------|-----------|----------------|
| **Assay** | ≥99.9% | ≥99.8% | Baseline |
| **Water** | ≤0.02% | ≤0.001% | Water hydrolyzes acid chlorides and activated esters |
| **Stabilizer (amylene)** | 50–150 ppm | None or 50 ppm | Stabilizer can interfere in NMR; may be removed |
| **Non-volatile residue** | ≤5 ppm | ≤10 ppm | — |

**Recommendation:** Anhydrous DCM from a Sure/Seal bottle for reactions. HPLC grade DCM is acceptable for washing. Do not use unstabilized DCM for long-term storage.

### Acetonitrile (ACN) for HPLC

ACN is the primary organic modifier in RP-HPLC peptide purification.

| Specification | HPLC Gradient | HPLC Isocratic | Why It Matters |
|--------------|--------------|----------------|----------------|
| **Assay** | ≥99.9% | ≥99.9% | Baseline |
| **Water** | ≤0.02% | ≤0.05% | UV baseline drift |
| **UV cutoff** | 190 nm | 195 nm | Low-UV peptide detection (210 nm) |
| **UV absorbance at 210 nm** | ≤0.05 AU | ≤0.10 AU | Baseline stability for peptide quantification |
| **Non-volatile residue** | ≤2 ppm | ≤5 ppm | Ghost peaks |

**Recommendation:** Use HPLC gradient grade ACN for any method with peptide detection below 220 nm. Isocratic grade is acceptable for preparative purification.

### Trifluoroacetic Acid (TFA)

TFA is the primary acid used in cleavage cocktails and HPLC mobile phases.

| Specification | HPLC Grade | Peptide Synthesis Grade | Why It Matters |
|--------------|-----------|------------------------|----------------|
| **Assay** | ≥99.0% | ≥99.5% | — |
| **Water** | ≤0.05% | ≤0.01% | Hydrolysis of protecting groups during cleavage |
| **Chloride** | ≤10 ppm | ≤5 ppm | Corrosion of stainless steel HPLC components |
| **Sulfate** | ≤0.01% | ≤0.005% | Non-volatile residue |
| **Non-volatile residue** | ≤0.01% | ≤0.005% | Contaminates cleaved peptide |

**Recommendation:** Peptide synthesis grade TFA for cleavage cocktails. HPLC grade is acceptable for HPLC mobile phases (0.05–0.1% TFA in water).

## Solvent Grade × Use Case Matrix

| Application | Recommended Grade | Minimum Acceptable Grade | Why |
|-------------|------------------|------------------------|-----|
| **Fmoc SPPS (coupling, deprotection)** | Peptide synthesis grade DMF | HPLC grade DMF (anhydrous) | Water and amines ruin activation |
| **Resin washing** | HPLC grade | ACS grade (with caution) | Residual DMF/DCM removed by washing |
| **Coupling (DCM-based)** | Anhydrous DCM | HPLC grade DCM (dried over molecular sieves) | Water competes for activated ester |
| **HPLC purification (analytical)** | HPLC gradient grade ACN | HPLC grade ACN | UV baseline stability critical |
| **HPLC purification (preparative)** | HPLC grade ACN | Technical grade (filtered and distilled) | Preparative tolerates slightly lower purity |
| **Cleavage cocktail** | Peptide synthesis grade TFA | HPLC grade TFA | Water content affects side-chain deprotection |
| **Ether precipitation** | HPLC grade MTBE or Et₂O | ACS grade | Impurities co-precipitate with peptide |
| **MALDI-TOF sample prep** | HPLC grade ACN and TFA | — | Spectral quality depends on purity |
| **NMR sample** | Anhydrous (deuterated) solvents | — | Water peak interferes with spectra |
| **LC-MS** | HPLC gradient grade solvents | HPLC grade | MS-compatible purity required |

## Water Content Thresholds for SPPS

Water in the coupling step is the most common cause of reduced yield:

| Water Level in DMF | Effect on Coupling Efficiency |
|-------------------|-------------------------------|
| **<50 ppm** | Optimal — full coupling in 5–15 min |
| **50–100 ppm** | Minimal impact — >95% coupling |
| **100–500 ppm** | Noticeable reduction — coupling drops to 85–95% |
| **500–1000 ppm** | Significant — 70–85% coupling; double coupling needed |
| **>1000 ppm** | Severe — <70% coupling; hydrolysis of activated ester dominant |

**Rule of thumb:** For each 100 ppm of water in DMF, ~2–5% of the activated amino acid is hydrolyzed before it can couple.

## Stabilizers and Preservatives

| Solvent | Common Stabilizer | Impact on Peptide Synthesis |
|---------|-----------------|----------------------------|
| **DCM** | Amylene (2-methyl-2-butene) | Generally inert; can be removed by distillation |
| **CHCl₃** | Ethanol (0.5–1%) | Ethanol can transesterify; use amylene-stabilized |
| **THF** | BHT (2,6-di-tert-butyl-4-methylphenol) or 0.025% BHT | BHT can appear as impurity in LC-MS |
| **Et₂O** | BHT or no stabilizer | BHT does not precipitate with peptide |
| **Dioxane** | BHT | Remove before use for sensitive chemistry |

## Practical Recommendations

1. **Dedicated peptide-grade DMF** should be purchased specifically for SPPS and stored under N₂
2. **Do not use "old" DMF** — DMF slowly degrades to dimethylamine and CO, even in sealed containers
3. **Dry solvents in-house** if needed: molecular sieves (3 Å or 4 Å) are effective for DMF, DCM, and ACN
4. **Test water content** by Karl Fischer titration — especially important for DMF and DCM used in SPPS
5. **Filter HPLC solvents** through 0.2 µm PTFE filters before use to remove particulate matter
6. **Use fresh TFA** for cleavage cocktails — old TFA accumulates water from the atmosphere
7. **Never store DMF in clear glass** — light accelerates degradation; use amber bottles

> **🔗 Related:** [Fmoc Amino Acid Side Chains](./fmoc-amino-acid-side-chains.md) | [Resin Comparison Guide](./resin-comparison-guide.md) | [Coupling Reagent Comparison](./coupling-reagent-comparison.md) | [Scavenger Selection Guide](./scavenger-selection-guide.md) | [Column Selection Guide](../equipment/column-selection-guide.md)
