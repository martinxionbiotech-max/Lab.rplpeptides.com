---
description: "Complete SPPS process — resin loading, coupling, deprotection, cleavage, and purification steps with parameters and QC methods."
---
# Solid Phase Peptide Synthesis — Complete Process


## TL;DR

The SPPS cycle consists of: resin preparation → loading → deprotection → coupling → washing (repeated per residue) → final cleavage → purification. Each cycle is monitored by Kaiser test.

SPPS is the standard method for peptide production. A peptide chain is assembled stepwise on insoluble resin beads, with excess reagents removed by simple filtration.

---

## 1. Resin Loading

### Purpose
Attach the first (C-terminal) amino acid to the solid support via a cleavable linker.

### Common Resins
| Resin | Linker | Cleavage | C-terminal Product |
|---|---|---|---|
| Wang resin | p-alkoxybenzyl alcohol | TFA | Carboxylic acid (-COOH) |
| Rink amide resin | Rink amide linker | TFA | Amide (-CONH₂) |
| 2-Chlorotrityl chloride (CTC) | Trityl chloride | Mild TFA | Protected peptide acid |

### Key Parameters
- **Loading capacity**: 0.3–1.5 mmol/g (vendor-specified)
- **Swelling solvent**: DCM or DMF (5–10 mL/g resin)
- **Swelling time**: 30–60 minutes before first coupling
- **First amino acid attachment**: Via symmetric anhydride or pre-activated ester

---

## 2. Coupling Reaction

### Purpose
Sequentially add Fmoc-protected amino acids to the growing peptide chain.

### Materials
- Fmoc-amino acids (2–5 fold molar excess)
- Activator (HBTU, HATU, DIC, or PyBOP)
- Base (DIEA or NMM)
- Solvent (DMF or NMP)

### Activation Chemistry

``` mermaid
graph LR
    A[Fmoc-AA-OH] --> B[+ Activator];
    B --> C[Active Ester];
    C --> D[+ NH2-Peptide-Resin];
    D --> E[Coupled Peptide-Resin];
    E --> F[+ Wash];
```

### Key Parameters
| Parameter | Typical Value | Notes |
|---|---|---|
| Amino acid excess | 3–5 equivalents | Higher for difficult couplings |
| Activation time | 2–5 minutes | Pre-activation before adding to resin |
| Coupling time | 30–60 minutes | Longer for sterically hindered AAs |
| Temperature | 20–50 °C | Microwave: 50–75 °C for faster coupling |
| Solvent | DMF or NMP | DMF most common |

### Monitoring Methods
- **Kaiser test** (ninhydrin): Blue = free amine (incomplete coupling)
- **Chloranil test**: For secondary amines (Proline)
- **UV monitoring**: Track Fmoc removal for coupling efficiency

---

## 3. Deprotection

### Purpose
Remove the Fmoc protecting group from the N-terminal amino acid before the next coupling.

### Standard Deprotection
- **Reagent**: 20–25% piperidine in DMF
- **Time**: 5–15 minutes
- **Temperature**: Room temperature (or 40–50 °C with microwave)

### Mechanism
1. Piperidine removes the Fmoc group
2. Releases dibenzofulvene (UV-active)
3. Dibenzofulvene is trapped by piperidine as a stable adduct

### Monitoring
- **UV absorption**: Measure dibenzofulvene at 301 nm
- **Quantitative**: Track deprotection efficiency per cycle

---

## 4. Cleavage

### Purpose
1. Release the peptide from the resin
2. Remove side-chain protecting groups (global deprotection)

### Standard Cocktail
| Component | Function | Typical % |
|---|---|---|
| TFA | Acid cleavage | 90–95% |
| TIS (triisopropylsilane) | Carbocation scavenger | 2–5% |
| H₂O | Polar scavenger | 2–5% |
| DTT or EDT | For sensitive residues | 0–2% |

### Process
1. Add cleavage cocktail to resin-bound peptide
2. Stir 1.5–4 hours at room temperature
3. Filter to remove resin beads
4. Precipitate peptide in cold diethyl ether or MTBE
5. Centrifuge/wash × 2–3
6. Dry under nitrogen or vacuum

---

## 5. Purification

### Purpose
Remove deletion sequences, truncated peptides, and other impurities from crude product.

### Method: Preparative HPLC
| Parameter | Typical Range |
|---|---|
| Column | C18 reverse phase (10–30 μm) |
| Mobile phase A | 0.1% TFA in water |
| Mobile phase B | 0.1% TFA in acetonitrile |
| Gradient | 5–60% B over 20–60 minutes |
| Detection | UV 214 nm, 254 nm, 280 nm |
| Flow rate | Scale-dependent (10–500 mL/min) |

> See full details: [Purification Process](../process/purification.md)

---

## 6. Lyophilization

### Purpose
Remove water and organic solvents to produce stable peptide powder.

### Process Steps
1. Freeze peptide solution (-40 to -80 °C)
2. Primary drying: Sublime ice under vacuum (0.1–0.5 mbar)
3. Secondary drying: Remove bound water (elevated temperature)

### Expected Outcome
- White to off-white amorphous powder
- Residual moisture: <5% (target <2%)
- Shelf-stable at -20 °C for 2+ years

> See full details: [Lyophilization Process](../process/lyophilization.md)

---

## Process Time Reference

| Step | Typical Duration |
|---|---|
| Resin swelling | 30–60 min |
| Per coupling cycle | 45–90 min |
| Total SPPS (30-mer) | 24–48 hours |
| Cleavage | 2–4 hours |
| Purification | 2–8 hours |
| Lyophilization | 24–48 hours |

- **1. Resin Loading** — Review the section above for key parameters, methods, and quality criteria.
- **2. Coupling Reaction** — Review the section above for key parameters, methods, and quality criteria.
- **3. Deprotection** — Review the section above for key parameters, methods, and quality criteria.
- **5. Purification** — Review the section above for key parameters, methods, and quality criteria.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is the SPPS cycle time per amino acid?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "A standard SPPS cycle takes 45\u201390 minutes per amino acid residue, including deprotection (10\u201315 min), washing (15\u201320 min), and coupling (30\u201360 min)."
      }
    }
    {
      "@type": "Question",
      "name": "How is coupling efficiency verified?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "The Kaiser test (ninhydrin test) is the standard method. Blue solution = incomplete coupling. A negative (colorless/yellow) test confirms completion."
      }
    }
    {
      "@type": "Question",
      "name": "What cleavage cocktail is typically used?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "The standard cocktail is TFA/TIS/H2O (95:2.5:2.5 by volume) for 2\u20134 hours at room temperature. Scavenger selection depends on amino acid composition."
      }
    }
    {
      "@type": "Question",
      "name": "What is the expected crude peptide purity?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Crude purity of 70\u201385% is typical for sequences under 30 amino acids. Lower purity may indicate difficult couplings requiring optimization."
      }
    }
    {
      "@type": "Question",
      "name": "How is the final product dried after cleavage?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "After ether precipitation, the crude peptide is dried under nitrogen flow or vacuum, then characterized by HPLC and MS before purification."
      }
    }
  ]
}
</script>

> 🔗 Related: [Peptide Synthesis Overview](../manufacturing/peptide-synthesis-overview.md) | [Manufacturing Workflow](../manufacturing/manufacturing-workflow.md) | [Resin Loading](./resin-loading.md) | [Coupling Reaction](./coupling-reaction.md) | [Purification](./purification.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/)

---

## Key Takeaways

- **1. Resin Loading** — Review the section above for key parameters, methods, and quality criteria.
- **2. Coupling Reaction** — Review the section above for key parameters, methods, and quality criteria.
- **3. Deprotection** — Review the section above for key parameters, methods, and quality criteria.
- **4. Cleavage** — Review the section above for key parameters, methods, and quality criteria.
