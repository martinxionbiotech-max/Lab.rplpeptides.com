---
description: "Stability-indicating HPLC method development — forced degradation, peak purity, mass balance, and method robustness for peptide stability studies."
---

# Stability-Indicating HPLC Methods

## Developing Methods for Peptide Degradation Studies

## What Makes a Method Stability-Indicating?

A stability-indicating method (SIM) can separate the parent peptide from all degradation products, process impurities, and excipients. It is essential for shelf-life determination.

---

## Forced Degradation Study Design

| Stress Condition | Protocol | Expected Degradation |
|---|---|---|
| **Acid hydrolysis** | 0.1 M HCl, 25 °C, 24 h | Asp-Pro cleavage, hydrolysis |
| **Base hydrolysis** | 0.1 M NaOH, 25 °C, 4 h | Deamidation, hydrolysis |
| **Thermal (dry)** | 40–80 °C, 1–4 weeks | Aggregation, oxidation |
| **Thermal (solution)** | 25–40 °C, 1–14 days | Multiple pathways |
| **Oxidative** | 0.3–3% H₂O₂, 25 °C, 24 h | Met/Trp/Cys oxidation |
| **Photolytic** | ICH Q1B light, 1.2 M lux·h | Photo-oxidation |
| **Freeze-thaw** | 3 cycles, −80 ↔ 25 °C | Aggregation |

---

## Method Qualification from Forced Degradation

| Criterion | Acceptance | How to Verify |
|---|---|---|
| **Specificity** | Main peak resolved from all degradants | Peak purity by PDA |
| **Mass balance** | Sum of peak areas = 100 ± 5% | Compare stressed vs unstressed |
| **Peak purity** | Main peak angle < purity threshold | PDA 3D data |
| **LOD/LOQ** | Degradants detected at ≤0.1% | S/N ≥ 3 (LOD), ≥ 10 (LOQ) |

---

## Gradient Optimization for SIM

``` mermaid
flowchart LR
    A[Initial gradient<br/>5-60% B/30 min] --> B{All peaks<br/>resolved?};
    B -->|No| C[Flatten slope<br/>at critical region];
    C --> D{Separation<br/>adequate?};
    D -->|No| E[Change pH or<br/>column chemistry];
    E --> D;
    B -->|Yes| F[Shorten run time];
    F --> G[Validate per ICH Q2(R1)];
```

> 🔗 Related: [HPLC Analysis](./hplc-analysis.md) | [Method Validation](./method-validation.md) | [Stability Testing](./stability-testing.md) | [Impurity Profiling](./impurity-profiling.md)
