---
description: "SPPS workflow diagram — complete solid-phase peptide synthesis cycle visualized with Mermaid flowchart."
---
# SPPS Workflow Diagram

## Complete Solid-Phase Peptide Synthesis Process

``` mermaid
flowchart TD
    A[Select Resin] --> B[Swelling<br/>DCM/DMF 30-60 min];
    B --> C[Load First<br/>Fmoc-AA-OH];
    C --> D[Cap Unreacted<br/>Sites];
    D --> E[Fmoc Deprotection<br/>20% Piperidine/DMF];
    E --> F[Wash × 4-6<br/>DMF];
    F --> G[Coupling<br/>Fmoc-AA-OH + Activator];
    G --> H[Wash × 3-4<br/>DMF];
    H --> I{Complete?};
    I -->|Kaiser Test+| J[Repeat Coupling];
    J --> H;
    I -->|Kaiser Test-| K[Next AA?];
    K -->|Yes| E;
    K -->|No| L[Final Fmoc<br/>Deprotection];

    L --> M[Wash × 5<br/>DCM, MeOH];
    M --> N[Cleavage Cocktail<br/>TFA/TIS/H2O];
    N --> O[Precipitation<br/>Cold Ether];
    O --> P[Centrifuge/Wash<br/>× 2-3];
    P --> Q[Dry under N2];
    Q --> R[Crude Peptide<br/>QC: HPLC, MS];

    style A fill:#e1f5fe
    style R fill:#e8f5e9
    style G fill:#fff3e0
    style N fill:#fce4ec
```

---

## Cycle Description

| Step | Key Action | Duration | QC Check |
|---|---|---|---|
| Resin selection | Choose based on C-terminal | — | Loading verification |
| Swelling | DCM or DMF | 30–60 min | Visual |
| Loading | First AA attachment | 1–2 h | Loading measurement |
| Capping | Ac₂O + DIEA | 20–30 min | — |
| Deprotection | 20% piperidine/DMF | 10–15 min | UV 301 nm |
| Coupling | AA + activator + base | 30–60 min | Kaiser test |
| Cleavage | TFA cocktail | 2–4 h | — |
| Precipitation | Cold ether | 5–15 min | Visual |

- **Complete Solid-Phase Peptide Synthesis Process** — Review the section above for key parameters, methods, and quality criteria.
- **Cycle Description** — Review the section above for key parameters, methods, and quality criteria.


---

## Key Takeaways

- **Complete Solid-Phase Peptide Synthesis Process** — Review the section above for key parameters, methods, and quality criteria.
- **Cycle Description** — Review the section above for key parameters, methods, and quality criteria.

> 🔗 Related: [SPPS Process Detail](../process/spps-process.md) | [Manufacturing Workflow](../manufacturing/manufacturing-workflow.md) | [Process Knowledge](../process/index.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
