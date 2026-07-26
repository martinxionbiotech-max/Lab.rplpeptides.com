---
description: "Endotoxin testing for peptide products — LAL assay methods, interference testing, and USP acceptance criteria."
---

# Endotoxin Testing

## Bacterial Endotoxins (LAL/rFC Test)

## Introduction

Endotoxin testing detects and quantifies lipopolysaccharides (LPS) from the outer membrane of Gram-negative bacteria. For peptide products intended for parenteral administration, endotoxin levels must be controlled below thresholds defined by USP <85> and Ph. Eur. 2.6.14. Even low levels of endotoxin can trigger pyrogenic responses (fever, inflammation, hypotension) upon injection.

Two reagent systems are available for endotoxin testing: the traditional Limulus amebocyte lysate (LAL), derived from horseshoe crab blood, and the synthetic recombinant Factor C (rFC) assay, which uses a genetically engineered version of the endotoxin-sensitive serine protease zymogen. rFC is increasingly preferred due to its sustainability, batch-to-batch consistency, and absence of animal-derived components.

## LAL vs. rFC Methods

| Parameter | LAL (Limulus Amebocyte Lysate) | rFC (Recombinant Factor C) |
|---|---|---|
| Source | Horseshoe crab (*Limulus polyphemus* or *Tachypleus tridentatus*) | Recombinant *E. coli* (synthetic gene) |
| Mechanism | Factor C → Factor B → pro-clotting enzyme → coagulin | rFC → activated rFC → cleaves fluorogenic substrate |
| Assay principle | Gel-clot, turbidimetric, or chromogenic | Fluorescence-based |
| Sensitivity range | 0.001–0.1 EU/mL (kinetic); 0.03 EU/mL (gel-clot) | 0.001–0.1 EU/mL (kinetic) |
| Interference profile | May cross-react with β-glucans | No β-glucan interference |
| Regulatory acceptance | USP <85>, Ph. Eur. 2.6.14 | USP <85> (since 2019), Ph. Eur. 2.6.14 (since 2022) |
| Animal-free | No | Yes |
| Lot-to-lot variability | Moderate (biological source) | Low (synthetic) |

## USP <85> Methods

| Method | Format | Quantitative | Sensitivity (EU/mL) | Instrument Required | Automation |
|---|---|---|---|---|---|
| Gel-clot | Test tubes | Semi-quantitative (limit test) | 0.03–0.5 | None (water bath, 37 °C) | No |
| Kinetic turbidimetric | Microplate or tube | Yes | 0.001–0.1 | Plate reader (340–360 nm, 37 °C) | Yes |
| Kinetic chromogenic | Microplate or tube | Yes | 0.001–0.1 | Plate reader (405–410 nm, 37 °C) | Yes |
| rFC (fluorogenic) | Microplate | Yes | 0.001–0.1 | Plate reader (Ex 380/Em 440, 37 °C) | Yes |

The kinetic chromogenic method (LAL or rFC) is the most widely adopted for peptide products due to its high sensitivity, quantitative output, and suitability for automated 96-well plate processing.

## Acceptance Criteria (USP <85>)

| Route of Administration | Endotoxin Limit (EU) | Basis |
|---|---|---|
| Injectable (intravenous) | ≤5.0 EU/kg body weight/h | K = 5.0 EU/kg/h |
| Intrathecal | ≤0.2 EU/kg body weight/h | K = 0.2 EU/kg/h |
| Radiopharmaceuticals (IV) | ≤175 EU/Vmax | 175 EU per maximum human dose |
| Water for injection (WFI) | ≤0.25 EU/mL | Per USP monograph |
| Peptide product (general research) | ≤10 EU/mg (or ≤5 EU/mg for GMP) | Per internal specification |

### Limit Calculation for a Peptide Product

The endotoxin limit for a specific product is calculated as:

```
Endotoxin Limit (EU/mg) = K / M
```

Where:
- K = threshold pyrogenic dose per kg per hour (5.0 EU/kg/h for IV; 0.2 EU/kg/h for IT)
- M = maximum human dose per kg per hour (mg/kg/h)

Example: If the maximum human dose of the peptide is 0.1 mg/kg/h:
```
Limit = 5.0 EU/kg/h ÷ 0.1 mg/kg/h = 50 EU/mg
```

## Interference Testing

Before routine endotoxin testing, each peptide product must undergo an interference test to confirm that the sample matrix does not inhibit or enhance the LAL/rFC reaction.

### Protocol (USP <85>, Ph. Eur. 2.6.14)

1. Prepare the peptide sample at the intended test concentration in endotoxin-free water (LAL reagent water, LRW)
2. Spike the sample with a known concentration of endotoxin (typically 0.5 EU/mL)
3. Test the spiked sample, unspiked sample, and standard curve in parallel
4. Calculate spike recovery

### Acceptance Criteria

| Parameter | Criterion | Action if Failed |
|---|---|---|
| Spike recovery | 50–200% of expected (0.5 EU spike) | Dilute sample further, adjust pH, use a different method |
| Standard curve R² | ≥0.980 | Re-prepare standards; check pipetting |
| Negative control | <LOD (e.g., <0.005 EU/mL) | Investigate water or reagent contamination |
| Positive product control (PPC) | Within 50–200% of spike | Repeat at 1:2, 1:4, 1:8 dilutions |
| Coefficient of variation (replicates) | ≤10% | Improve pipetting precision |

For peptides that fail interference screening at a 1:10 dilution, continue to test at 1:50, 1:100, and 1:500 dilutions. If interference persists, switch to the rFC method (which has a different buffer system and is less sensitive to sample matrix effects) or use an alternative test such as the monocyte activation test (MAT).

## Interpretation Guide

A passing endotoxin result (e.g., <2.0 EU/mg for a GMP peptide) indicates the product is suitable for parenteral administration at the intended dose. Sporadic positive results near the limit should be investigated — if a few vials test slightly above the limit, it may indicate a filling line contamination event rather than a bulk product problem. In such cases, retest the bulk material and increase environmental monitoring during filling.

For research peptides tested at ≤10 EU/mg, a result of <5 EU/mg is considered excellent and indicates no significant endotoxin burden from raw materials or manufacturing.

## Common Issues

- **β-glucan interference**: β-glucans from cellulose filters, paper, or certain excipients can activate the LAL Factor G pathway, producing false positives. The rFC assay avoids this entirely.
- **pH interference**: The LAL/rFC reaction requires pH 6.0–8.0. Peptide samples buffered at extreme pH must be neutralized or diluted into LRW before testing.
- **Poor spike recovery at high peptide concentration**: Highly concentrated peptide solutions (>5 mg/mL) frequently suppress the LAL reaction. Dilution to ≤1 mg/mL for the test is a common remedy.
- **Glassware contamination**: All glassware must be depyrogenated (250 °C, ≥30 min) or certified endotoxin-free. Use only endotoxin-free pipette tips and microplates.

> 🔗 Related: [Microbial Limits Testing](./microbial-limits.md) | [Quality Control Overview](./index.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
