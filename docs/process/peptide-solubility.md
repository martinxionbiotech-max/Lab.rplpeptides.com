---
description: "Peptide solubility guide — solvent selection, pH optimization, co-solvent strategies, and troubleshooting for peptide dissolution."
---

# Peptide Solubility Guide

## Dissolution Strategies for Peptide Synthesis and QC

## Factors Affecting Peptide Solubility

| Factor | Effect | Example |
|---|---|---|
| Sequence length | Longer = less soluble | >20 AA challenging |
| Hydrophobicity | High = poor aqueous solubility | Leu, Val, Ile clusters |
| Net charge | Charged = better solubility | Basic/acidic residues help |
| Secondary structure | β-sheet = aggregation → precipitation | Membrane peptides |
| Salt form | Acetate > TFA > HCl solubility | Counterion exchange |

---

## Solvent Selection Guide

### For Synthesis

| Solvent | Peptide Solubility | Use Case |
|---|---|---|
| DMF | Good (most sequences) | Standard SPPS |
| NMP | Very good | Difficult sequences |
| DMSO | Excellent | Hydrophobic peptides |
| DCM | Poor | Resin swelling only |
| NMP/DMSO (1:1) | Excellent | Extreme cases |

### For QC (HPLC)

| Solvent | Recommendation |
|---|---|
| Mobile phase A | 0.1% TFA in water |
| Co-solvent | 10-50% acetonitrile or DMSO |
| Initial DMSO stock | If peptide won't dissolve in A |
| Final DMSO in injection | ≤5% to avoid peak distortion |

---

## pH-Dependent Solubility

For peptides with ionizable groups:

| Residue | pKa | Fully Charged pH |
|---|---|---|
| Asp/Glu (acidic) | 4.0 / 4.5 | pH > 6.0 |
| Lys (basic) | 10.5 | pH < 8.5 |
| Arg (basic) | 12.5 | pH < 10.0 |
| His (basic) | 6.0 | pH < 5.0 |

**Rule of thumb**: Peptide is most soluble at pH 2 units away from its pI.

---

## Troubleshooting

| Problem | Solution |
|---|---|
| Peptide won't dissolve in water | Add 10-30% acetonitrile |
| Still insoluble | Try 100% DMSO first, then dilute |
| Aggregates in solution | Add 0.1% TFA or 6 M guanidine |
| Cloudy solution | Increase pH (for acidic) or decrease (for basic) |
| Gel formation | Dilute 2-5×, sonicate, warm gently |
| Precipitates during HPLC gradient | Use less organic in initial conditions |

> 🔗 Related: [Purification](../process/purification.md) | [HPLC Analysis](../quality-control/hplc-analysis.md) | [Formulation & Excipients](../process/formulation-excipients.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
