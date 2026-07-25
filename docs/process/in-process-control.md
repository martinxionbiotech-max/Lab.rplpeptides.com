---
description: "In-process control methods for peptide manufacturing — Kaiser test, chloranil test, UV monitoring, conductivity, and automated feedback systems."
---

# In-Process Control

## Monitoring Peptide Synthesis in Real Time

## Purpose

In-process controls (IPC) verify each synthesis step before proceeding, preventing accumulation of errors and ensuring final product quality.

---

## IPC Methods Comparison

| Method | Monitors | Time | Sensitivity | Quantitative |
|---|---|---|---|---|
| **Kaiser test (ninhydrin)** | Free amine | 5–10 min | +++ | Semi |
| **Chloranil test** | Free amine | 2 min | ++ | No |
| **TNBS test** | Free amine | 10 min | ++++ | Yes |
| **UV monitoring (301 nm)** | Deprotection | Real-time | ++ | Yes |
| **Conductivity** | Coupling | Real-time | + | Yes |
| **IR spectroscopy** | Amide bond | Real-time | ++ | Yes |

---

## Kaiser Test Protocol

### Reagent Preparation

| Reagent | Composition |
|---|---|
| A | 5 g ninhydrin in 100 mL ethanol |
| B | 80 g phenol in 20 mL ethanol |
| C | 2 mL 0.001 M KCN in 98 mL pyridine |

### Test

1. Wash 5–10 resin beads with ethanol
2. Add 2 drops each of A, B, C
3. Heat to 100 °C for 5 min
4. Read color:

| Color | Interpretation |
|---|---|
| **Colorless or yellow** | ✅ No free amine — coupling complete |
| **Blue or purple** | ❌ Free amine present — coupling incomplete |
| **Light blue** | ⚠️ May need extended coupling |

---

## Automated IPC with UV Monitoring

### Deprotection Monitoring
- Continuous flow-through UV cell at 301 nm
- Two peaks per deprotection cycle
- Peak area correlates to amino acid loading
- Trend: decreasing area = decreasing resin accessibility

### Conductivity Monitoring
- Measures ion concentration in coupling step
- Drops sharply when coupling completes
- Useful for first ~15 AA; less sensitive later

---

## In-Process Release Criteria

| Step | IPC Check | Pass Criteria |
|---|---|---|
| After resin loading | Loading measurement | Within ±10% target |
| After each coupling | Kaiser test | Negative (yellow) |
| After deprotection | UV monitor | Absorbance peak detected |
| Before cleavage | Final cycle Kaiser | Negative |
| After cleavage | HPLC (crude) | Purity ≥70% expected |
| After purification | HPLC (pooled) | ≥98% per target |

> 🔗 Related: [SPPS Process](../process/spps-process.md) | [Coupling Reaction](../process/coupling-reaction.md) | [HPLC Analysis](../quality-control/hplc-analysis.md) | [Custom Peptide Synthesis at RPL](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
