---
description: "Peptide salt form selection — TFA removal via HCl/acetate exchange, acetate vs. HCl vs. TFA salts, and impact on solubility and stability."
---

# Salt Form Selection

## TL;DR

Crude peptides are isolated as TFA (trifluoroacetate) salts after standard Fmoc cleavage. TFA salts can interfere with biological assays, solubility, and stability. Salt exchange to acetate, HCl, or other counterions is often required. The choice of salt form affects hygroscopicity, solubility profile, peptide content, and formulation compatibility.

---

## Why Salt Form Matters

| Property | TFA Salt | Acetate Salt | HCl Salt |
|---|---|---|---|
| Peptide content | 70–85% | 75–90% | 80–95% |
| Hygroscopicity | Moderate | Moderate–High | Low–Moderate |
| Acetonitrile solubility | Good | Moderate | Low |
| Water solubility | Excellent | Excellent | Good–Excellent |
| IR absorption (1680 cm⁻¹) | Strong TFA carbonyl | Absent | Absent |
| Cell-based assay interference | Cytotoxic at >10 mM | Minimal | Minimal |
| HPLC peak shape | Sharp (ion-pairing) | Normal | Normal |
| Stability | Good | Good | May degrade at low pH |

---

## Why Remove TFA?

TFA is the standard counterion because the cleavage cocktail uses 90–95% TFA. However:

1. **TFA absorbs strongly in the IR** at 1,673 cm⁻¹ — interferes with FTIR characterization
2. **TFA suppresses ion signals** in ESI-MS — reduces detection sensitivity
3. **TFA is cytotoxic** at elevated concentrations — problematic for cell-based assays
4. **TFA content is variable** (peptide-dependent) — complicates accurate dosing
5. **TFA ion-pairs strongly** — can alter HPLC retention times unpredictably

---

## Salt Exchange Methods

### Lyophilization-Based Exchange

The most common method. Dissolve TFA-peptide in exchange medium and lyophilize.

| Method | Exchange Medium | Final Salt | Efficiency |
|---|---|---|---|
| HCl exchange | 10–50 mM HCl | HCl salt | 85–98% |
| Acetate exchange | 10% acetic acid (v/v) | Acetate salt | 80–95% |
| Acetate exchange | 0.1 M NH₄OAc (pH 5–6) | Acetate salt | 85–95% |
| Phosphate exchange | 10 mM phosphate buffer | Phosphate salt | 60–85% |

**Protocol** (acetate exchange):
1. Dissolve TFA-peptide (10 mg/mL) in 10% acetic acid
2. Lyophilize
3. Repeat 2–3× until residual TFA <1% (w/w)
4. Final product is acetate salt

### Chromatographic Exchange

| Method | Column | Mobile Phase | Efficiency |
|---|---|---|---|
| Ion-exchange (anion) | Q-Sepharose or DEAE | NH₄OAc gradient | 95–99% |
| Size-exclusion + exchange | Sephadex G-10 | NH₄OAc → H₂O | 90–95% |
| Preparative HPLC gradient change | C18 column | NH₄OAc buffer → H₂O | Variable |

---

## Properties by Counterion

| Counterion | pKₐ | Peptide Content (typical) | Assay Compatibility |
|---|---|---|---|
| TFA (CF₃COO⁻) | 0.23 | 70–80% | Poor — cytotoxic |
| Acetate (CH₃COO⁻) | 4.76 | 75–88% | Good |
| Chloride (Cl⁻) | −7 | 80–95% | Excellent |
| Phosphate (H₂PO₄⁻) | 2.14 | 70–80% | Good |
| Citrate | 3.13, 4.76, 6.40 | 75–85% | Good |
| Mesylate (CH₃SO₃⁻) | −1.9 | 80–90% | Good |
| Tartrate | 3.0, 4.4 | 75–85% | Moderate |

---

## Impact on Peptide Content

The counterion contributes to the total mass of the lyophilized powder. Higher counterion molecular weight = lower peptide content.

| Counterion | MW (g/mol) | Number of charges per peptide | Peptide Content Example (MW 1,500 peptide) |
|---|---|---|---|
| TFA | 113 | 1 | 77% |
| TFA | 113 | 3 | 60% |
| Acetate | 59 | 1 | 85% |
| Acetate | 59 | 3 | 72% |
| Chloride | 35.5 | 1 | 87% |
| Chloride | 35.5 | 3 | 75% |

**Formula**: Peptide content (%) = [Peptide MW / (Peptide MW + n × Counterion MW + n × H₂O)] × 100%

Where n = number of basic residues (Lys, Arg, His, N-terminus) potentially charged.

---

## Solubility Profiles

| Solvent | TFA Salt | Acetate Salt | HCl Salt |
|---|---|---|---|
| Water (neutral pH) | Excellent | Excellent | Good |
| 5% acetic acid | Excellent | Good | Moderate |
| PBS, pH 7.4 | Good | Good | Moderate |
| Acetonitrile/water | Excellent | Good | Low |
| DMSO | Good | Good | Good |
| Ethanol/water | Moderate | Good | Poor |
| Pure ethanol | Poor | Moderate | Very poor |

---

## Practical Decision Guide

```
Does the peptide need cell-based assays?
├── Yes → Remove TFA (acetate preferred)
└── No  → TFA acceptable for most analytical needs

Is peptide content critical for accurate dosing?
├── Yes → Use HCl salt (highest content)
└── No  → Acetate or TFA acceptable

Is the peptide unstable at low pH?
├── Yes → Acetate or phosphate salt (mild pH)
└── No  → HCl or TFA acceptable

Will the peptide be lyophilized in formulation?
├── Yes → Acetate or HCl salt (lower hygroscopicity)
└── No  → Any salt form acceptable
```

---

## Residual TFA Determination

| Method | LOQ | Use |
|---|---|---|
| ¹⁹F-NMR | 0.01% (w/w) | Most sensitive, requires NMR |
| Ion chromatography | 0.05% (w/w) | Routine QC method |
| HPLC-UV (210 nm) | 0.1% (w/w) | No special equipment needed |
| Combustion ion chromatography | 0.01% | Total fluorine analysis |

---

## Key Takeaways

- TFA is the default counterion after Fmoc cleavage but may interfere with biological assays
- Acetate exchange (3× lyophilization from 10% AcOH) removes >95% of TFA
- HCl salt provides the highest peptide content (80–95%) and is best for accurate dosing
- Counterion choice affects solubility, hygroscopicity, stability, and formulation compatibility
- Peptide content decreases with higher counterion MW and more basic residues
- Always characterize residual TFA content for acetate or HCl-exchanged peptides

> 🔗 Related: [Peptide Content](../quality-control/peptide-content.md) | [Lyophilization](./lyophilization.md) | [Purification](./purification.md) | [Purity Analysis](../quality-control/purity-analysis.md) | [Formulation Excipients](./formulation-excipients.md) | [TFA](../raw-materials/tfa.md) | [Manufacturing Workflow](../manufacturing/manufacturing-workflow.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
