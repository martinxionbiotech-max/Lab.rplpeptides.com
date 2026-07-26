---
description: "Comparison of UV/PDA, MS, ELSD, and CAD detectors for peptide HPLC — sensitivity, specificity, cost, and application suitability table."
---

# Detector Comparison for Peptide Analysis: UV/PDA, MS, ELSD, and CAD

## Introduction

Detector selection determines what you can see — and what you miss — in peptide analysis. Each detection technology offers a different balance of sensitivity, specificity, quantitation accuracy, and cost. This guide compares the four most common detectors used in peptide HPLC.

## UV / Photodiode Array (PDA) Detection

### How It Works
Peptide bonds absorb UV light strongly at 190–220 nm. Aromatic amino acids (Trp, Tyr, Phe) absorb at 254–280 nm. PDA adds full-spectrum acquisition for peak purity assessment.

### Performance
- **Sensitivity:** 0.1–1 µg on-column (210–220 nm); ~10 ng for peptides with Trp/Tyr
- **Linearity:** Excellent (3–4 orders of magnitude)
- **Specificity:** Moderate — any UV-absorbing species interferes

### Strengths
- Universally applicable — all peptides absorb at low UV
- Reliable, low maintenance, relatively low cost
- Quantitation with external standards is straightforward
- PDA enables peak purity analysis via spectral comparison

### Limitations
- Low specificity — co-eluting impurities with similar chromophores can be missed
- Gradient baseline drift from solvent UV absorption at low wavelengths
- Cannot detect non-UV-absorbing species (some modified peptides, salts)

## Mass Spectrometry (MS) Detection

### How It Works
Peptides are ionized (typically ESI) and detected by mass-to-charge ratio. Single quad (SQ), triple quad (MS/MS), and high-resolution (HRMS) variants are available.

### Performance
- **Sensitivity:** fmol–pmol level; as low as 1–10 ng with SIM
- **Linearity:** 2–3 orders of magnitude (limited by ion suppression)
- **Specificity:** Very high — mass fingerprint uniquely identifies each peptide

### Strengths
- Definitive identification by molecular weight
- MS/MS provides sequence confirmation and fragmentation analysis
- Can identify impurities, truncated sequences, and post-translational modifications
- Compatible with gradient LC without significant baseline issues

### Limitations
- High acquisition and operating cost (especially HRMS)
- Requires experienced operators for method development
- Ion suppression can affect quantitation accuracy
- Not always practical for routine QC (training, maintenance)
- Solvent/additive restrictions (non-volatile buffers unacceptable)

## Evaporative Light Scattering Detection (ELSD)

### How It Works
The column effluent is nebulized into droplets, the solvent evaporates, and non-volatile analyte particles scatter a light beam. Signal is proportional to particle mass.

### Performance
- **Sensitivity:** 1–10 µg on-column (lower than UV)
- **Linearity:** Sigmoidal — log-log transformation needed for quantitation
- **Specificity:** Low — detects any non-volatile solute

### Strengths
- Universal detection — responds to all non-volatile analytes regardless of chromophores
- Gradient-compatible with minimal baseline drift
- Useful for peptides lacking aromatic residues or strong UV absorbance

### Limitations
- Poor sensitivity compared to UV and MS
- Non-linear response complicates quantitation
- Semi-volatile analytes lost during evaporation
- Requires volatile mobile phases (non-volatile buffers unacceptable)

## Charged Aerosol Detection (CAD)

### How It Works
Similar to ELSD but uses a charged aerosol from a corona discharge to charge dried particles, measured by an electrometer. Signal is proportional to particle mass.

### Performance
- **Sensitivity:** 10–100 ng on-column (better than ELSD)
- **Linearity:** ~3 orders of magnitude (log-log), improved by power function fitting
- **Specificity:** Low — detects any non-volatile solute

### Strengths
- Near-universal response that is more consistent than ELSD
- Better sensitivity than ELSD for most analytes
- Less affected by analyte chemical properties (response is particle-mass-based)
- Good for detecting non-UV-absorbing peptides or impurities

### Limitations
- Still less sensitive than UV or MS for most peptide applications
- Requires volatile mobile phases
- Higher cost than ELSD or UV
- Non-destructive? No — sample is destroyed during detection

## Detector Specification and Application Table

| Parameter | UV/PDA | MS (SQ) | MS/MS (Triple Quad) | ELSD | CAD |
|-----------|--------|---------|---------------------|------|-----|
| **Sensitivity (peptide)** | 100 ng | 1–10 ng | 0.1–1 ng | 1–10 µg | 10–100 ng |
| **Linearity range** | 3–4 orders | 2–3 orders | 2–3 orders | 2 orders (log) | 3 orders (log) |
| **Specificity** | Moderate | Very high | Very high | Low | Low |
| **Quantitation accuracy** | Excellent | Good (with ISTD) | Excellent | Moderate | Good |
| **Peptide ID capability** | Spectral matching | Molecular weight | Sequence info | None | None |
| **Mobile phase restrictions** | Low UV cutoff | Volatile only | Volatile only | Volatile only | Volatile only |
| **Capital cost (USD)** | $15K–$40K | $80K–$150K | $200K–$500K | $10K–$25K | $25K–$50K |
| **Operating cost/year** | Low ($500) | Moderate ($5K) | High ($15K) | Low ($1K) | Low ($2K) |
| **Maintenance complexity** | Low | Moderate | High | Low | Low |

## Application Recommendations

| Application | Recommended Detector | Rationale |
|-------------|---------------------|-----------|
| Routine QC purity (main product) | UV/PDA | Workhorse — sensitive, reliable, low cost |
| Impurity profiling (release) | UV/PDA + MS | MS identifies unknown impurities |
| Peptide mapping | PDA + MS/MS | Sequence coverage requires MS/MS |
| Identity confirmation | MS (single quad) | Molecular weight is sufficient |
| Batch comparability | UV/PDA | Quantitative, well-characterized |
| Quantitation high-throughput | UV/PDA | Most linear, robust for validated methods |
| Non-UV-absorbing peptides | CAD or ELSD | Only viable options without MS |
| Pharmacokinetic studies | MS/MS | Required sensitivity in biological matrix |
| Stability-indicating assays | PDA | Peak purity assessment critical |

## Practical Guidance

- **For routine QC:** Start with UV/PDA at 210–220 nm. It is sensitive enough for most peptide assays and by far the most economical option.
- **For method development:** Add MS detection to identify unknown peaks and confirm impurity identity.
- **For GMP release testing:** UV is the quantitation method of choice. A CAD or MS can supplement for non-UV-absorbing impurities.
- **For research:** PDA provides peak purity information that single-wavelength UV cannot — vital during stability studies.

> **🔗 Related:** [Column Selection Guide](./column-selection-guide.md) | [HPLC Method Validation](./hplc-method-validation-instruments.md) | [Solvent Purity Guide](../raw-materials/solvent-purity-guide.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
