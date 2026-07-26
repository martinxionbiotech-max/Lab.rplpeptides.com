---
description: "TFA (trifluoroacetic acid) — purity grades, role in cleavage cocktails, concentration guidelines by resin type, handling hazards, waste disposal protocols, and use as HPLC ion-pairing agent."
---

# TFA — Trifluoroacetic Acid

## Essential Reagent for Cleavage, Deprotection, and Analysis

## Introduction

Trifluoroacetic acid (TFA) is the single most important reagent in peptide workup and analysis. In Fmoc SPPS, TFA serves dual critical roles: as the primary component of cleavage cocktails that release the peptide from the solid support and remove side-chain protecting groups, and as an ion-pairing agent in HPLC mobile phases that sharpens peptide peaks and improves resolution. With a pKa of 0.23, TFA is one of the strongest carboxylic acids, yet its moderate boiling point (72.4 °C) allows convenient removal by evaporation. Proper selection of TFA grade and understanding of its concentration effects are essential for reproducible cleavage yields and chromatographic performance.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | Trifluoroacetic acid |
| **CAS number** | 76-05-1 |
| **Molecular formula** | CF₃COOH |
| **Molecular weight** | 114.02 g/mol |
| **Boiling point** | 72.4 °C (at 1 atm) |
| **Melting point** | −15.4 °C |
| **Density** | 1.48 g/mL (20 °C) |
| **pKa** | 0.23 |
| **Dielectric constant (ε)** | 8.55 (25 °C) |
| **Viscosity** | 0.81 cP (25 °C) |
| **Vapour pressure** | 105 mmHg (25 °C) |
| **Refractive index** | 1.285 (nD²⁰) |

## Purity Grades

| Grade | Purity | Water Content | Typical Use | Price Index |
|-------|--------|--------------|-------------|-------------|
| Synthesis grade | ≥99.0% | ≤0.1% | Peptide cleavage | Low |
| Reagent grade | ≥99.5% | ≤0.05% | General laboratory | Low |
| HPLC grade | ≥99.8% | ≤0.01% | HPLC mobile phase | Moderate |
| LC-MS grade | ≥99.9% | ≤0.005% | LC-MS analysis | High |
| Biotech grade | ≥99.5% | ≤0.05% | GMP manufacturing | Moderate |
| Anhydrous grade | ≥99.9% | ≤0.005% | Water-sensitive couplings | High |

**Selection guide:** For routine peptide cleavage, synthesis grade is sufficient. For HPLC mobile phase preparation, use HPLC grade or higher. Do not substitute — lower grades contain visible-wavelength UV-absorbing impurities and higher water content that reduces cleavage efficiency.

## Role in Cleavage Cocktails

TFA is the backbone of all standard cleavage cocktails. Its concentration in the cocktail determines whether the peptide is fully deprotected and released, or whether side-chain protecting groups are retained.

### Fmoc SPPS Cleavage (Standard)

| Resin Type | TFA Concentration | Cleavage Time | Cocktail Components |
|------------|------------------|---------------|-------------------|
| Wang resin | 90–95% | 1.5–3 h | TFA/TIS/H₂O (95:2.5:2.5) |
| Rink Amide | 90–95% | 1–2 h | TFA/TIS/H₂O (95:2.5:2.5) |
| Rink Acid | 90–95% | 1–2 h | TFA/TIS/H₂O (95:2.5:2.5) |
| 2-Cl-Trt resin | 95% | 30 min | TFA/DCM (1:99) for protected peptide |
| Sieber resin | 1–5% | 5–15 min | TFA/DCM (1–5%) — retains side-chain PGs |

### Concentration Recommendations by Cleavage Objective

| Objective | TFA % | Scavenger System | Time | Notes |
|-----------|-------|-----------------|------|-------|
| Full deprotection + cleavage | 95% | TIS 2.5%, H₂O 2.5% | 1.5–3 h | Standard Reagent R |
| Full deprotection + Trp protection | 88% | Phenol 5%, H₂O 5%, TIS 2% | 2–4 h | Reagent B |
| Full deprotection + Trp + Arg(Pbf) | 82.5% | Phenol 5%, H₂O 5%, TIS 2.5%, EDT 5% | 2–4 h | Reagent K |
| Side-chain protected peptide | 1–5% | In DCM; no scavenger | 5–30 min | Sieber or 2-Cl-Trt only |
| Nⁿ-Boc removal (Boc SPPS) | 50% | In DCM | 20–30 min | Intermediate step |

### Mechanism of TFA Action in Cleavage

TFA protonates the peptide-resin linkage (ester or amide bond), generating a labile O-acyl or N-acyl intermediate that cleaves to release the free peptide. Simultaneously, TFA protonates acid-labile protecting groups (tBu, Boc, Trt, Pbf), generating carbocations that must be trapped by scavengers. The water content in TFA (<0.05% in HPLC grade) affects the equilibrium: excess water slows the protonation equilibrium, while anhydrous TFA accelerates cleavage but may leave trace of benzyl-type protecting groups incompletely removed.

## TFA in HPLC Analysis

| Parameter | Recommendation | Effect |
|-----------|---------------|--------|
| Concentration | 0.05–0.1% (v/v) in water and acetonitrile | Optimum peak shape; below 0.05% broadens peaks |
| pH of 0.1% aqueous TFA | ~2.0 | Suppresses silanol ionisation on C18 |
| UV transparency at 214 nm | Excellent (A <0.002 AU) at 0.1% | Allows sensitive peptide detection |
| Volatility | Complete under vacuum | Compatible with LC-MS and fraction lyophilisation |
| Gradients | Compatible; TFA concentration kept constant | Maintain constant ion-pairing throughout run |

**Note:** TFA concentration must be identical in both mobile phases A and B to avoid baseline drift during gradient runs. A difference of even 0.02% produces a measurable UV absorbance drift at 214 nm.

## Handling Hazards and Safety

| Hazard | H-Statement | Precaution |
|--------|-------------|------------|
| Corrosive | H314 — severe skin burns and eye damage | Acid-resistant gloves (neoprene or butyl rubber), face shield |
| Toxic by inhalation | H332 — harmful if inhaled | Fume hood mandatory; never work open-bench |
| Lachrymator | — | Causes profuse tearing at >1 ppm |
| Volatile | — | Store in vented cabinet; cap immediately after use |
| Water-reactive | — | Contact with water generates exotherm and HF |
| Tissue penetration | — | Absorbed through skin; wash immediately if splashed |

**First aid:** Skin contact — flush with copious water for ≥15 min, remove contaminated clothing. Eye contact — irrigate continuously for ≥20 min, seek immediate medical attention. Inhalation — move to fresh air; oxygen if available.

## Waste Disposal

TFA waste requires special handling as it is not compatible with standard organic solvent waste streams:

| Waste Type | Disposal Method | Notes |
|------------|----------------|-------|
| Cleavage cocktail (spent) | Collect separately; neutralise with NaOH before aqueous disposal | TFA content high enough to acidify large volumes |
| TFA/water mixtures | Cannot be incinerated (generates HF) | Neutralise to pH 6–8, then aqueous disposal |
| Empty containers | Triple-rinse with water; dispose as corrosive waste | Residual vapour is highly corrosive |
| Spent rag/adsorbent | Seal in polyethylene bag; incinerator disposal | Avoid cellulose-based adsorbents (decompose) |

**Never mix TFA waste with halogenated solvent waste streams containing DCM — TFA reacts with DCM under basic conditions to form explosive diazomethane-like intermediates.**

## Storage Recommendations

- **Container:** High-density polyethylene (HDPE) or PTFE — avoid glass for long-term storage (TFA etches glass, introducing silicate impurities)
- **Temperature:** Room temperature (15–25 °C) in a cool, well-ventilated area
- **Shelf life:** >3 years if moisture ingress is prevented. TFA itself is stable but absorbs water from air
- **Purity monitoring:** Check water content by Karl Fischer titration before use in moisture-sensitive cleavage applications

---

> **🔗 Related:** [Cleavage Process](../process/cleavage.md) | [Acetonitrile](./acetonitrile.md) | [Purification](../process/purification.md) | [Scavenger Selection Guide](./scavenger-selection-guide.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
