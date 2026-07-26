---
description: "Mass confirmation by mass spectrometry — molecular weight verification and acceptance criteria for peptide identity."
---

# Mass Confirmation

## Molecular Weight Verification

## Introduction

Mass confirmation is the primary identity test for synthetic peptides. The experimentally determined molecular weight is compared against the theoretical monoisotopic or average mass calculated from the amino acid sequence. A mass match within the defined acceptance window provides high-confidence confirmation of the correct primary structure, including the intended sequence length, post-translational modifications, and disulfide bridging pattern.

Mass confirmation is performed using electrospray ionization mass spectrometry (ESI-MS) coupled with liquid chromatography (LC-MS) or, for simpler peptides, by direct infusion. Time-of-flight (TOF) and quadrupole (Q) mass analyzers provide sufficient mass accuracy for routine QC. Orbitrap and FT-ICR instruments are reserved for high-resolution characterization where sub-ppm mass accuracy is required.

## Exact Mass vs. Average Mass

Two mass values are calculated for each peptide sequence, and the choice between them depends on the resolution of the mass spectrometer:

| Mass Type | Definition | When to Use | Example (Substance P, 1347.74 Da) |
|---|---|---|---|
| **Monoisotopic mass** | Mass calculated using the most abundant isotope of each element (¹²C, ¹H, ¹⁴N, ¹⁶O, ³²S) | High-resolution MS (TOF, Orbitrap) | 1347.7354 Da |
| **Average mass** | Mass calculated using the weighted average isotopic mass of each element | Low-resolution MS (quadrupole, ion trap) | 1348.63 Da |

For peptides <2000 Da, the monoisotopic mass is readily observable and preferred for identity confirmation. For peptides >4000 Da, the monoisotopic peak may be too low in relative abundance, and the average mass is used instead. The difference between monoisotopic and average mass is approximately 0.6 Da per 1000 Da of molecular weight.

## Mass Accuracy Requirements

| Mass Analyzer | Typical Resolution (FWHM) | Mass Accuracy (ppm) | Mass Accuracy (Da at 3000 Da) | Suitability |
|---|---|---|---|---|
| Quadrupole (single or triple) | 1,000–4,000 | 100–500 ppm | ±0.3–1.5 Da | Routine identity confirmation |
| Time-of-flight (TOF) | 10,000–40,000 | 5–20 ppm | ±0.015–0.06 Da | High-confidence confirmation |
| Q-TOF | 10,000–40,000 | 3–10 ppm | ±0.009–0.03 Da | Characterization-grade |
| Orbitrap | 60,000–240,000 | <3 ppm | ±0.009 Da | Molecular formula assignment |
| FT-ICR | >500,000 | <1 ppm | ±0.003 Da | Highest accuracy; research only |

### Acceptance Criteria

| Application | Mass Accuracy Requirement | Deconvolution Method | Acceptance Window |
|---|---|---|---|
| Research peptide | ≤±1.0 Da | Average mass (MaxEnt, standard) | ±1.0 Da (or ±500 ppm) |
| In vivo / preclinical | ≤±0.5 Da | Monoisotopic mass (TOF) | ±0.5 Da (or ±200 ppm) |
| GMP (clinical/commercial) | ≤±0.3 Da | Monoisotopic (TOF or higher) | ±0.3 Da (or ±100 ppm) |
| Characterization / method validation | ≤±0.1 Da | Monoisotopic (Orbitrap or Q-TOF) | ±0.1 Da (or ±10 ppm) |

## Deconvolution Software Comparison

Software for charge-state deconvolution converts the m/z spectrum into a zero-charge (neutral) mass spectrum:

| Software | Algorithm | Strengths | Limitations | Typical Use Case |
|---|---|---|---|---|
| MaxEnt 1 (Waters) | Maximum entropy | Robust for complex spectra; handles overlapping charge states | Requires manual parameter tuning | Routine LC-MS identity |
| BioPharmaView (Agilent) | Bayesian protein reconstruction | Integrated with MassHunter; good for intact analysis | Vendor-specific | Intact mass confirmation |
| MagTran | Zscore algorithm | Fast for simple spectra; freeware | Struggles with adducts | Quick checks |
| UniDec | Bayesian deconvolution | Excellent for multi-component mixtures | Computationally intensive | Complex mixtures / intact mass |
| Protein Deconvolution (Thermo) | ReSpect / AutoSpect algorithm | Integrated with Xcalibur; automated | Requires Xcalibur license | GMP environments |

### Deconvolution Acceptance Criteria

| Parameter | Requirement |
|---|---|
| Number of charge states used for deconvolution | ≥3 |
| R² of charge state linear fit | ≥0.999 |
| Mass accuracy match to theoretical | Per table above |
| Adduct peaks (Na⁺, K⁺, TFA) | Identified; not mistaken for target |

## Report Format and Interpretation

| Parameter | Result | Pass/Fail |
|---|---|---|
| Sequence (theoretical) | H-Tyr-Gly-Gly-Phe-Met-Gly-Met-NH₂ | — |
| Theoretical monoisotopic mass | 762.3025 Da | — |
| Found mass (deconvoluted) | 762.2981 Da | — |
| Mass error | −0.0044 Da (−5.8 ppm) | ✅ Pass |
| Charge states observed | [M+H]⁺, [M+Na]⁺, [M+2H]²⁺, [M+3H]³⁺ | ✅ Pass |
| Adduct notes | [M+Na]⁺ at 784.28 Da (minor) | Acceptable |
| Identity | Confirmed | ✅ Pass |

### Interpreting Mass Discrepancies

| Observed Mass Difference (Δm) | Likely Cause | Recommended Action |
|---|---|---|
| Δm ≈ ±1 Da (not ±1 Da exactly) | Deletion or insertion sequence | Check synthesis history; re-purify |
| Δm ≈ ±18 Da | Water loss (dehydration) or gain (hydrolysis) | Check for Asp dehydration or backbone hydrolysis |
| Δm ≈ ±16 Da | Oxidation (Met→sulfoxide) or reduction | Re-purify under inert atmosphere |
| Δm ≈ +22 Da or +38 Da | Na⁺ or K⁺ adduct | Acceptable; confirm main peak is correct |
| Δm ≈ +113 Da | TFA adduct (CF₃COO⁻) | Common in TFA-salts; confirm identity |
| Δm ≈ +44 Da | Acetate adduct | Verify counterion |
| Δm ≈ +42 Da | Acetylation | Incomplete deprotection |

## Common Issues

- **In-source fragmentation**: Labile peptides (e.g., those containing Asp-Pro bonds) may fragment in the ion source, producing artifact peaks. Reduce cone voltage or source temperature.
- **Incomplete deconvolution**: Peptides >5000 Da or those with extensive adduction require optimized deconvolution parameters.
- **Multi-component mass spectra**: Co-eluting impurities produce multiple deconvoluted masses. Use LC-MS rather than direct infusion to separate components before mass measurement.

> 🔗 Related: [LC-MS Testing](./lc-ms-testing.md) | [LC-MS System](../equipment/lc-ms.md) | [COA Understanding](./coa-understanding.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
