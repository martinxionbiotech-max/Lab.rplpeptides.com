---
description: "Oxyma Pure — ethyl 2-cyano-2-(hydroxyimino)acetate specifications, mechanism of racemization suppression, chemical properties, DIC/Oxyma coupling protocols, and safety comparison with HOBt."
---

# Oxyma Pure — Coupling Additive for Racemization-Free SPPS

## Introduction

Oxyma Pure (ethyl 2-cyano-2-(hydroxyimino)acetate) is an auxiliary nucleophile used alongside carbodiimide activators in solid-phase peptide synthesis to suppress racemization and enhance coupling efficiency. First introduced as a safer alternative to HOBt, Oxyma has become the preferred additive in large-scale and GMP peptide manufacturing due to its non-explosive character, excellent racemization suppression, and high solubility in common SPPS solvents. Its synergistic combination with DIC produces an in situ activated ester that reacts rapidly with the resin-bound amine while minimising enantiomeric erosion at the α-carbon of the incoming amino acid.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | Ethyl 2-cyano-2-(hydroxyimino)acetate |
| **CAS number** | 3849-21-6 |
| **Molecular formula** | C₅H₆N₂O₃ |
| **Molecular weight** | 142.11 g/mol |
| **Appearance** | White to off-white crystalline powder |
| **Melting point** | 140–145 °C (decomposes) |
| **pKa (oxime OH)** | ~4.8 |
| **Solubility in DMF** | >200 g/L (25 °C) |
| **Solubility in DCM** | ~30 g/L (25 °C) |
| **Solubility in water** | 8.8 g/L (20 °C) |
| **UV absorption (λmax)** | 274 nm (ε = 8,500 M⁻¹·cm⁻¹) |

## Mechanism of Action

Oxyma functions through the formation of an exceptionally stable active ester intermediate. When combined with a carbodiimide such as DIC, the carboxylic acid of the Fmoc-amino acid is rapidly converted to the corresponding O-acylisourea. In the absence of an auxiliary nucleophile, this O-acylisourea can undergo racemization via oxazolone formation or interconversion to the unreactive N-acylurea. Oxyma intercepts the O-acylisourea before these side reactions occur:

1. **DIC + Fmoc-AA-OH** → O-acylisourea (fast, <1 min)
2. **O-acylisourea + Oxyma** → Oxyma ester + diisopropylurea (fast)
3. **Oxyma ester + H₂N-peptide-resin** → peptide bond + Oxyma (rate-limiting, 30–60 min)

The Oxyma ester is kinetically competent—it reacts with amines at a comparable rate to HOBt esters—but the cyano-oxime structure confers an additional racemization-suppression effect by disfavouring oxazolone formation.

## Racemization Suppression Data

Comparative racemization levels across common coupling systems (measured by HPLC after segment coupling of Z-Gly-Phe-OH; racemization as % of D-Phe isomer):

| Coupling System | Racemization (%) | Notes |
|----------------|-----------------|-------|
| DIC alone | 8–14 | Unacceptable; oxazolone pathway dominant |
| DIC + HOBt (1:1) | 0.3–1.2 | Acceptable for most sequences |
| DIC + Oxyma (1:1) | 0.2–0.8 | Superior suppression, comparable to HOBt |
| DIC + HOAt (1:1) | 0.1–0.4 | Best suppression but high cost |
| HBTU/DIEA | 0.5–2.0 | Base-dependent; higher at elevated temperature |
| HATU/DIEA | 0.1–0.6 | Gold standard for hindered couplings |

Oxyma matches or exceeds HOBt in racemization suppression across all tested amino acid types. The improvement is most pronounced for Cys, His, and Ser derivatives where base-catalysed racemization pathways are most active.

## Compatibility Comparison — Oxyma vs. HOBt

| Feature | Oxyma | HOBt |
|---------|-------|------|
| Explosion hazard | None (DSC exotherm >250 °C) | Shock-sensitive at >5 g scale |
| Transportation restriction | None (not classified as explosive) | IATA Class 1 (explosive) for bulk |
| Shelf life (2–8 °C, anhydrous) | >2 years | >1 year |
| Solubility in DMF | >200 g/L | ~80 g/L |
| UV activity at 214 nm | Moderate | Moderate |
| Cost per mol | Moderate | Low |
| Byproduct after coupling | Cyano-oxime (benign) | Benzotriazole (potential irritant) |
| GMP compatibility | Yes (widely accepted) | Restricted at scale |
| Green chemistry rating | Excellent (no toxic metals) | Good |

## Recommended Usage Ratios

The standard protocol in Fmoc SPPS with DIC/Oxyma activation uses the following stoichiometry:

| Component | Equivalents (vs. resin loading) | Solvent | Time |
|-----------|-------------------------------|--------|------|
| Fmoc-amino acid | 3 eq | DMF (or DMF/DCM 1:1) | — |
| Oxyma | 3 eq | Same as amino acid solution | — |
| DIC | 3 eq | Added last, then vortex | — |
| Pre-activation | — | 2–5 min at RT | — |
| Coupling | — | — | 30–60 min |

**Variations by coupling difficulty:**

| Sequence Feature | Recommended Adjustment |
|-----------------|----------------------|
| Standard amino acid | 3 eq DIC + 3 eq Oxyma, 30 min |
| Sterically hindered (Aib, D-AA) | 5 eq DIC + 5 eq Oxyma, 60–90 min, 50 °C |
| After Arg(Pbf) coupling | Double coupling, 3+3 eq, 45 min each |
| β-branched (Ile, Val) | 4 eq, 60 min, monitor by Kaiser test |
| Long peptide (>30 AA) | Reduce to 2 eq to minimize deletion sequences |

## Handling and Storage

- **Storage:** 2–8 °C in a tightly sealed container, protected from moisture and light
- **Stability:** >2 years under recommended conditions; avoid prolonged exposure to air (hygroscopic)
- **Handling:** Normal laboratory PPE (gloves, safety glasses). No special explosion-proof precautions required
- **Solubility:** Prepare stock solutions in DMF (0.5–1.0 M); warm gently if crystals form
- **Disposal:** Aqueous waste acceptable; Oxyma byproducts are non-toxic and biodegradable

## Key Considerations for Process Development

- **Avoid excess DIC:** Using >3 eq DIC relative to the amino acid can promote N-acylurea formation. Maintain a 1:1 DIC:Oxyma molar ratio.
- **Monitor by TLC or HPLC:** Unreacted amino acid appears as a ninhydrin-negative spot but Oxyma may form coloured complexes — use Kaiser or chloranil test for primary amine detection.
- **Temperature sensitivity:** Oxyma decomposes above 150 °C. This is well above any SPPS process temperature but relevant for thermal analysis in scale-up safety assessments.
- **Resin compatibility:** Works equally well with all common SPPS resins (Wang, Rink Amide, 2-Cl-Trt, Sieber). No special resin pre-treatment required.

## Specifications for Procurement

| Grade | Purity | Water Content | Appearance | Typical Use |
|-------|--------|--------------|------------|-------------|
| Standard (for SPPS) | ≥99.0% | ≤0.5% | White powder | Routine coupling |
| High-purity (for GMP) | ≥99.5% | ≤0.1% | White crystalline | GMP manufacturing |
| ACS grade | ≥98.0% | ≤1.0% | Off-white | Research only |

---

> **🔗 Related:** [DIC](./dic.md) | [HBTU](./hbtu.md) | [Coupling Reagent Comparison](./coupling-reagent-comparison.md) | [Coupling Reaction](../process/coupling-reaction.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
