---
description: "Peptide content determination methods — UV spectrophotometry, nitrogen analysis, and water content correction."
---

# Peptide Content

## Net Peptide Content Determination

## Introduction

Peptide content, also referred to as net peptide content or peptide mass fraction, is the percentage of the material that is active peptide, after accounting for water, residual solvents, counter-ions, and salts. A batch with 98% HPLC purity may contain only 80% peptide by weight if water and TFA counter-ions constitute the remaining 20%. Accurate content determination is essential for dose calculation, formulation, and batch-to-batch comparability.

Two primary methods are used for peptide content determination: UV spectrophotometry (using the peptide's intrinsic absorption at 280 nm or 214 nm) and amino acid analysis (AAA). Each method has distinct advantages and limitations. The official content value on the certificate of analysis is typically the combination of the content result adjusted for water and residual solvents.

## UV vs. AAA Methods

| Parameter | UV Spectrophotometry | Amino Acid Analysis (AAA) |
|---|---|---|
| Principle | Beer-Lambert law: A = εbc | Quantitative hydrolysis → AA quantitation |
| Sample size | 0.2–1.0 mg (in ~1 mL cuvette) | 0.5–2.0 mg |
| Specificity | Requires knowledge of ε (extinction coefficient) | Composition-specific |
| Counterion included? | No (measures peptide only) | Yes (total peptide + counterion after correction) |
| Water correction needed? | Yes (if measuring powder; not needed if in solution) | Yes (same) |
| Trp: Excellent ε₂₈₀ | Trp (~5500 M⁻¹cm⁻¹), Tyr (~1490 M⁻¹cm⁻¹) | Trp destroyed in acid hydrolysis; must use base hydrolysis |
| Automation | High (plate reader, flow cell) | Moderate (HPLC with derivatization) |
| Turnaround | 5–10 minutes | 1–2 days |
| Precision (RSD) | 1–3% (well-calibrated) | 3–8% |
| Regulatory acceptance | Yes (for identity + content, with ε verified) | Yes (gold standard for content) |

### When to Use Each Method

| Scenario | Recommended Method | Rationale |
|---|---|---|
| Routine QC release (Tyr/Trp-containing peptides) | UV (280 nm) | Fast, requires minimum sample, good precision |
| Peptides lacking Tyr and Trp | AAA or UV at 205/214 nm | Low ε at 280 nm; 205 nm has interference risk |
| Method validation | Both UV + AAA | Cross-validates; AAA provides reference |
| Content discrepancy investigation | AAA | Composition-based; less susceptible to counterion artifacts |
| GMP/clinical material release | AAA (primary) + UV (confirmatory) | Regulatory expectation; orthogonal methods |

## Water/Salt/Counterion Correction

Peptide content = 100% − (water % + residual solvent % + counterion % + inert excipient %)

### Typical Component Distribution for TFA-Salt Peptides

| Component | Research Grade (%) | GMP Grade (%) | Notes |
|---|---|---|---|
| **Net peptide (active)** | 75–85 | 80–90 | Corrected for all non-peptide components |
| **TFA counter-ion** | 8–15 | 5–12 | Proportional to basic residue content (Lys, Arg, His) |
| **Water** | 2–5 | 1–3 | Measured by Karl Fischer |
| **Residual solvents** | ≤0.5 | ≤0.5 | Measured by HS-GC (ICH Q3C) |
| **Inert excipients** | Variable | Variable | Mannitol, sucrose, etc. (formulation-dependent) |
| **Acetate counter-ion** | 2–8 (if acetate form) | 2–5 (if acetate form) | Alternative to TFA |

### Counter-Ion Mass Contribution

The mass contribution of TFA counter-ions depends on the number of basic residues and the N-terminal free amine:

```
Counterion content (%) = [n × M_TFA / (M_peptide_free_base)] × (1 − Water% − Solvent%) × 100
```

Where n = number of basic residues (Lys, Arg, His) + N-terminal NH₂, M_TFA = 113.02 Da (TFA⁻), and M_peptide_free_base is the free base (uncharged) molecular weight.

For a peptide with 5 basic residues and a free base MW of 2500 Da, the theoretical TFA content is approximately 5 × 113.02 / 2500 × (1 − 0.03) × 100 ≈ 21.9%. Actual TFA content is measured by ion chromatography or ion-selective electrode and compared to the theoretical value.

## Peptide Content Calculation Formulas

| Formula | Purpose | Example |
|---|---|---|
| **Net peptide (UV)** = (A₂₈₀ × DF) / (ε₂₈₀ × b) × Mw | Content by UV | A₂₈₀ = 0.45, DF = 100, ε = 5500 M⁻¹cm⁻¹, b = 1 cm, Mw = 3000 → 0.45×100/(5500×1)×3000 = 24.5 mg → content = 24.5/25.0 = 98% |
| **Net peptide (corrected)** = (100 − Water% − Solvent% − Counterion%) | Corrected content | 100 − 3% − 0.2% − 12% = 84.8% w/w |
| **Peptide content (AAA)** = (Σ AA mass recovered / Sample mass) × (Mw peptide / Σ AA MW) | Content by AAA | Recovered AA mass = 18.5 mg, sample mass = 22.0 mg, Mw ratio = 1.02 → content = 18.5/22.0 × 1.02 × 100 = 85.8% |
| **Accounting check** | Verify sum | Peptide (84.8%) + Water (3.0%) + Solvents (0.2%) + TFA (12.0%) = 100% |

## Acceptance Criteria

| Product Grade | UV Content (w/w) | Corrected Content (w/w) | Water Limit | Residual Solvents |
|---|---|---|---|---|
| Research peptide | Report ≥70% | ≥80% | ≤5% | Report |
| In vivo / preclinical | ≥75% | ≥80% | ≤3% | ≤0.5% |
| GMP (clinical) | ≥80% | ≥85% | ≤2% | ≤0.5% |
| GMP (commercial) | ≥80% | ≥85% | ≤2% | ≤0.2% |

## Interpretation Guide

A corrected peptide content of 84.8% (as above) is typical for a trifluoroacetate salt peptide with moderate water content. If the TFA content by ion chromatography (e.g., 18.5%) significantly exceeds the theoretical TFA content (12%), the excess may indicate residual TFA from cleavage — investigate the lyophilization cycle or wash steps.

If UV and AAA content values disagree by more than 10%, investigate:
- Extinction coefficient error (are Tyr/Trp content correct?)
- UV measurement interference (absorbance from counterion, excipient, or buffer)
- AAA hydrolysis recovery (was internal standard recovery within 85–115%? Were Ser/Thr/VaI/Ile values extrapolated from time points?)

## Common Issues

- **Extinction coefficient uncertainty**: For peptides with no Trp or Tyr, use the 214 nm extinction coefficient (estimated as ~1000 M⁻¹cm⁻¹ per peptide bond), or use the biuret/BCA method. For novel sequences, determine ε experimentally by AAA correlation.
- **Hygroscopic powder**: Weighing variability due to moisture uptake is a principal source of content variability. Condition samples in a desiccator over P₂O₅ for 4 h prior to weighing.
- **Incomplete drying during KF**: If KF extraction time is insufficient, water will be under-estimated, inflating the peptide content value. Verify with a water reference standard.

> 🔗 Related: [Water Content](./water-content.md) | [Residual Solvents](./residual-solvents.md) | [COA Understanding](./coa-understanding.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
