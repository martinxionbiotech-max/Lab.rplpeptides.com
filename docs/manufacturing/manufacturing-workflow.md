---
description: "End-to-end peptide manufacturing workflow — from resin selection through synthesis, purification, lyophilization, and QC release."
---
# Manufacturing Workflow

## End-to-End Peptide Manufacturing Process

``` mermaid
flowchart TD
    A[Raw Material<br/>Receipt & QC] --> B[Resin Selection<br/>& Loading]
    B --> C[SPPS Assembly<br/>Automated Cycles]
    C --> D[Cleavage<br/>from Resin]
    D --> E[Crude Peptide<br/>QC: HPLC, MS]
    E --> F{Purity ≥ Target?}
    F -->|Yes| G[Lyophilization]
    F -->|No| H[Purification<br/>Prep-HPLC]
    H --> I[Pooled Fractions<br/>QC: HPLC]
    I --> J{Meets Spec?}
    J -->|Yes| G
    J -->|No| H
    G --> K[Final Product<br/>QC Release]
    K --> L[Packaging &<br/>Shipment]
```

---

## Stage-by-Stage Overview

### 1. Raw Material Receipt
- Incoming QC of amino acids, resins, solvents, reagents
- Certificate of Analysis (COA) verification

### 2. SPPS Assembly
- Automated or manual coupling cycles
- Each cycle: deprotection → wash → coupling → wash
- Monitoring: Kaiser test, UV tracking

### 3. Cleavage
- TFA-based cleavage cocktail
- Global deprotection of side-chain protecting groups
- Precipitation in cold ether

### 4. Crude Peptide QC
- Analytical HPLC (purity assessment)
- LC-MS (mass confirmation)
- Decision point: purity ≥ 70–85% → proceed to lyophilization or purification

### 5. Purification (Prep-HPLC)
- Gradient elution on C18 column
- Fraction collection based on UV detection
- Pooled fraction QC

### 6. Lyophilization
- Freeze-drying to remove solvents
- Final product as amorphous or crystalline powder

### 7. Final QC Release
- Full specification testing
- COA generation

---

## Typical Timeline

| Scale | Timeline |
|---|---|
| Research (mg–g) | 1–2 weeks |
| Preclinical (g–10g) | 2–4 weeks |
| Clinical (10g–100g) | 3–6 weeks |
| Commercial (>100g) | 4–10 weeks |

- **End-to-End Peptide Manufacturing Process** — Review the section above for key parameters, methods, and quality criteria.
- **Stage-by-Stage Overview** — Review the section above for key parameters, methods, and quality criteria.
- **Typical Timeline** — Review the section above for key parameters, methods, and quality criteria.


---

## Key Takeaways

- **End-to-End Peptide Manufacturing Process** — Review the section above for key parameters, methods, and quality criteria.
- **Stage-by-Stage Overview** — Review the section above for key parameters, methods, and quality criteria.
- **Typical Timeline** — Review the section above for key parameters, methods, and quality criteria.

> 🔗 Related: [Manufacturing Overview](./peptide-synthesis-overview.md) | [SPPS Process](../process/spps-process.md) | [Process Flows Overview](../process-flows/index.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
