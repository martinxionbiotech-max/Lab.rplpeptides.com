---
description: "Peptide purification workflow diagram — preparative HPLC process with fraction screening and purity decision logic."
---
# Purification Workflow Diagram

## Preparative HPLC Peptide Purification

Crude peptide obtained from solid-phase synthesis requires purification to remove truncated sequences, deletion peptides, scavenger adducts, and other byproducts formed during assembly and cleavage. The workflow below describes a standard single-pass preparative HPLC purification process. For peptides requiring higher purity grades or those with challenging impurity profiles, re-purification or alternative separation strategies may be employed.

``` mermaid
flowchart TD
    A[Crude Peptide] --> B[Dissolve in<br/>Mobile Phase A];
    B --> C[Filter<br/>0.45 μm];
    C --> D[Equilibrate Column];
    D --> E[Load Sample];
    E --> F[Gradient Elution<br/>5-60% B];
    F --> G[UV Detection<br/>214 nm];
    G --> H[Peak Detection];
    H --> I[Collect Fractions];
    I --> J[Analytical HPLC<br/>Screen Fractions];
    J --> K{Purity ≥98%?};
    K -->|Yes| L[Pool Pure<br/>Fractions];
    K -->|No| M{Purity ≥90%?};
    M -->|Yes| N[Re-purify];
    N --> F;
    M -->|No| O[Discard];
    L --> P[Lyophilize];
    P --> Q[Final Purified<br/>Peptide];
```

## Purification Strategy Selection

The choice of purification technique depends on target peptide properties, scale, and purity requirements. The table below compares the three most common peptide purification strategies.

| Technique | Principle | Best For | Limitations |
|---|---|---|---|
| **RP-HPLC** (Reversed-Phase) | Hydrophobic interaction with C4/C8/C18 stationary phase; elution with acetonitrile/water + 0.1% TFA gradient | Most peptides 2–50 aa; final polishing step | High solvent consumption; limited loading per run; expensive for bulk |
| **IEX** (Ion Exchange) | Electrostatic interaction; cation or anion exchange based on peptide net charge at buffer pH | Initial capture; removing charge-variant impurities; large-scale capture | Limited resolution for similar-length peptides; requires desalting step |
| **SEC** (Size-Exclusion) | Molecular size/Stokes radius; larger molecules elute first | Desalting; buffer exchange; aggregate removal | Poor resolution for similar-sized species; low loading capacity |

**Decision Logic:** For most peptide purification workflows, RP-HPLC serves as the primary polishing step. IEX is recommended when the impurity profile contains significant charge variants or when processing large volumes of crude peptide at early-stage capture. SEC is reserved for final polishing after RP-HPLC to remove aggregates or for buffer exchange into formulation buffers.

## Gradient Optimization Parameters

Gradient design directly impacts resolution, run time, and recovery. Key optimization parameters include:

| Parameter | Typical Range | Optimization Guidance |
|---|---|---|
| **Gradient slope** | 0.5–2.0% B/min | Shallower gradients improve resolution for closely eluting impurities; steeper gradients for rapid screening |
| **Organic modifier** | Acetonitrile (preferred) or Methanol | ACN offers lower UV cutoff (190 nm) and better resolution; MeOH for cost-sensitive large-scale runs |
| **Ion-pairing agent** | 0.05–0.1% TFA | Higher TFA improves peak shape but suppresses MS signal; use 0.01% TFA + 0.09% FA for LC-MS compatibility |
| **Column temperature** | 25–60 °C | Elevated temperature reduces viscosity, improves mass transfer, and alters selectivity |
| **Flow rate** | 10–80 mL/min (prep scale) | Maintain linear velocity of 150–300 cm/hr for optimal resolution; scale from analytical methods |
| **Loading capacity** | 5–20 mg peptide/mL resin | Reduce loading for difficult separations; increase for routine purifications where resolution permits |

**Gradient Design Rule:** For first-pass method development, start with a 1%/min gradient of 5–60% B over 55 minutes at 40 °C. Adjust slope by ±0.3%/min based on observed resolution. If the main peak elutes within the first 10% of the gradient window, reduce the initial %B; if elution occurs above 50% B after a run, shift the gradient window upward.

## Fraction Pooling Criteria

Fraction screening by analytical HPLC is the critical quality gate in the purification workflow. Pooling decisions determine final product purity and yield.

- **Primary pooling**: Combine fractions with ≥98% purity by area percent at 214 nm. This pool becomes the final product after lyophilization.
- **Secondary pooling**: Fractions between 95–97.9% can be pooled separately for re-purification on a second pass. With an optimized gradient, these often yield ≥98% after re-chromatography.
- **Heel fractions**: Fractions below 95% are typically discarded or reserved for research-grade material if purity is ≥90%.
- **Edge cuts**: Leading and trailing edges of the main peak often contain impurities that elute slightly ahead of or behind the target peptide. These should be excluded from the primary pool even if they meet the 98% threshold individually.

**Pooling rule of thumb:** Only pool fractions that are flanked by fractions of comparable purity. If a fraction at 98% is adjacent to fractions at 85% and 90%, it likely contains co-eluting impurities that are not resolved by the analytical method. Confirm by LC-MS before finalizing.

## Purity Decision Flow

| Crude Purity | Action |
|---|---|
| ≥85% | Single pass purification typically sufficient |
| 70–84% | May need re-purification or IEX capture before RP-HPLC polish |
| 60–70% | Requires 2 passes or significant method optimization |
| <60% | Review synthesis conditions; consider alternative synthetic strategy |

---

> 🔗 Related: [Purification Process](../process/purification.md) | [Preparative HPLC](../equipment/preparative-hplc.md) | [HPLC Analysis](../quality-control/hplc-analysis.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
