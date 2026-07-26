---
description: "DCM (dichloromethane) — physical properties, role in resin swelling, washing and cleavage in SPPS, chlorinated solvent handling protocols, and comprehensive safety data."
---

# DCM — Dichloromethane

## Resin Swelling, Wash, and Cleavage Cocktail Solvent

## Introduction

Dichloromethane (DCM, methylene chloride) is the second most frequently used solvent in solid-phase peptide synthesis, after DMF. Its unique combination of properties — exceptional swelling of polystyrene-divinylbenzene (PS-DVB) resins, low viscosity for efficient washing, volatility for rapid solvent removal, and chemical inertness under SPPS conditions — makes it indispensable for several key operations. DCM excels as a pre-swelling solvent before the first coupling, as an intermediate wash solvent to bridge between DMF and other solvents, and as a carrier or diluent in cleavage cocktails. Its lower polarity compared to DMF also makes it the preferred medium for coupling reactions involving hydrophobic sequences or when aggregation must be reduced.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | Dichloromethane |
| **CAS number** | 75-09-2 |
| **Molecular formula** | CH₂Cl₂ |
| **Molecular weight** | 84.93 g/mol |
| **Boiling point** | 39.6 °C (at 1 atm) |
| **Melting point** | −96.7 °C |
| **Density** | 1.326 g/mL (20 °C) |
| **Dielectric constant (ε)** | 9.08 (25 °C) |
| **Dipole moment** | 1.60 D |
| **Viscosity** | 0.413 cP (25 °C) |
| **Refractive index** | 1.423 (nD²⁰) |
| **Flash point** | None (non-flammable in closed cup test) |
| **Vapour pressure** | 436 mmHg (25 °C) |
| **Vapour density** | 2.93 × air (heavier than air) |
| **Solubility in water** | 13 g/L (20 °C) |
| **Solubility of water in DCM** | 1.5 g/L (20 °C) |
| **Electrical conductivity** | Very low (4.3 × 10⁻¹¹ S/m) |
| **Evaporation rate (BuAc=1)** | 14.5 (very fast) |

## Role in SPPS

### Resin Swelling

DCM produces the highest swelling volume for standard polystyrene-based SPPS resins, which is critical for achieving optimal reaction kinetics in SPPS:

| Resin Type | Swelling in DCM (mL/g) | Swelling in DMF (mL/g) | Ratio (DCM/DMF) |
|------------|----------------------|----------------------|-----------------|
| Wang resin (100–200 mesh) | 6–8 | 4–6 | 1.4–1.6× |
| Rink Amide (100–200 mesh) | 7–9 | 5–7 | 1.3–1.5× |
| 2-Cl-Trt (100–200 mesh) | 6–8 | 4–6 | 1.3–1.6× |
| PAM resin (Boc chemistry) | 6–8 | 4–5 | 1.5–1.7× |
| Sieber resin | 6–8 | 4–6 | 1.4–1.5× |

**Pre-swelling protocol:** Suspend dry resin in DCM (10 mL/g) for 15–30 min before the first DMF coupling. The swollen resin provides maximum solvent-accessible surface area for the initial, most critical coupling step. DCM is then exchanged for DMF through a series of DCM → DMF/DCM 1:1 → DMF washes (3 × 10 seconds each).

### Washing

DCM serves as an intermediate wash solvent between DMF-based coupling and deprotection cycles:

| Wash Step | Solvent | Volume | Duration | Purpose |
|-----------|---------|--------|----------|---------|
| After coupling | DMF | 5 × 5–10 mL/g | 30 s each | Remove excess reagents |
| Transition | DMF → DMF/DCM → DCM | 3 × 5 mL/g | 15 s each | Gradient polarity change |
| After Fmoc deprotection | DMF | 5 × 5–10 mL/g | 30 s each | Remove piperidine/DMF |
| Final resin wash | DCM then MeOH | 3 × 5 mL/g each | 30 s each | Prepare for drying/storage |
| Before HF cleavage (Boc) | DCM | 3 × 10 mL/g | 30 s each | Remove residual DMF and acetic acid |

### Cleavage Cocktail Component

DCM is used as a diluent in cleavage cocktails, primarily in two scenarios:

| Application | DCM Concentration | Purpose |
|------------|-------------------|---------|
| Boc deprotection wash | 50% TFA/DCM | Carrier for acidic deprotection cocktail |
| Protected peptide cleavage (Sieber/2-Cl-Trt) | 95–99% DCM + 1–5% TFA | Mild acidolysis retaining side-chain PGs |
| Pre-HF resin swelling (Boc SPPS) | 100% DCM | Ensure HF access to all peptide-resin bonds |
| HF cleavage cocktail diluent | 10% DCM + 10% p-cresol + 80% HF | Diluent/viscosity modifier for HF |

### Aggregation Reduction

DCM's lower polarity (ε = 9.08 vs. 36.7 for DMF) helps disrupt peptide chain aggregation during difficult couplings. For sequences with high aggregation propensity (β-sheet-prone, hydrophobic, or long sequences), coupling in DMF/DCM mixtures (1:1 to 1:3, v/v) can improve yields by:

- Reducing inter-chain hydrogen bonding through lower solvent polarity
- Improving resin solvation in hydrophobic domains
- Increasing diffusion rates of activated amino acids (lower viscosity)

## Chlorinated Solvent Handling — Special Considerations

DCM requires distinct handling protocols compared to non-chlorinated SPPS solvents:

| Property | Handling Implication |
|----------|---------------------|
| **Heavier than air** | Vapour accumulates in low-lying areas (under fume hood counters, pits) — cannot be detected by standard overhead vapour monitors |
| **Low boiling point (39.6 °C)** | Evaporates rapidly at room temperature; 15 min open exposure evaporates 70% of a 10 cm² surface |
| **PVC incompatibility** | DCM dissolves PVC tubing, gloves, and container linings — use HDPE, PTFE, or glass |
| **Light sensitivity** | DCM slowly photolyses to HCl and phosgene under intense UV/sunlight — store in amber or opaque containers |
| **Phase behaviour** | DCM forms a dense lower layer with water — organic layer is always the bottom phase |

## Safety Data

### Health Hazards

| Hazard | Classification | Workplace Limit | Chronic Effect |
|--------|---------------|----------------|----------------|
| Carcinogenicity | H350 (suspected of causing cancer — IARC Group 2A) | TWA: 25 ppm (8 h); STEL: 50 ppm (15 min) | Increased risk of brain, lung, and liver cancer |
| Acute toxicity (inhalation) | H332 (harmful if inhaled) | 25 ppm TWA | Drowsiness, dizziness, impaired coordination |
| Skin irritation | H315 (causes skin irritation) | — | Defatting of skin, dermatitis with repeated exposure |
| Eye irritation | H319 (causes serious eye irritation) | — | Reversible; conjunctival redness |
| CNS depression | H336 (may cause drowsiness/dizziness) | Effects detectable from 200 ppm | Narcotic effect at high concentrations |
| Metabolite | — | — | Metabolised to CO (detectable in exhaled breath) |

**Metabolic carboxyhaemoglobin:** DCM is metabolised in the liver to carbon monoxide, producing measurable increases in blood COHb levels. After exposure to 100 ppm for 2 hours, COHb levels rise to 3–4%. Individuals with cardiovascular conditions are particularly susceptible to this effect.

### Chemical Hazards

| Scenario | Reaction | Risk |
|----------|----------|------|
| DCM + strong base (NaOH, KOH) | Hydrolysis to formaldehyde + HCl | Exothermic; generates reactive intermediates |
| DCM + strong oxidisers (HNO₃, perchloric acid) | Potentially explosive oxidation | May produce phosgene (COCl₂) |
| DCM + TFA (under basic conditions) | Explosive diazomethane-like intermediates | **Extremely hazardous** — see TFA waste disposal note |
| DCM + Al/Li metal | Alkylation of metal surface | Fire risk with finely divided metals |
| DCM + dimethyl sulfoxide (DMSO) with TFA | Pummerer rearrangement | Exothermic; produces toxic gases |
| DCM photolysis | HCl + phosgene + chlorine | Occurs in strong UV light; avoid exposure |

### Handling Best Practices

1. **Fume hood mandatory** — DCM evaporates too rapidly for any open-bench work
2. **Nitril or neoprene gloves** — butyl rubber offers slightly better breakthrough time (>30 min); natural rubber is rapidly dissolved
3. **No PVC equipment** — DCM dissolves PVC in seconds; use HDPE, PTFE, or glass containers
4. **Container sealing** — Vapour emissions from unsealed containers exceed OSHA PEL within minutes in a standard laboratory
5. **Carbon monoxide monitoring** — Consider CO monitoring for personnel handling DCM daily (>2 h/day) at scale
6. **Avoid heating** — Heating DCM accelerates vapourisation and decomposition; use sealed systems with condensers if heating is required

## Waste Disposal

- Collect as **halogenated solvent waste** — never mix with acetone or non-halogenated waste
- Environmental regulation: DCM is an ozone-depletion substance precursor under the Montreal Protocol (Class III ODS in Europe)
- Disposition: Incineration at licensed hazardous waste facility with HCl scrubber
- Ship in clearly labelled, sealed HDPE containers; fill level ≤80% (vapour pressure)

---

> **🔗 Related:** [DMF](./dmf.md) | [Resin Loading](../process/resin-loading.md) | [SPPS Process](../process/spps-process.md) | [TFA](./tfa.md) | [Scavenger Selection Guide](./scavenger-selection-guide.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
