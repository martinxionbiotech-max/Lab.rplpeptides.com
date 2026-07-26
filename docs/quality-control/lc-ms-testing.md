---
description: "LC-MS testing for peptide identity confirmation — ESI-MS, mass calculation, ionization conditions, and data interpretation."
---

# LC-MS Testing

## Identity Confirmation by Mass Spectrometry

## Introduction

Liquid chromatography–mass spectrometry (LC-MS) is the standard platform for peptide identity confirmation in QC laboratories. The hyphenated technique provides two orthogonal dimensions of information — chromatographic retention time and mass-to-charge (m/z) ratio — allowing simultaneous assessment of purity and identity. For most synthetic peptides, a single LC-MS run can confirm the correct molecular weight, detect common adducts, identify process-related impurities, and assess overall purity by UV at 214 nm.

The LC component is typically a reversed-phase C18 or C8 column using a water–acetonitrile gradient with 0.1% formic acid or TFA. The MS component is most commonly an ESI source coupled to a single quadrupole, triple quadrupole, or time-of-flight (TOF) analyzer.

## Method Parameters Table

| Parameter | Typical Value | Range | Optimization Notes |
|---|---|---|---|
| Column | C18, 2.1 × 50 mm, 1.7 µm | C4, C8, C18; 1.7–5 µm | Longer columns for complex mixtures |
| Mobile phase A | 0.1% formic acid in water | 0.05–0.2% FA or 0.02–0.1% TFA | FA preferred for MS sensitivity |
| Mobile phase B | 0.1% formic acid in acetonitrile | Methanol or ACN; 0.05–0.2% FA | ACN gives sharper peaks |
| Gradient | 5–60% B over 10–20 min | Linear or multi-step | Shallow gradient near expected elution |
| Flow rate | 0.3 mL/min | 0.1–0.6 mL/min | ≤0.4 mL/min for standard ESI |
| Column temp | 40–60 °C | 30–80 °C | Higher temp for larger peptides |
| Injection volume | 1–10 µL | 0.5–50 µL | Maintain <5 µg on column |
| Ionization mode | ESI positive | ESI positive/negative | Positive for most basic peptides; negative for acidic |
| Scan range (m/z) | 300–2000 | 200–4000 | Adjust for peptide size |
| UV detection | 214 nm (or 220, 280 nm) | — | 214 nm for peptide bond |

### ESI Source Optimization

| Parameter | Typical Setting | Effect of Too Low | Effect of Too High |
|---|---|---|---|
| Capillary voltage | 3.0–4.0 kV | Poor ionization | Corona discharge |
| Cone voltage (fragmentor) | 20–40 V | Low signal | In-source fragmentation |
| Source temperature | 120–150 °C | Poor desolvation | Thermal degradation |
| Desolvation temperature | 300–400 °C | Solvent clusters | Excessive (rare) |
| Desolvation gas flow (N₂) | 600–900 L/h | Droplet carryover | Turbulence, signal loss |
| Cone gas flow | 50–150 L/h | Insufficient focusing | Reduced transmission |

## Ionization and Mass-to-Charge (m/z) Relationship

Electrospray ionization produces multiply charged ions of the general form [M + nH]ⁿ⁺ for basic peptides under positive ion mode:

```
m/z = (M + n × 1.0078) / n
```

Where M = molecular weight of the neutral peptide, n = number of charges (proton adducts).

For a peptide of ~1000 Da, the dominant charge state is typically [M+2H]²⁺. For a 5000 Da peptide, [M+5H]⁵⁺ through [M+8H]⁸⁺ are expected. The charge state distribution provides information about the number of basic residues (Lys, Arg, His, and the N-terminal amine).

## Adduct Ion Identification

Adducts are non-covalent associations between the peptide and ions present in the mobile phase or sample matrix. Recognizing adducts prevents misassignment of the target mass:

| Adduct | Mass Added (Da) | m/z Shift (+1 charge) | Common Source | Frequency |
|---|---|---|---|---|
| Na⁺ (sodium) | +21.9819 | +22.0 | Glassware, buffer salts | Common |
| K⁺ (potassium) | +37.9559 | +38.0 | Buffer salts, glassware | Occasional |
| NH₄⁺ (ammonium) | +17.0265 | +17.0 | Ammonium bicarbonate buffers | Occasional |
| TFA (CF₃COO⁻) | +112.9856 | +113.0 | HPLC mobile phase (TFA system) | Very common in TFA systems |
| Acetate (CH₃COO⁻) | +42.0106 | +42.0 | Acetate buffers | Occasional |
| Fe²⁺ | +53.9349 | +54.0 | Metal contamination | Rare |
| Phosphate | +97.9769 | +98.0 | Phosphate buffers | Rare |
| Dimer (2M+H)⁺ | +M | Variable | High concentration | High conc. samples |

### Mass Tolerance Table

| LC-MS Configuration | Mass Tolerance (Da) | Mass Tolerance (ppm at 2000 Da) | Application |
|---|---|---|---|
| Single quadrupole (LC-MS) | ±1.0 Da | ±500 ppm | Routine identity (research) |
| Triple quadrupole (LC-MS/MS) | ±0.5 Da | ±250 ppm | Identity + fragmentation |
| Q-TOF (LC-MS) | ±0.05 Da | ±25 ppm | High-confidence identity |
| Ion trap | ±0.3 Da | ±150 ppm | Identity + MSⁿ |
| Orbitrap | ±0.005 Da | ±2.5 ppm | Characterization-grade |

For routine QC release testing, a mass accuracy of ±1.0 Da on a single quadrupole instrument is generally acceptable for peptides <5000 Da. For higher accuracy requirements (e.g., characterization of clinical material), Q-TOF or higher-resolution instrumentation is recommended.

## Interpretation Guide

A confirmed identity result requires:
1. The deconvoluted mass of the main chromatographic peak matches the theoretical mass within the specified tolerance
2. At least three charge states are observed and yield a consistent deconvoluted mass
3. No unexpected high-abundance masses are present at the retention time of the main peak

### Common Spectral Patterns

| Observation | Interpretation |
|---|---|
| Correct mass + low-abundance [M+Na]⁺ | Normal; verify main peak identity |
| Correct mass + [M+TFA]⁻ present | TFA from mobile phase; acceptable |
| Mass matches, but early-eluting shoulder | Likely D-isomer at low level |
| Mass matches with +16 Da shoulder | Partial Met oxidation during analysis |
| No mass match within ±1 Da for main peak | Identity failure; investigate |
| Expected charge envelope absent | Possible aggregation in solution |

## Common Issues

- **Suppression of ionization**: High concentrations of TFA (>0.05%) in mobile phase suppress ESI signal. Use formic acid or propionic acid instead. Alternatively, use a post-column TFA-fix solution.
- **TFA adduct over-assignment**: In TFA-containing mobile phases, the [M+TFA]⁻ ion is often mistaken for a second component. Confirm by comparing with a formic acid-only system.
- **Split peaks due to cis/trans proline isomerization**: Peptides with multiple Pro residues may show two peaks with identical mass. This is a conformational phenomenon, not an impurity.
- **In-source oxidation**: Met-containing peptides may oxidize during ionization. Reduce source temperature or use a cooled ESI probe.

> 🔗 Related: [LC-MS System](../equipment/lc-ms.md) | [Mass Confirmation](./mass-confirmation.md) | [HPLC Analysis](./hplc-analysis.md) | [What Is a Research Peptide](https://rplpeptides.com/what-is-research-peptide/) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
