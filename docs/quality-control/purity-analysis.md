---
description: "Peptide purity analysis by HPLC — area percent calculation, impurity profiling, and acceptance criteria for research and GMP grades."
---

# Purity Analysis

## HPLC Purity and Impurity Profiling

## Introduction

Purity analysis by reversed-phase HPLC (RP-HPLC) with UV detection at 214 nm is the primary method for quantifying peptide purity. The 214 nm wavelength corresponds to the absorption maximum of the peptide bond, providing a uniform response factor across different peptide sequences. Purity values derived from HPLC are reported as area percent — the integrated area of the main peak divided by the total area of all peaks in the chromatogram.

It is critical to distinguish between **area percent** (HPLC purity) and **weight percent** (absolute peptide content). Area percent reflects the relative abundance of the peptide species among all UV-absorbing components, whereas weight percent accounts for water, residual solvents, and counter-ions. A peptide may appear ≥98% pure by HPLC area yet contain only 80% peptide by weight. Both metrics are reported on the certificate of analysis.

## HPLC Purity Calculation

Purity by HPLC area percent is calculated as:

```
Purity (%) = (A_main / Σ A_all) × 100
```

Where:
- A_main = integrated area of the principal peptide peak
- Σ A_all = sum of integrated areas of all peaks (excluding void volume, system peaks, and solvent front)

### System Suitability Requirements

| Parameter | Requirement |
|---|---|
| Theoretical plates (main peak) | ≥5000 |
| Tailing factor | 0.8–1.8 |
| Resolution (main peak from nearest impurity) | ≥1.5 |
| RSD of retention time (5 replicate injections) | ≤1.0% |
| RSD of peak area (5 replicate injections) | ≤2.0% |
| Signal-to-noise (0.1% impurity standard) | ≥10:1 |
| Blank injection | No interfering peaks |

## Impurity Profiling and Thresholds

Individual impurities are reported when their peak area exceeds the reporting threshold. The following thresholds align with ICH Q3A/Q3B guidance adapted for peptide drug substances:

| Purity Range | Report Threshold | Identify Threshold | Qualify Threshold |
|---|---|---|---|
| ≥98% | ≥0.05% | ≥0.10% | ≥0.15% |
| 95–98% | ≥0.10% | ≥0.15% | ≥0.20% |
| <95% | ≥0.15% | ≥0.25% | ≥0.50% |

### Routine Impurity Categories

| Impurity Type | Typical RT Relative to Main Peak | Common Level (%) | Origin |
|---|---|---|---|
| Deletion sequences | 0.70–0.95 (earlier) | 0.05–2.0 | Incomplete coupling during SPPS |
| Truncated peptides | 0.65–0.90 (earlier) | 0.02–1.0 | Failed deprotection |
| D-isomers | 0.95–1.05 (shoulder) | 0.1–5.0 | Racemization during coupling |
| Oxidation products | 0.80–0.95 (earlier) | 0.05–0.5 | Met or Trp air oxidation |
| Dimer/aggregates | 1.05–1.30 (later) | 0.1–2.0 | Post-cleavage assembly |
| Scavenger residues | 0.30–0.60 (early) | 0.02–0.5 | Cleavage cocktail carryover |

## Acceptance Criteria

| Application | HPLC Purity (Area %) | Single Largest Impurity | Total Impurities | Reporting |
|---|---|---|---|---|
| Research use | ≥95% | ≤3.0% | ≤5.0% | All ≥0.1% |
| In vivo studies | ≥98% | ≤1.0% | ≤2.0% | All ≥0.05% |
| Clinical GMP (Phase I–III) | ≥98% | ≤1.0% | ≤2.0% | All ≥0.05% |
| Diagnostic (IVD) | ≥98% | ≤1.0% | ≤2.0% | All ≥0.05% |
| Custom requirement | Per CoA specification | As agreed | As agreed | Per agreement |

## Interpretation Guide

A purity result of 98.5% with a single 0.8% impurity and no other peak above 0.05% indicates a well-purified peptide. The impurity at 0.8% should be identified if manufacturing consistency requires it. A purity result of 95.2% with multiple 0.2–0.5% impurities suggests a batch that may benefit from additional preparative HPLC purification.

When purity falls below specification, review the impurity profile to determine whether a dominant process-related impurity (e.g., a specific deletion product) can be minimized by adjusting synthesis conditions, or whether the impurity profile indicates broad, low-level contamination requiring more fundamental changes.

## Common Issues

- **Co-eluting impurities**: Impurities that co-elute with the main peak inflate apparent purity. Use PDA peak purity analysis or MS detection to verify single-component peak status.
- **Gradient-related baseline drift**: A rising or falling baseline can distort integration. Use blank gradient subtraction and consistent integration parameters.
- **Overloaded injection**: Injecting >50 µg of peptide on a 4.6 mm ID column broadens peaks and under-estimates impurities. Maintain column loading at or below 20–30 µg.

> 🔗 Related: [HPLC Analysis](./hplc-analysis.md) | [LC-MS Testing](./lc-ms-testing.md) | [COA Understanding](./coa-understanding.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
