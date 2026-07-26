---
description: "DMF (N,N-dimethylformamide) — physical properties, solvent quality impact on SPPS, water sensitivity threshold, storage protocols, and comprehensive safety and hazard data for peptide synthesis."
---

# DMF — N,N-Dimethylformamide

## Primary Solvent for Fmoc Solid-Phase Peptide Synthesis

## Introduction

N,N-Dimethylformamide (DMF) is the workhorse solvent in Fmoc SPPS, serving as the medium for resin swelling, amino acid coupling, Fmoc deprotection, and inter-step washes. Its high polarity, excellent dissolving capacity for Fmoc-amino acids and activators, and compatibility with all common SPPS resins make it the default choice for both research-scale and GMP manufacturing. However, solvent quality—particularly water content and amine impurity levels—directly affects synthesis outcomes, and proper storage is essential to prevent degradation into dimethylamine (DMA), which competes with the peptide chain for activated amino acids.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | N,N-Dimethylformamide |
| **CAS number** | 68-12-2 |
| **Molecular formula** | C₃H₇NO |
| **Molecular weight** | 73.09 g/mol |
| **Boiling point** | 153 °C (at 1 atm) |
| **Melting point** | −61 °C |
| **Density** | 0.944 g/mL (25 °C) |
| **Dielectric constant (ε)** | 36.7 (25 °C) |
| **Dipole moment** | 3.82 D |
| **Viscosity** | 0.802 cP (25 °C) |
| **Flash point** | 58 °C (closed cup) |
| **Autoignition temperature** | 445 °C |
| **Vapour pressure** | 3.77 mmHg (25 °C) |
| **Refractive index** | 1.428 (nD²⁰) |
| **UV cutoff** | 270 nm |
| **Solubility in water** | Miscible in all proportions |
| **Hygroscopicity** | Strongly hygroscopic |

## Solvent Quality Impact on SPPS

The quality of DMF is one of the most underappreciated variables affecting SPPS yield and purity. Contaminants in low-grade or aged DMF introduce multiple failure modes:

| Contaminant | Source | Effect on SPPS | Threshold |
|-------------|--------|----------------|-----------|
| Water | Hygroscopic absorption from air | Hydrolyses activated esters; reduces coupling efficiency | >0.1% water causes measurable yield loss |
| Dimethylamine (DMA) | Thermal/photolytic decomposition of DMF | Competes for activated amino acids — produces N-methyl amide termination products | >50 ppm DMA causes detectable shortmers |
| Formic acid | Decomposition of DMF | Acidifies the reaction; can prematurely cleave acid-labile protecting groups | >100 ppm causes side reactions |
| Metal ions | Leaching from containers | Can catalyse racemisation at Cys and His | >1 ppm for Cu/Fe |

**Water sensitivity threshold:** DMF used for SPPS should have ≤0.05% water content (500 ppm). DMF with >0.1% water causes a measurable drop in coupling efficiency, particularly for DIC/Oxyma-activated couplings where the active ester is susceptible to hydrolysis. The effect is magnified with extended pre-activation times.

## Role in SPPS

| Function | Typical Volume | Duration | Details |
|----------|---------------|----------|---------|
| Resin pre-swelling | 10 mL/g resin | 15–30 min | Swells polystyrene resin to 4–6 mL/g; accelerates first coupling |
| Coupling solvent | 5–10 mL/g resin | 30–60 min | Dissolves Fmoc-amino acids (0.2–0.5 M) and activators |
| Fmoc deprotection | 5–10 mL/g resin | 2 × 5–15 min | Carrier for 20% piperidine in DMF |
| Wash after coupling | 5 × 5–10 mL/g resin | 30–60 s each | Removes excess reagents and byproducts |
| Wash after deprotection | 5 × 5–10 mL/g resin | 30–60 s each | Removes piperidine and dibenzofulvene adducts |
| Wash before DCM | 3 × 5–10 mL/g resin | 30 s each | Intermediates between DMF and DCM washes |

**Resin swelling values in different solvents for polystyrene (PS) and Tentagel (TG) resins:**

| Resin Type | DMF (mL/g) | DCM (mL/g) | NMP (mL/g) | MeOH (mL/g) |
|------------|-----------|-----------|-----------|------------|
| Wang (PS, 100–200 mesh) | 4–6 | 6–8 | 5–7 | 2–3 |
| Rink Amide (PS) | 5–7 | 7–9 | 5–7 | 2–3 |
| 2-Cl-Trt (PS) | 4–6 | 6–8 | 4–6 | 2–3 |
| Tentagel S RAM | 6–8 | 3–5 | 6–8 | 3–4 |

## Solvent Comparison for SPPS

| Property | DMF | NMP | DCM | DMAc |
|----------|-----|-----|-----|------|
| Dielectric constant (ε) | 36.7 | 32.2 | 9.1 | 37.8 |
| Toxicity | Teratogen (reproductive hazard) | Irritant (less toxic) | Carcinogen (suspected) | Irritant |
| Swelling of PS resin | Good | Good | Excellent | Good |
| API solubility | Excellent | Good | Poor | Excellent |
| Viscosity (cP, 25 °C) | 0.80 | 1.66 | 0.41 | 0.92 |
| Boiling point (°C) | 153 | 202 | 40 | 166 |
| Removal by vacuum | Slow | Very slow | Fast | Slow |
| Cost | Low | Moderate | Low | Moderate |
| Degradation product | DMA (nucleophile) | Methylamine (uncommon) | HCl (under light) | Dimethylamine |

## Handling and Safety

### Acute Toxicity Data

| Hazard | Classification | Limit value (workplace) |
|--------|---------------|------------------------|
| Reproductive toxicity | H360D (may damage the unborn child) | If inhaled or absorbed through skin |
| Acute toxicity (inhalation) | H332 | STEL: 30 ppm (15 min) |
| Skin absorption | H312 (harmful in contact with skin) | Absorbed with systemic effects |
| Eye irritation | H319 | Causes serious eye irritation |
| Flammability | Class 3 (flash point 58 °C) | Not classified as highly flammable |

### Safe Handling Practices

1. **Always use a fume hood** — DMF vapours are heavier than air and accumulate in low-lying areas
2. **Double gloves recommended** — nitrile gloves provide resistance for 15–30 min before breakthrough; use butyl rubber for extended handling
3. **Solvent-dispensing systems** — use closed-loop dispensing to prevent vapour release and moisture ingress
4. **Contamination monitoring** — test water content weekly by Karl Fischer titration; replace if >0.1%
5. **Container integrity** — use amber glass or HDPE containers; DMF degrades in UV light

## Storage Recommendations

| Parameter | Recommendation |
|-----------|---------------|
| Container | Tightly sealed amber glass or HDPE, ≤2.5 L for frequent use |
| Temperature | 15–25 °C, stable for >2 years if sealed |
| Inert atmosphere | Nitrogen or argon blanket recommended for long-term storage |
| Desiccant | Molecular sieves (3Å or 4Å) can be added but must be pre-dried |
| Avoid | PVC containers (DMF dissolves PVC); metal containers (leaching) |
| Lifetime after opening | 2–4 months in humid environments (>50% RH) |

**Monitoring degradation:** DMF decomposition to DMA accelerates at >50 °C and under UV exposure. Test by ninhydrin — a positive test indicates DMA contamination. For HPLC-grade DMF, monitor by UV absorbance at 270 nm (cutoff increases with DMA content).

## Waste Disposal

- Collect separately from halogenated solvent waste
- Incinerate at licensed facility (no chlorinated byproducts)
- Never mix with DCM or chloroform in waste containers (unpredictable exothermic reactions at elevated temperature)

---

> **🔗 Related:** [DCM](./dcm.md) | [Acetonitrile](./acetonitrile.md) | [Coupling Reaction](../process/coupling-reaction.md) | [Resin Comparison Guide](./resin-comparison-guide.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
