---
description: "LC-MS system specifications — mass analyzer types, ionization sources, mass range, resolution, and sensitivity for peptide analysis."
---
# LC-MS System

## Liquid Chromatography-Mass Spectrometry

## Category
Analysis Equipment

## Application
Identity confirmation and purity assessment

## Function
Combines HPLC separation with mass detection for molecular weight confirmation of peptide peaks.

---

## Introduction

Liquid chromatography-mass spectrometry (LC-MS) is the primary analytical tool for peptide characterization in both research and GMP manufacturing environments. It performs two essential functions: separating peptide components by reversed-phase HPLC and confirming their identity by measuring the mass-to-charge ratio (m/z) of the eluting species. For peptide QC, LC-MS is used to confirm molecular weight against the theoretical value, detect deletion sequences and incomplete deprotection byproducts, identify common adducts (Na⁺, K⁺, TFA), and monitor batch-to-batch consistency. The selection of ionization method and mass analyzer type determines the instrument's capabilities for different peptide mass ranges and application requirements.

## Ionization Methods: ESI vs. MALDI

| Parameter | Electrospray Ionization (ESI) | Matrix-Assisted Laser Desorption/Ionization (MALDI) |
|-----------|------------------------------|------------------------------------------------------|
| Ionization mechanism | Electrospray droplet desolvation | Laser ablation from crystalline matrix |
| Charge state | Multiple (z = 2–6 common for peptides) | Predominantly singly charged (z = 1) |
| Mass range | Up to 5000 m/z (extended) | Up to 500,000 Da (linear mode) |
| Compatible with LC | Yes — online coupling standard | No — offline spotting required |
| Sample preparation | Minimal — direct injection | Matrix spotting required |
| Salt tolerance | Low — salts suppress ionization | Moderate |
| Mass accuracy | 1–5 ppm (with calibration) | 50–200 ppm (linear), 5–20 ppm (reflector) |
| Quantitative capability | Excellent (MRM mode) | Limited |
| Fragment ion generation | MS/MS via CID or HCD | Post-source decay (PSD) or LIFT |
| Primary peptide use | Identity confirmation, purity, quantitation | Intact mass screening, large peptides |

For routine peptide QC, **ESI is the overwhelming standard** because it couples directly to HPLC, generates multiple charge states that aid in mass determination, and supports MS/MS fragmentation for sequence confirmation. MALDI is used selectively for screening very large peptides or proteins where the single-charge spectrum simplifies interpretation.

## Mass Analyzer Types and Performance

| Analyzer Type | Resolution (FWHM) | Mass Accuracy | Scan Speed | m/z Range | Typical Application |
|--------------|-------------------|---------------|------------|-----------|-------------------|
| Single quadrupole (Q) | ~1,000 (unit) | ±0.5 Da | Fast | 10–3000 | Routine molecular weight confirmation |
| Triple quadrupole (QqQ) | ~1,000 (unit) | ±0.3 Da | Fast | 10–3000 | Quantitative analysis (MRM) |
| Quadrupole-TOF (Q-TOF) | 20,000–40,000 | <5 ppm | Fast | 50–20,000 | High-resolution peptide mapping |
| Time-of-flight (TOF) | 15,000–25,000 | <5 ppm | Very fast | up to 500,000 | Intact mass, large peptides |
| Orbitrap (FTMS) | 60,000–240,000 | <1 ppm | Moderate | 50–6000 | High-resolution, PTM analysis |
| Ion trap (IT) | ~1,000 (unit) | ±0.5 Da | Fast | 50–4000 | MSⁿ fragmentation |

For standard peptide manufacturing QC, a **single quadrupole or triple quadrupole LC-MS** provides adequate resolution (unit resolution) and mass accuracy (±0.5 Da) to confirm peptide identity, detect deletion sequences, and quantify purity. **Q-TOF instruments** are increasingly used for comprehensive peptide characterization and impurity profiling in GMP environments, where the higher resolution enables separation of closely related mass species.

## Resolution and Detection Specifications

| Specification | Standard QC LC-MS | High-Resolution LC-MS |
|--------------|------------------|----------------------|
| Resolution (FWHM) | 1,000–2,000 | 20,000–240,000 |
| Mass accuracy | ±0.5 Da | <5 ppm (<0.02 Da at 4000 Da) |
| Detection limit (peptide) | 0.1–1.0 ng on column | 10–100 pg on column |
| Linear dynamic range | 10³–10⁴ | 10⁴–10⁵ |
| Scan rate | 5–10 Hz | 10–30 Hz |
| Spectral acquisition | Full scan, SIM, MRM | Full scan, MS/MS |
| Deconvolution algorithm | MaxEnt or similar | MaxEnt, Xtract, Autospec |
| Result confidence | Identity confirmed (±1 Da) | Identity confirmed + sequence coverage |

The difference between standard and high-resolution LC-MS is most apparent when analyzing complex peptide mixtures (e.g., crude peptide before purification), where unit-resolution instruments may fail to resolve co-eluting species with similar masses. For release testing of purified peptides at ≥98% purity, a standard LC-MS is often sufficient.

## Detection Limits and Peptide Mass Ranges

| Peptide MW Range | Detection Mode | LC-MS Type | Limit of Detection | Typical Applications |
|-----------------|---------------|-----------|-------------------|---------------------|
| <1,000 Da | Full scan (100–2000 m/z) | Any Q or Q-TOF | 0.1–1.0 ng | Dipeptides, short fragments |
| 1,000–5,000 Da | Full scan (200–2500 m/z) | Standard Q or Q-TOF | 0.1–1.0 ng | Most synthetic therapeutic peptides |
| 5,000–10,000 Da | Full scan extended range | Q-TOF or TOF | 1–10 ng | Long linear peptides, some proprietary sequences |
| 10,000–50,000 Da | Deconvolution required | Q-TOF or TOF | 10–100 ng | Peptide–protein conjugates |
| >50,000 Da | MALDI-TOF preferred | MALDI-TOF | 1–50 pmol | Fusion peptides, protein fragments |

**Practical sensitivity for peptide QC:** Most commercial synthetic peptides (1,000–5,000 Da) are easily detected at 0.1–1.0 ng on column using a standard ESI-quadrupole LC-MS system. For longer peptides (>5,000 Da), the decrease in ionization efficiency and shift to higher charge states reduces detection sensitivity, making high-resolution TOF-based systems advantageous.

## Common Peptide Adducts and Artifact Identification

| Adduct Type | Mass Shift | Frequency | Cause | Notes |
|------------|-----------|-----------|-------|-------|
| [M+H]⁺ | +1.0078 Da | Always present | Protonation | The expected molecular ion |
| [M+Na]⁺ | +22.9893 Da | Common | Sodium from glassware, buffers | Indicates poor desalting |
| [M+K]⁺ | +38.9637 Da | Occasional | Potassium contamination | Reduce with desalting |
| [M+TFA+H]⁺ | +113.9387 Da | Very common | Trifluoroacetate counterion | Characteristic of TFA-salt peptides |
| [M+H+NH₃]⁺ | +18.0338 Da | Occasional | Ammonium adducts | From ammonium bicarbonate buffers |
| [M+ACN+H]⁺ | +41.0265 Da | Common in ESI | Acetonitrile (mobile phase) | Frequently observed, not a contaminant |
| +16 Da | +15.9949 Da | Common | Oxidation (Met, Cys, Trp) | Quality indicator — track by MS |
| +44 Da | +42.0106 Da | Occasional | Acetylation | May indicate incomplete capping removal |
| -18 Da | -18.0106 Da | Occasional | Dehydration of Ser/Thr | Heating artifact |

## Key Takeaways

- **Ionization:** ESI is the standard for routine peptide LC-MS, providing online LC coupling and multiple charge states for accurate mass determination. MALDI is used selectively for large peptides and rapid screening.
- **Mass Analyzer Selection:** Single quadrupole instruments suffice for routine identity confirmation (±0.5 Da). High-resolution Q-TOF or Orbitrap instruments are needed for complex impurity profiling and comprehensive sequence characterization.
- **Mass Range Coverage:** Standard LC-MS systems cover the 1,000–5,000 Da range that encompasses most therapeutic synthetic peptides. Longer peptides (>5,000 Da) require Q-TOF or TOF instruments with extended mass ranges.
- **Detection Limits:** 0.1–1.0 ng on column is achievable for standard peptides. Sensitivity decreases for larger, less efficiently ionized sequences.
- **Adduct Awareness:** Na⁺, K⁺, and TFA adducts are the most common non-peptide signals. Monitoring the +16 Da oxidation shift provides a valuable quality indicator for peptides containing susceptible residues.

> 🔗 Related: [Mass Spectrometer](./mass-spectrometer.md) | [LC-MS Testing](../quality-control/lc-ms-testing.md) | [Mass Confirmation](../quality-control/mass-confirmation.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/)
