---
description: "Preparative HPLC peptide purification — method development, column selection, gradient optimization, and purity targets."
---
# Purification


## TL;DR

Preparative HPLC is the standard method for peptide purification to ≥98% purity. Method development focuses on gradient selection, column choice, and fraction screening by analytical HPLC.

## Why Peptides Need Purification

Crude peptide from SPPS typically contains:
- **Target peptide** (60–85%)
- **Deletion sequences** (missing one or more amino acids)
- **Truncated sequences** (incomplete synthesis)
- **Scavenger residues** from cleavage
- **Salts and organic impurities**

---

## Preparative HPLC Method

### Column Selection

| Parameter | Research Scale | Process Scale |
|---|---|---|
| Column ID | 10–30 mm | 50–200 mm |
| Particle size | 5–10 μm | 10–30 μm |
| Stationary phase | C18 (most common), C8, C4 | C18 |
| Length | 150–250 mm | 250–300 mm |

### Mobile Phase

| Phase | Typical Composition |
|---|---|
| A (aqueous) | 0.05–0.1% TFA in water |
| B (organic) | 0.05–0.1% TFA in acetonitrile |
| Alternative A | 0.1% formic acid or 20 mM NH₄HCO₃ |
| Alternative B | Methanol or isopropanol |

### Gradient Profile (Typical)

| Time | %B | Event |
|---|---|---|
| 0–5 min | 5–10% | Equilibration/loading |
| 5–30 min | 10–50% | Linear gradient |
| 30–35 min | 50–95% | Column wash |
| 35–45 min | 95–5% | Re-equilibration |

---

## Purification Process

``` mermaid
flowchart LR
    A[Crude Peptide] --> B[Dissolve in<br/>Mobile Phase A];
    B --> C[Filter<br/>0.45 μm];
    C --> D[Inject onto<br/>Prep Column];
    D --> E[Gradient Elution];
    E --> F[UV Detection<br/>214/254 nm];
    F --> G[Fraction Collection];
    G --> H[Analytical QC<br/>of Fractions];
    H --> I{>98% Purity?};
    I -->|Yes| J[Pool & Lyophilize];
    I -->|No| K[Re-purify or Discard];
```

---

## Key Parameters

### Loading Capacity
| Column Size | Maximum Load (crude) |
|---|---|
| 10 mm ID | 5–20 mg |
| 20 mm ID | 20–100 mg |
| 30 mm ID | 100–500 mg |
| 50 mm ID | 0.5–2 g |
| 100 mm ID | 2–10 g |

### Detection Wavelengths
- **214 nm**: Peptide bond absorption (most sensitive)
- **254 nm**: Aromatic residues (Phe, Tyr, Trp)
- **280 nm**: Tyr and Trp

### Flow Rate
| Column ID | Flow Rate |
|---|---|
| 10 mm | 3–5 mL/min |
| 20 mm | 10–20 mL/min |
| 30 mm | 20–40 mL/min |
| 50 mm | 60–120 mL/min |

---

## Common Challenges

| Issue | Cause | Solution |
|---|---|---|
| Poor resolution | Shallow gradient too fast | Extend gradient or adjust slope |
| Peak tailing | Column overload | Reduce load or use larger column |
| Multiple peaks | Deletion sequences | Optimize SPPS synthesis |
| Low recovery | Peptide precipitation | Add co-solvent or adjust pH |

---

## Alternative Purification Methods

| Method | Use Case |
|---|---|
| Ion exchange | Charged peptides, removal of TFA counter-ion |
| Size exclusion | Desalting, buffer exchange |
| Flash C18 | Fast initial purification |
| Reversed-phase | Industry standard for most peptides |

- **Preparative HPLC for Peptide Purification** — Review the section above for key parameters, methods, and quality criteria.
- **Why Peptides Need Purification** — See the section for detailed parameters and specifications.
- **Preparative HPLC Method** — Review the section above for key parameters, methods, and quality criteria.
- **Purification Process** — Review the section above for key parameters, methods, and quality criteria.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What purity standard is typical for research peptides?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Research-grade peptides typically target \u226595% purity by HPLC. GMP-grade requires \u226598% purity for clinical applications."
      }
    }
    {
      "@type": "Question",
      "name": "What column type is used for prep HPLC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "C18 reversed-phase columns (10\u201330 \u03bcm particle size) are standard. Column diameter ranges from 10 mm (lab) to 100+ mm (production)."
      }
    }
    {
      "@type": "Question",
      "name": "How is gradient optimized?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Start with 5\u201360% acetonitrile gradient over 30\u201360 column volumes. Adjust slope, temperature, and pH to improve separation of critical peak pairs."
      }
    }
    {
      "@type": "Question",
      "name": "What is typical product recovery?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Single-pass recovery is 60\u201385% depending on purity target. Re-purification may be needed for \u226598% purity, reducing overall recovery."
      }
    }
    {
      "@type": "Question",
      "name": "How are fractions screened?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Fractions are screened by analytical HPLC. Pools with \u226598% purity are combined, lower purity fractions may be re-purified or discarded."
      }
    }
  ]
}
</script>

> 🔗 Related: [SPPS Process](./spps-process.md) | [Preparative HPLC System](../equipment/preparative-hplc.md) | [HPLC Analysis](../quality-control/hplc-analysis.md) | [LC-MS Testing](../quality-control/lc-ms-testing.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/)

---

## Key Takeaways

- **Why Peptides Need Purification** — See the section above for detailed parameters and specifications.
- **Preparative HPLC Method** — Review the section above for key parameters, methods, and quality criteria.
- **Purification Process** — Review the section above for key parameters, methods, and quality criteria.
- **Key Parameters** — Review the section above for key parameters, methods, and quality criteria.
