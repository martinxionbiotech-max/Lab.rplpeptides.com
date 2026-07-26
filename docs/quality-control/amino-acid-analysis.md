---
description: "Amino acid analysis for peptide composition — hydrolysis, derivatization, HPLC separation, and quantification methods."
---

# Amino Acid Analysis

## Peptide Composition Verification

## Introduction

Amino acid analysis (AAA) is a fundamental identity and composition test for synthetic peptides. The method quantitatively determines the molar ratios of constituent amino acids after complete hydrolysis of the peptide. AAA provides four critical pieces of information: (1) confirmation that the amino acid composition matches the theoretical sequence, (2) detection of unexpected amino acids indicating contamination, (3) verification of the correct molar ratio of each residue (e.g., a peptide with two Leu residues should yield approximately double the molar response of a single Ile residue), and (4) an independent measure of peptide content.

AAA is orthogonal to LC-MS mass confirmation and HPLC purity analysis. While MS confirms that the intact peptide has the correct molecular weight, AAA confirms that every expected amino acid is present in the correct proportions. This combination provides high confidence in the correct primary structure.

## Hydrolysis Methods

| Method | Conditions | Recovery | Strengths | Limitations |
|---|---|---|---|---|
| **Standard HCl hydrolysis** | 6 M HCl, 110 °C, 24 h (vapor or liquid phase) | 90–100% for most stable AAs | Reproducible, well-established, scalable | Trp destroyed; Asn/Gln → Asp/Glu; Cys degraded |
| **Microwave-assisted hydrolysis** | 6 M HCl, 150–165 °C, 15–30 min (in microwave digester) | Comparable to standard in 1/50th time | Rapid turnaround; good for screening | Less uniform bulk heating; specialized equipment |
| **Performic acid oxidation + HCl** | Performic acid (0 °C, 16 h) → then 6 M HCl, 110 °C, 24 h | Cys → cysteic acid (~90%), Met → methionine sulfone | Quantitative Cys and Met determination | Complex protocol; Trp still destroyed |
| **Base hydrolysis** | 4 M NaOH or Ba(OH)₂, 110 °C, 16–24 h | Trp recovered (70–95%) | Required for Trp determination | Asp/Glu/Ser/Thr degraded; metallic contaminant risk |
| **Enzymatic hydrolysis** | Multiple proteases (trypsin, chymotrypsin, pronase) in sequence | Near-native recovery of all AAs | All AAs preserved (including Trp and amides) | Slow (24–48 h); incomplete digestion for some sequences |

**Standard method of choice**: Vapor-phase hydrolysis with 6 M HCl + 0.1% phenol at 110 °C for 24 h. Phenol protects Tyr from halogenation. Norleucine (Nle) is added as an internal standard before hydrolysis.

## Derivatization Methods

After hydrolysis, amino acids are derivatized to enable UV or fluorescence detection:

| Derivatization Reagent | Detection | Sensitivity | Pre- or Post-Column | Stability of Derivative | Compatible with |
|---|---|---|---|---|---|
| OPA (o-phthalaldehyde) | Fluorescence (Ex 340/Em 450) | Low pmol | Pre-column | Moderate (auto-sampler may be needed) | Most AAs except Pro |
| FMOC (9-fluorenylmethoxycarbonyl) | Fluorescence (Ex 260/Em 315) or UV 254 | Sub-pmol | Pre-column | Stable (hours) | All AAs including Pro |
| AQC (6-aminoquinolyl-N-hydroxysuccinimidyl) | Fluorescence (Ex 250/Em 395) | 0.1–1 pmol | Pre-column | Very stable (days) | All AAs |
| Ninhydrin | UV 570 nm (440 nm for Pro) | 100 pmol | Post-column | Immediate | All AAs (classic method) |
| Dabsyl chloride | UV 436 nm | 1–10 pmol | Pre-column | Stable | All AAs |

**Recommended**: AQC (AccQ-Tag, Waters) or OPA/FMOC dual derivatization for maximum sensitivity and sequence coverage.

## Expected Composition Calculation

### Molar Ratio Calculation

For a theoretical peptide sequence, the molar ratio of each amino acid relative to a stable reference (e.g., Ala, Val, or internal standard) is calculated as:

```
Expected Molar Ratio = Number of residues of AA in sequence / Number of residues of reference AA
```

### Example: Peptide AYPGNLAAP (900.1 Da)

| Amino Acid | Expected Residues | Expected Molar Ratio (Ala = 1.0) |
|---|---|---|
| Ala (A) | 2 | 1.00 |
| Pro (P) | 2 | 1.00 |
| Gly (G) | 1 | 0.50 |
| Tyr (Y) | 1 | 0.50 |
| Asn (N) | 1 | 0.50 |
| Leu (L) | 1 | 0.50 |

### Acceptance Criteria for Amino Acid Release Testing

| Parameter | Research Grade | In Vivo/GMP Grade |
|---|---|---|
| Molar ratio tolerance (residues ≥2 in sequence) | ±20% of expected | ±15% of expected |
| Molar ratio tolerance (residues = 1 in sequence) | ±30% of expected | ±20% of expected |
| Total calculated vs. theoretical content recovery | 80–120% | 85–115% |
| Unexpected amino acids | None at >0.1 molar ratio | None at >0.05 molar ratio |
| Internal standard (Nle) recovery | 85–115% | 90–110% |
| Arg/Lys/His ratio to theoretical | ±25% | ±20% |

## Interpretation Guide

All predicted amino acids should be detected at molar ratios close to the expected values. If a particular residue is systematically low (e.g., Ser or Thr at <70% of expected), the peptide may contain a partially resistant bond or the hydrolysis time may be insufficient. Extended hydrolysis with time-point sampling (24, 48, 72 h) can differentiate incomplete hydrolysis from residue degradation.

If an amino acid is absent entirely (e.g., Met missing but predicted), the peptide may have undergone oxidation during hydrolysis. Reduced or absent Trp (destroyed by acid) is expected; its absence does not constitute a failure.

The total protein content calculated from AAA should agree with the peptide content determined by UV spectrophotometry (within ±10%). If the values diverge, investigate the counterion type, water content, and the peptide's extinction coefficient.

## Common Issues

- **Incomplete hydrolysis**: Bonds involving Ile-Ile, Val-Val, or Leu-Val are resistant to acid hydrolysis. Extend hydrolysis time to 48 or 72 h and use time-point extrapolation to infinity for accurate quantitation.
- **Cys/Trp loss**: Cys is destroyed by acid hydrolysis. Use performic acid oxidation (producing cysteic acid) for quantitative Cys analysis. Trp requires basic or enzymatic hydrolysis.
- **Asn/Gln ambiguity**: Asn and Gln are completely deamidated to Asp and Glu during acid hydrolysis. Their presence as amides is inferred from the intact mass data, not from AAA.
- **Salt/counterion interference**: High concentrations of salts (particularly from TFA) can inhibit derivatization. Dialyze or dilute samples prior to analysis.
- **Carryover contamination**: Hydrophobic amino acids (Phe, Leu, Ile) can persist on the HPLC column. Use a wash cycle and blank injection between samples.

> 🔗 Related: [Mass Confirmation](./mass-confirmation.md) | [HPLC Analysis](./hplc-analysis.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
