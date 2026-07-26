---
description: "SEC-HPLC for peptide aggregate analysis — molecular weight distribution, aggregation monitoring, and method parameters for size-exclusion chromatography."
---

# Aggregate Analysis by SEC

## Size-Exclusion HPLC for Peptide Aggregates

## Introduction

Aggregation is a common degradation pathway for peptides in solution and during lyophilization. Aggregates — ranging from soluble dimers and trimers to sub-visible and visible particles — can compromise product safety (by increasing immunogenicity) and efficacy (by reducing the concentration of active monomer). Size-exclusion chromatography (SEC-HPLC) is the primary analytical method for quantifying soluble aggregates in peptide products.

SEC separates molecules by hydrodynamic volume rather than by chemical interaction. Larger aggregates elute earlier because they are excluded from the pores of the stationary phase, while the monomer and fragments are retained longer. SEC provides a direct mass-based (or UV-absorbance-based) estimate of aggregate content and is the method of choice for demonstrating that aggregate levels remain within specification throughout the product shelf life.

## SEC-HPLC Method

### Column Specifications

| Parameter | Recommended | Range |
|---|---|---|
| Stationary phase | Silica-based diol or polymer (e.g., TSKgel G2000SWXL, Zenix SEC-300) | Diol, polyhydroxy, or agarose-based |
| Particle size | 3–5 µm | 1.8–10 µm |
| Pore size | 200–300 Å | 125–500 Å (smaller for peptides <10 kDa) |
| Column dimensions | 7.8 × 300 mm | 4.6–21.2 mm ID; 150–600 mm length |
| Exclusion limit | 30–150 kDa | Match to peptide + aggregate size range |
| pH range | 2.5–7.5 (silica); 2.0–12.0 (polymer) | Depends on column chemistry |

### Mobile Phase and Operating Conditions

| Parameter | Recommended | Notes |
|---|---|---|
| Mobile phase | 100 mM phosphate + 200 mM NaCl, pH 7.0 | Salt suppresses ionic interactions |
| Organic modifier | 5–15% acetonitrile or isopropanol (if needed) | Reduces hydrophobic interactions |
| Flow rate | 0.5 mL/min | 0.2–1.0 mL/min; slower for better resolution |
| Temperature | Ambient (25 °C) | Controlled at 25 ± 2 °C for reproducibility |
| Detection | UV 214 nm (280 nm for Tyr/Trp-containing) | 214 nm for universal peptide detection |
| Injection load | 10–50 µg (on column) | Avoid overloading; 25 µg typical |
| Run time | 30–40 min | 1.5–2× column void volume |
| Calibration standards | Gel filtration standards (thyroglobulin, albumin, RNase, aprotinin) | For apparent MW estimation |

## Aggregate Types and Identification

### SEC Elution Profiles

| Aggregate Species | Approximate Apparent MW | Relative Retention Time (RRT) | Typical Level (%) | Concern Level |
|---|---|---|---|---|
| Higher-order oligomers (>10-mer) | >50 kDa | 0.45–0.55 | <0.1% | Critical (if present) |
| Hexamer | 6× monomer | 0.55–0.65 | <0.5% | High |
| Tetramer | 4× monomer | 0.65–0.72 | <0.3% | High |
| Trimer | 3× monomer | 0.72–0.80 | <0.5% | Moderate |
| Dimer | 2× monomer | 0.80–0.90 | ≤2% | Moderate |
| **Monomer** | 1× monomer | 1.00 (reference) | ≥95% | Target |
| Fragment (large) | < monomer | 1.05–1.25 | ≤2% | Low |
| Fragment (small) | ≪ monomer | 1.25–1.50 | ≤1% | Low |

### Differentiation from Non-SEC Peaks

A peak eluting at the void volume (typically RRT 0.40–0.50) may represent either aggregates >300 kDa (excluded from pores) or, in some cases, micellar structures. Confirm aggregation by:
- **Light scattering detection**: Use multi-angle light scattering (MALS) to confirm molecular weight
- **Second-dimension analysis**: Collect SEC fraction and analyze by reversed-phase HPLC or MS
- **Filter test**: Pre-filter the sample through 0.2 µm; if the void peak disappears, it was a particle rather than soluble aggregate

## Acceptance Criteria and Limits

| Application | Monomer (%) | Total Aggregates (%) | Dimer (%) | Higher-order Oligomers (%) | Fragments (%) |
|---|---|---|---|---|---|
| Research peptide (non-sterile) | ≥95 | ≤5 | ≤3 | ≤2 | ≤3 |
| In vivo / injectable grade | ≥97 | ≤3 | ≤2 | ≤1 | ≤2 |
| GMP (clinical/commercial) | ≥98 | ≤2 | ≤1.5 | ≤0.5 | ≤1.5 |
| Peptide therapeutic *(parenteral)* | ≥99 | ≤1 | ≤0.8 | ≤0.2 | ≤1.0 |
| Peptide therapeutic *(lyophilized)* | ≥98 | ≤2 | ≤1.5 | ≤0.5 | ≤1.0 |

For peptides with inherent aggregation propensity (e.g., hydrophobic sequences, β-sheet-forming motifs), tighter limits may be set based on manufacturing capability and stability data.

## Interpretation Guide

A normal SEC profile shows a sharp monomer peak with minimal front-shoulder (dimer) and no void-volume peak. If dimer exceeds 2% in a GMP batch, investigate formulation conditions (pH, ionic strength, excipient compatibility) and storage parameters (temperature, freeze-thaw cycles). A void-volume peak of any size in an injectable product is a critical deviation and requires root cause investigation.

For stability studies, the % monomer should not decrease by more than 2% from the initial value over the claimed shelf life. A decrease ≥5% suggests a fundamental formulation or packaging deficiency.

## Common Issues

- **Non-size-exclusion effects**: Ionic or hydrophobic interactions between the peptide and SEC resin cause anomalous retention (peak tailing, late elution). Mitigate by increasing mobile phase ionic strength (≥200 mM salt) or adding 5–15% organic modifier.
- **On-column aggregation**: High concentration (>5 mg/mL) or prolonged residence time on the column can induce artificial aggregation. Reduce injection load and confirm by running the same sample at two different concentrations.
- **Column fouling**: Accumulation of strongly retained material alters selectivity over time. Include a periodic column regeneration protocol (e.g., 1–2 column volumes of 0.1 M NaOH followed by re-equilibration).
- **Sample preparation-induced aggregates**: Vortexing, rapid pipetting, or freeze-thaw of peptide solutions can generate artifactual aggregates. Prepare samples gently and consistently.

> 🔗 Related: [HPLC Analysis](./hplc-analysis.md) | [Stability Testing](./stability-testing.md) | [Impurity Profiling](./impurity-profiling.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
