---
description: "DIC (N,N'-diisopropylcarbodiimide) — chemical properties, activation mechanism, coupling efficiency comparison with EDC, handling precautions, and recommended protocols for SPPS."
---

# DIC — N,N′-Diisopropylcarbodiimide

## Carbodiimide Coupling Reagent for Peptide Synthesis

## Introduction

N,N′-Diisopropylcarbodiimide (DIC) is a carbodiimide-based coupling reagent widely used in solid-phase peptide synthesis as part of the DIC/additive activation system. When used in combination with Oxyma, HOBt, or HOAt, DIC generates active esters that undergo aminolysis to form the peptide bond. DIC is distinct from other coupling reagents in three important ways: it is a liquid at room temperature (facilitating handling and stock solution preparation), it generates diisopropylurea (DIU) as a byproduct rather than tetramethylurea or other water-soluble ureas, and it requires no exogenous base for activation. These properties make DIC particularly attractive for green chemistry initiatives and large-scale GMP manufacturing.

## Chemical and Physical Properties

| Property | Value |
|----------|-------|
| **IUPAC name** | N,N′-Diisopropylmethanediimine |
| **CAS number** | 693-13-0 |
| **Molecular formula** | C₇H₁₄N₂ |
| **Molecular weight** | 126.20 g/mol |
| **Appearance** | Colourless to pale yellow liquid |
| **Boiling point** | 145–148 °C |
| **Melting point** | −44 °C |
| **Density** | 0.806 g/mL (20 °C) |
| **Refractive index** | 1.432 (nD²⁰) |
| **Flash point** | 37 °C (closed cup) |
| **Solubility in DMF** | Miscible |
| **Solubility in DCM** | Miscible |
| **Solubility in water** | Reacts (hydrolyses) |
| **Vapour pressure** | 3.8 mmHg (25 °C) |

## Mechanism of Carbodiimide Activation

The activation of a carboxylic acid by DIC proceeds through the following established pathway:

1. **O-Acylisourea formation (fast):** DIC reacts with the carboxyl group of the Fmoc-amino acid to form a highly reactive O-acylisourea intermediate within seconds.
2. **Racemisation risk (without additive):** The O-acylisourea can rearrange to the unreactive N-acylurea (a dead end) or undergo oxazolone formation (leading to racemisation). In the absence of an auxiliary nucleophile, racemisation levels of 8–14% are typical.
3. **Additive interception:** When Oxyma or HOBt is present, the auxiliary nucleophile attacks the O-acylisourea faster than the intramolecular rearrangement, forming a stable active ester.
4. **Aminolysis (rate-limiting):** The active ester reacts with the resin-bound amine over 30–60 minutes, regenerating the free auxiliary and producing the peptide bond. The byproduct diisopropylurea precipitates partially in DMF and is removed during washes.

## DIC vs. EDC — Comparison Table

| Feature | DIC | EDC (EDAC·HCl) |
|---------|-----|----------------|
| **CAS number** | 693-13-0 | 25952-53-8 (HCl salt) |
| **Physical form** | Liquid | White crystalline powder (HCl salt) |
| **Water solubility** | Immiscible, reacts with water | Water-soluble (as HCl salt) |
| **Byproduct** | Diisopropylurea (partially soluble in DMF/DCM) | 1-Ethyl-3-(3-dimethylaminopropyl)urea (water-soluble) |
| **Base required** | No | No (free base form); yes (HCl form — need 1 eq base) |
| **Coupling rate (with HOBt)** | Fast (30–60 min) | Moderate (60–90 min) |
| **Racemisation (with HOBt)** | 0.3–1.2% | 0.5–2.0% |
| **Cost per mole** | Very low | Low |
| **Storage stability** | Good (2–8 °C, >1 year) | Good (room temperature, desiccated) |
| **Solvent compatibility** | DMF, DCM, NMP, THF | Water, methanol, DMF |
| **Green chemistry** | Excellent | Good |
| **Preferred in SPPS** | Yes (most common carbodiimide) | No (rare in SPPS) |

## Coupling Efficiency: DIC/Additive vs. Aminium Salts

| Coupling System | Relative Coupling Rate | Racemisation | Cost per 100 Couplings (1 mmol scale) | Byproduct Removal |
|----------------|----------------------|-------------|--------------------------------------|-------------------|
| DIC + Oxyma (1:1:1) | Moderate (30–60 min) | Very low (0.2–0.8%) | <$5 | DIU removed by DMF/DCM washes |
| DIC + HOBt (1:1:1) | Moderate (30–60 min) | Low (0.3–1.2%) | <$5 | DIU + benzotriazole |
| HBTU + DIEA (1:1:2) | Fast (5–20 min) | Low–moderate (0.5–2.0%) | ~$15 | Tetramethylurea (water-soluble) |
| HATU + DIEA (1:1:2) | Very fast (5–15 min) | Very low (0.1–0.6%) | ~$80 | Tetramethylurea + pyridine byproducts |
| COMU + DIEA (1:1:2) | Fast (3–10 min) | Very low (0.2–0.5%) | ~$25 | Morpholine-based (water-soluble) |

**Key insight:** DIC + Oxyma offers the most economical system with racemisation performance comparable to HATU. It is preferred for scale-up operations and sequences where racemisation risk is a concern but cost control is also important.

## Handling Precautions

| Hazard | Classification | Risk | Precaution |
|--------|---------------|------|------------|
| Sensitiser | H317 (may cause allergic skin reaction) | Dermal sensitisation | Avoid skin contact; use nitrile gloves |
| Irritant — respiratory | H335 (may cause respiratory irritation) | Inhalation of vapours | Fume hood mandatory |
| Eye irritant | H319 (causes serious eye irritation) | Splash risk | Safety goggles or face shield |
| Flammable | H226 (flammable liquid) | Fire risk | Keep away from ignition sources |
| Water reactive | — | Hydrolyses exothermically | Keep container tightly sealed |

**Special handling note:** DIC is a known sensitiser. Once sensitised, even trace contact can trigger a dermal reaction. Use double gloves and change them after significant handling.

## Recommended Protocols

### Standard DIC/Oxyma Protocol

| Step | Detail |
|------|--------|
| Dissolve Fmoc-AA-OH (3 eq) in DMF (0.3–0.5 M final) | 2–3 mL DMF per mmol |
| Add Oxyma (3 eq) | 426 mg per mmol |
| Add DIC (3 eq, 3.0 M in DMF) | Equimolar to Oxyma |
| Pre-activate | 2–5 min, room temperature |
| Add to resin | 30–60 min, room temperature (or 50 °C for hindered couplings) |
| Wash | 5 × DMF at 30 s each |
| Monitor | Kaiser test (ninhydrin — negative = coupling complete) |

### Double Coupling Protocol (for Difficult Sequences)

1. First coupling cycle as above
2. Drain, wash 3× with DMF
3. Repeat activation with fresh Fmoc-AA-OH + Oxyma + DIC
4. Couple for 60 min
5. Wash 5× with DMF

## Storage

- **Short-term:** 2–8 °C in a tightly sealed container, protected from moisture
- **Long-term:** −20 °C for >6 months storage
- **Container:** Glass or HDPE; avoid metal containers (catalytic decomposition)
- **Purity check:** DIC should be colourless. Yellowing indicates decomposition (oligomeric carbodiimide or urea formation). Discard if colour change is observed.

---

> **🔗 Related:** [Oxyma](./oxyma.md) | [HBTU](./hbtu.md) | [Coupling Reagent Comparison](./coupling-reagent-comparison.md) | [Coupling Reaction](../process/coupling-reaction.md) | [Custom Peptide Synthesis — Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
