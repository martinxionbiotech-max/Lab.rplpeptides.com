---
description: "HPLC analysis for peptide purity determination — reversed-phase methods, gradient conditions, column selection, and calculations."
---
# HPLC Analysis


## TL;DR

Reversed-phase HPLC with UV detection at 214 nm is the primary method for peptide purity determination. A C18 column with 0.1% TFA in water/acetonitrile gradient is the standard configuration.

## Principle

Reversed-phase HPLC separates peptide components based on hydrophobicity. The peptide elutes as a peak, and purity is calculated as the area percentage of the main peak relative to all detected peaks.

---

## What Are the Standard HPLC Method Parameters?

| Parameter | Typical Value |
|---|---|
| Column | C18, 4.6 × 250 mm, 5 μm |
| Mobile phase A | 0.05–0.1% TFA in water |
| Mobile phase B | 0.05–0.1% TFA in acetonitrile |
| Gradient | 5–60% B over 20–40 min |
| Flow rate | 1.0 mL/min |
| Detection | UV 214 nm |
| Temperature | 25 °C |
| Injection | 10–50 μL |

---

## Purity Calculation

```
% Purity = (Area of main peak / Total area of all peaks) × 100
```

### Acceptance Criteria
| Grade | Minimum Purity |
|---|---|
| Crude | — (baseline) |
| Research | ≥95% |
| Purified | ≥98% |
| GMP | ≥98% (per COA spec) |

---

## Interpreting a Chromatogram

- **Main peak**: Target peptide
- **Earlier eluting peaks**: Typically deletion sequences (shorter)
- **Later eluting peaks**: Truncated peptides or hydrophobic impurities
- **Baseline separation**: Indicates good resolution

---

## Related Tests

- Purity analysis
- Impurity profiling
- Method validation

- **Peptide Purity Determination** — Review the section above for key parameters, methods, and quality criteria.
- **What Are the Standard HPLC Method Parameters?** — See the section for detailed parameters and specifications.
- **Purity Calculation** — Review the section above for key parameters, methods, and quality criteria.
- **Interpreting a Chromatogram** — Review the section above for key parameters, methods, and quality criteria.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What wavelength is used for peptide detection?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "214 nm (amide bond absorption) is the primary wavelength. 254/280 nm are used as secondary channels for aromatic residues detection."
      }
    }
    {
      "@type": "Question",
      "name": "What is the standard mobile phase?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Mobile phase A: 0.1% TFA in water. Mobile phase B: 0.1% TFA in acetonitrile. TFA acts as an ion-pairing agent for better peak shape."
      }
    }
    {
      "@type": "Question",
      "name": "What run time is typical for purity analysis?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Standard analytical runs are 20\u201340 minutes. Fast methods (10\u201315 min) are used for in-process monitoring."
      }
    }
    {
      "@type": "Question",
      "name": "How is purity calculated?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Purity = (area of main peak / total area of all peaks) \u00d7 100%. Integrate all peaks above 0.05% area threshold."
      }
    }
    {
      "@type": "Question",
      "name": "What causes peak tailing in peptide HPLC?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Peak tailing is caused by secondary interactions with free silanol groups. Improve by lowering pH, increasing temperature, or using hybrid/charged surface columns."
      }
    }
  ]
}
</script>

> 🔗 Related: [Analytical HPLC System](../equipment/analytical-hplc.md) | [Purity Analysis](./purity-analysis.md) | [LC-MS Testing](./lc-ms-testing.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/)

---

## Key Takeaways

- **What Are the Standard HPLC Method Parameters?** — See the section above for detailed parameters and specifications.
- **Purity Calculation** — Review the section above for key parameters, methods, and quality criteria.
- **Interpreting a Chromatogram** — Review the section above for key parameters, methods, and quality criteria.
