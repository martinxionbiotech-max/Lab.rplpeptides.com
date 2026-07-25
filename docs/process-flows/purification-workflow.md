---
description: "Peptide purification workflow diagram — preparative HPLC process with fraction screening and purity decision logic."
---
# Purification Workflow Diagram

## Preparative HPLC Peptide Purification

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

---

## Purity Decision Flow

| Crude Purity | Action |
|---|---|
| ≥85% | Single pass purification |
| 70–84% | May need re-purification |
| 60–70% | Requires 2 passes or method optimization |
| <60% | Review synthesis conditions |

- **Preparative HPLC Peptide Purification** — Review the section above for key parameters, methods, and quality criteria.
- **Purity Decision Flow** — Review the section above for key parameters, methods, and quality criteria.


---

## Key Takeaways

- **Preparative HPLC Peptide Purification** — Review the section above for key parameters, methods, and quality criteria.
- **Purity Decision Flow** — Review the section above for key parameters, methods, and quality criteria.

> 🔗 Related: [Purification Process](../process/purification.md) | [Preparative HPLC](../equipment/preparative-hplc.md) | [HPLC Analysis](../quality-control/hplc-analysis.md)
