---
description: "Acetonitrile (MeCN) — HPLC-grade specifications, UV cutoff, gradient suitability, safety hazards including HCN release under acidic conditions, and proper storage protocols for peptide purification."
---

# Acetonitrile

## HPLC Mobile Phase Solvent for Peptide Purification

## Introduction

Acetonitrile (MeCN, CH₃CN) is the standard organic solvent used as mobile phase B in reversed-phase HPLC for peptide purification and analysis. Its combination of low UV absorbance, moderate eluting strength, excellent peptide solubility, and low viscosity makes it the preferred organic modifier over methanol, ethanol, or 2-propanol for peptide separations. The quality of acetonitrile—particularly its UV transparency, water content, and trace impurity profile—directly determines the sensitivity of peptide detection at 214 nm and the reproducibility of gradient retention times across batches.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | Ethanenitrile |
| **CAS number** | 75-05-8 |
| **Molecular formula** | CH₃CN |
| **Molecular weight** | 41.05 g/mol |
| **Boiling point** | 81.6 °C (at 1 atm) |
| **Melting point** | −45 °C |
| **Density** | 0.782 g/mL (25 °C) |
| **Refractive index** | 1.342 (nD²⁰) |
| **Dielectric constant (ε)** | 37.5 (25 °C) |
| **Dipole moment** | 3.92 D |
| **Viscosity** | 0.34 cP (25 °C) |
| **UV cutoff** | 190 nm |
| **Flash point** | 2 °C (closed cup) — highly flammable |
| **Autoignition temperature** | 524 °C |
| **Vapour pressure** | 89 mmHg (20 °C) |
| **Solubility in water** | Miscible in all proportions |
| **Azeotrope with water** | Acetonitrile/water 83.7:16.3, bp 76.5 °C |

## HPLC Grade Specifications

| Parameter | HPLC Gradient Grade | HPLC Isocratic Grade | LC-MS Grade | ACS Grade |
|-----------|--------------------|---------------------|-------------|-----------|
| **Purity (GC)** | ≥99.9% | ≥99.8% | ≥99.95% | ≥99.5% |
| **Water content (KF)** | ≤0.02% (200 ppm) | ≤0.05% | ≤0.01% | ≤0.1% |
| **UV cutoff** | 190 nm | 190 nm | 189 nm | 192 nm |
| **Absorbance at 200 nm** | ≤0.05 AU | ≤0.10 AU | ≤0.01 AU | — |
| **Absorbance at 210 nm** | ≤0.02 AU | ≤0.05 AU | ≤0.005 AU | ≤0.10 AU |
| **Absorbance at 254 nm** | ≤0.005 AU | ≤0.02 AU | ≤0.001 AU | ≤0.05 AU |
| **Non-volatile residue** | ≤2 ppm | ≤5 ppm | ≤1 ppm | ≤10 ppm |
| **Free acid (as CH₃COOH)** | ≤0.001% | ≤0.005% | — | ≤0.005% |
| **Ammonia (as NH₃)** | ≤1 ppm | ≤2 ppm | — | ≤4 ppm |
| **Typical use** | Gradient HPLC, prep HPLC | Isocratic HPLC | LC-MS | General lab |

**Selection guide:** For preparative HPLC purification of peptides where fractions are collected and lyophilised, HPLC gradient grade is recommended. For analytical HPLC method development and validation, HPLC gradient grade ensures baseline stability across gradients. For LC-MS analysis, use LC-MS grade to minimise background ions in the 50–200 m/z range.

## UV Cutoff and Detection Sensitivity

Acetonitrile has the lowest UV cutoff (190 nm) of all common HPLC organic solvents. This enables peptide detection at 214 nm (peptide bond absorption) with minimal baseline noise and drift:

| Solvent | UV Cutoff (nm) | Relative Absorbance at 214 nm (100% solvent) |
|---------|---------------|---------------------------------------------|
| Acetonitrile | 190 | 0.01 AU |
| Methanol | 205 | 0.15 AU |
| Ethanol | 210 | 0.50 AU |
| 2-Propanol | 210 | 0.35 AU |
| THF | 212 | 0.80 AU |

At 214 nm, 100% acetonitrile produces only ~0.01 AU of background absorbance. This allows full-scale detection of peptide peaks at 0.1–1.0 AUFS (absorbance units full scale) without baseline correction.

## Gradient Suitability

Acetonitrile is uniquely suited for gradient elution in peptide HPLC because of its near-linear relationship between solvent composition and elution strength for most peptides, producing evenly spaced peaks across the gradient. Key considerations:

| Parameter | Recommendation | Rationale |
|-----------|---------------|-----------|
| Initial % B | 5–10% | Adequate for peptide retention on C18 without peak broadening |
| Final % B | 50–60% | Elutes most peptides ≤30 AA; increase to 80% for longer or more hydrophobic peptides |
| Gradient slope | 1–2% B/min | Optimal resolution for complex peptide mixtures |
| Flow rate (analytical) | 1 mL/min (4.6 mm ID) | Standard for 5 µm particle columns |
| Flow rate (preparative) | 10–20 mL/min (20–22 mm ID) | Scale-appropriate for peptide mass load |
| Column temperature | 25–40 °C | Higher temperature reduces backpressure and improves peak shape |
| Re-equilibration time | 5–10 column volumes | Necessary for retention time reproducibility (<0.1 min variation) |

## Safety Hazards

Acetonitrile poses several distinct hazards that require careful laboratory management:

### Acute Toxicity

| Route | Classification | Symptoms | Threshold |
|-------|---------------|----------|-----------|
| Inhalation | H332 (harmful if inhaled) | Headache, dizziness, nausea | 40 ppm (OSHA PEL) |
| Skin absorption | H312 (harmful in contact with skin) | Cyanosis, hypotension | Absorbed through intact skin |
| Ingestion | H302 (harmful if swallowed) | Metabolised to cyanide | ~100 mL fatal dose |
| Eye contact | H319 (causes eye irritation) | Redness, pain | Direct contact |

### Hydrogen Cyanide (HCN) Release

**Critical warning:** Acetonitrile can release hydrogen cyanide gas under specific conditions relevant to peptide chemistry:

| Condition | HCN Risk | Mitigation |
|-----------|----------|------------|
| Strong acid + acetonitrile + water | High (HCN release via hydrolysis) | Never mix acetonitrile with concentrated H₂SO₄ or HNO₃ |
| Basic hydrolysis | Moderate | Avoid NaOH/MeCN mixtures; use in well-ventilated hood |
| UV photolysis | Low | Amber glass containers for long-term storage |
| Thermal decomposition (>200 °C) | High | Never heat acetonitrile above 200 °C in open systems |
| **TFA/acetonitrile mixtures** | **Low risk at room temp** | TFA/H₂O/MeCN at pH 2 does not generate measurable HCN; safe for HPLC use |

The well-known HCN release hazard applies primarily to strong acid digestion or high-temperature conditions, not to standard HPLC conditions (TFA 0.1% at room temperature). Nevertheless, all acetonitrile waste should be labelled and handled as potentially cyanogenic if acidified.

### Flammability

- **Flammability class:** IB (flash point 2 °C)
- **Explosive range in air:** 3.0–17.0% (v/v)
- **Extinguishing media:** Dry chemical, CO₂, alcohol-resistant foam
- **Avoid:** Water jet (spreads burning acetonitrile)

## Storage

| Parameter | Recommendation |
|-----------|---------------|
| Container | Amber glass (protects from UV photolysis) or HDPE for ≤4 L containers |
| Temperature | 15–25 °C; avoid storage near heat sources |
| Inert atmosphere | Nitrogen blanket recommended for multi-litre containers |
| Shelf life (unopened) | >3 years when stored in original sealed container |
| Shelf life (after opening) | 6–12 months; monitor water content and purity by GC |
| Compatibility | Do not store in PVC containers (acetonitrile plasticises PVC) |
| Ventilation | Store in flammable solvent cabinet; never in refrigerators with spark-producing electronics |

## Waste Disposal

- Collect as non-halogenated organic solvent waste
- Incinerate at licensed facility (acetonitrile burns cleanly to CO₂, H₂O, and N₂)
- Do not mix with bleach or hypochlorite (forms toxic chlorinated cyanides)
- Label waste containers as potentially cyanogenic if acetonitrile has been in contact with strong acids

---

> **🔗 Related:** [TFA](./tfa.md) | [Preparative HPLC](../equipment/preparative-hplc.md) | [HPLC Analysis](../quality-control/hplc-analysis.md) | [DMF](./dmf.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
