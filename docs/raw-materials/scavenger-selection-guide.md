---
description: "Scavenger selection guide for peptide cleavage — TIS, EDT, thioanisole, phenol, and water — with a scavenger × protecting group matrix for optimal side-reaction suppression."
---

# Scavenger Selection Guide for Peptide Cleavage

## Introduction

During TFA-mediated cleavage and deprotection of peptides from the solid support, the liberated protecting groups generate highly reactive carbocations and other electrophilic species. Without proper scavenging, these electrophiles alkylate sensitive amino acid side chains (Trp, Met, Cys, Tyr), producing irreparable damage to the target peptide. This guide explains the function of each common scavenger and provides a decision matrix for selecting the optimal cleavage cocktail.

## What Are Scavengers and Why Are They Necessary?

When TFA cleaves a protecting group (e.g., tBu generates isobutylene, Trt generates trityl cation, Pbf generates Pbf sulfonic acid), the released cation can:

1. **Alkylate Trp** — mono- and di-alkylated indole
2. **Alkylate Met** — S-alkylation at the thioether sulfur
3. **Alkylate Cys** — S-alkylation of the free thiol
4. **Alkylate Tyr** — O-alkylation of the phenol
5. **Re-form protecting groups** — re-protection of target peptide

Scavengers intercept these reactive species by acting as:
- **Hydride donors** — reduce carbocations to hydrocarbons
- **Nucleophiles** — trap cations as stable adducts
- **Acid stabilizers** — modulate TFA activity

## Common Scavengers

### Triisopropylsilane (TIS)

| Property | Value |
|----------|-------|
| **Type** | Silane hydride donor |
| **Boiling point** | 178 °C |
| **Typical concentration** | 2–5% (v/v) in TFA |
| **Cations trapped** | Trityl, tBu, Boc, Pbf |

TIS is the most popular silane-based scavenger. It acts as a hydride donor, reducing carbocations to the corresponding hydrocarbon. The trityl-TIS adduct (a colorless compound) is highly soluble in cleavage cocktails, avoiding the precipitation issues seen with older methods.

**Advantages:**
- Very good at trapping trityl and tBu cations
- Does not introduce sulfurous odors (unlike EDT)
- Compatible with most peptide sequences
- Volatile — easily removed during evaporation/N₂ blow-down

**Limitations:**
- Less effective for hard carbocations (e.g., from Tos or benzyl groups)
- Requires sufficient concentration (≥2.5% for Trt-heavy sequences)

### 1,2-Ethanedithiol (EDT)

| Property | Value |
|----------|-------|
| **Type** | Dithiol nucleophile |
| **Boiling point** | 144 °C |
| **Typical concentration** | 1–5% (v/v) in TFA |
| **Cations trapped** | tBu, Boc, Pbf, Trt |

EDT is a powerful dithiol nucleophile. It is particularly effective in preventing Pbf-related alkylation of Trp.

**Advantages:**
- Excellent at scavenging Pbf cations (best available)
- Very good for Trp protection during Arg(Pbf) deprotection
- Prevents Met oxidation

**Limitations:**
- Extremely unpleasant odor (mercaptan)
- Potential to form cyclic adducts with free thiols
- Can reduce disulfide bonds if present (use only after oxidation)
- Pungent smell persists in product if not fully removed

### Thioanisole

| Property | Value |
|----------|-------|
| **Type** | Thioether (sulfide) nucleophile |
| **Boiling point** | 193 °C |
| **Typical concentration** | 2.5–10% (v/v) in TFA |
| **Cations trapped** | Trt, Pbf, tosyl |

Thioanisole is a strong nucleophile that effectively traps "hard" carbocations.

**Advantages:**
- Excellent for low-TFA cleavage (Boc chemistry, unreactive PGs)
- Very effective for recalcitrant protecting groups
- Helps solubilize hydrophobic peptides in cleavage cocktail

**Limitations:**
- Potent odor
- Not volatile — can persist in the final product
- Can cause product coloration if insufficiently removed
- Less commonly needed for routine Fmoc SPPS

### Phenol

| Property | Value |
|----------|-------|
| **Type** | Phenolic nucleophile |
| **Melting point** | 40.5 °C |
| **Typical concentration** | 2–5% (w/v) in TFA |
| **Cations trapped** | Trt, tBu, benzyl |

Phenol is an underused but highly effective scavenger. It is especially valuable for protecting Trp from alkylation.

**Advantages:**
- Excellent protection of Trp indole ring
- Minimal odor
- Solid at room temperature — easy to handle
- Does not introduce new sulfur chemistry

**Limitations:**
- Must be warmed to melt before addition to TFA
- Less effective than EDT for Pbf-related alkylation
- Leaves a slight phenolic residue if not fully removed

### Water (H₂O)

| Property | Value |
|----------|-------|
| **Type** | Brønsted base / nucleophile |
| **Typical concentration** | 2–10% (v/v) in TFA |
| **Cations trapped** | tBu, Boc (as isobutylene) |

Water is the simplest and cheapest scavenger. It is always included in the standard Reagent R (TFA/TIS/H₂O 95:2.5:2.5).

**Advantages:**
- Cheap, non-toxic, no odor
- Universally compatible
- Never removed — compatible with lyophilization
- Essential for protonation of released groups

**Limitations:**
- Weak scavenger — insufficient as a sole scavenger for sequences containing Arg(Pbf) or Trt
- Cannot replace TIS or EDT for difficult sequences
- Excess water (≥10%) slows cleavage rate

## Scavenger × Protecting Group Matrix

The following table shows which scavengers effectively trap each protecting group:

| Protecting Group | Scavenger Effectiveness |
|-----------------|------------------------|
| | **TIS** | **EDT** | **Thioanisole** | **Phenol** | **H₂O** |
|-----------------|---------|---------|-----------------|------------|-------|
| **Trt** (Cys, Asn, Gln, His) | ★★★★★ | ★★★ | ★★★★ | ★★★ | ★★ |
| **tBu** (Ser, Thr, Tyr) | ★★★★ | ★★★ | ★★★ | ★★★ | ★★★ |
| **Boc** (Lys) | ★★★★ | ★★★ | ★★★ | ★★★ | ★★★ |
| **OtBu** (Asp, Glu) | ★★★★ | ★★★ | ★★★ | ★★★ | ★★★ |
| **Pbf** (Arg) | ★★★ | ★★★★★ | ★★★★ | ★★ | ★ |
| **Tos** (Arg, legacy) | ★ | ★★ | ★★★★ | ★★ | ★ |
| **Bzl** (Cys, Ser, Thr — Boc SPPS) | ★ | ★★ | ★★★★ | ★★ | ★ |
| **Mtt** (Lys, Cys) | ★★★★ | ★★★ | ★★★ | ★★★ | ★★ |
| **Aloc** (various) | ★ | ★ | ★ | ★ | ★ |

**Rating:** ★★★★★ = Excellent / ★ = Poor or ineffective

## Standard Cleavage Cocktail Formulations

| Cocktail Name | Composition | Best For |
|--------------|-------------|----------|
| **Reagent R** | TFA/TIS/H₂O (95:2.5:2.5) | Most standard peptides — standard, reliable |
| **Reagent B** | TFA/Phenol/H₂O/TIS (88:5:5:2) | Trp-containing peptides (phenol protects Trp) |
| **Reagent K** | TFA/Phenol/H₂O/TIS/EDT (82.5:5:5:2.5:5) | Arg(Pbf) + Trp-containing — most demanding sequences |
| **Reagent H** | TFA/Phenol/H₂O/EDT/Thioanisole (80.5:2.5:2.5:2.5:12) | Boc SPPS, high-risk sequences |
| **Reagent A** | TFA/Phenol/H₂O (95:2.5:2.5) | Simple peptides without sensitive AA |
| **TFA/TIS only** | TFA/TIS (97.5:2.5) | Peptides without Arg(Pbf) or Trp |

## Cleavage Cocktail Selection by Peptide Composition

| Peptide Contains | Recommended Cocktail | Rationale |
|-----------------|---------------------|-----------|
| **No sensitive residues** | Reagent R (TFA/TIS/H₂O) | Simple, effective, minimal cost |
| **Trp (but no Arg)** | Reagent B (add phenol) | Phenol prevents Trp alkylation |
| **Arg(Pbf) (but no Trp)** | Reagent R (with extended time) | 2–4 h cleavage; TIS sufficient for Pbf |
| **Trp + Arg(Pbf)** | Reagent K | EDT critical for Pbf-related Trp alkylation |
| **Cys (free thiol target)** | Reagent R (+ 2% EDT optional) | EDT prevents disulfide formation during cleavage |
| **Met** | Reagent R or B | Avoid oxidants; add 1% EDT if needed |
| **Trp + Met** | Reagent K or B + 1% EDT | Two susceptible residues need strong protection |
| **Multiple Trt groups** | Reagent R (2.5% TIS minimum) | Each Trt consumes 1 equivalent of TIS hydride |
| **Hexa-Arg sequences** | Reagent K | Heavy Pbf load requires maximum scavenging |
| **Protected peptide (Sieber/2-Cl-Trt)** | 1–5% TFA/DCM (no scavenger needed) | Side-chain PGs retained — no reactive species |

## Practical Guidelines

### Concentration Tuning

| Sequence Complexity | TIS | H₂O | EDT | Phenol | Cleavage Time |
|-------------------|-----|-----|-----|--------|---------------|
| Simple (<10 AA, no sensitive residues) | 2.5% | 2.5% | 0% | 0% | 1–1.5 h |
| Medium (Trp or Met present) | 2.5% | 5% | 0% | 3% | 1.5–2 h |
| Complex (Arg(Pbf) + Trp) | 2.5% | 5% | 5% | 5% | 2–4 h |
| Very complex (multiple Arg, Trp, Cys) | 2% | 5% | 5% | 5% | 3–5 h |

### Order of Addition

1. TFA (cold, 0 °C)
2. H₂O
3. TIS
4. EDT (if used — add last)
5. Phenol (solid — dissolve in TFA before other liquids)

### Workup After Cleavage

1. Filter to remove resin beads
2. Precipitate peptide in cold MTBE or Et₂O (10 volumes)
3. Centrifuge or filter
4. Wash 2–3× with cold Et₂O
5. Dissolve in water/ACN and lyophilize

**Scavenger removal during workup:**
- **TIS:** Volatile — mostly removed during N₂ blow-down and ether washes
- **EDT:** Partially removed by ether washes; residual odor may remain
- **Thioanisole:** Not volatile — requires extensive ether washing or preparative HPLC
- **Phenol:** Partially removed by ether; residual can be seen as a UV peak in HPLC

## Troubleshooting

| Problem | Likely Cause | Solution |
|---------|-------------|----------|
| Trp alkylation (observed by MS) | Insufficient scavenger for Arg(Pbf) | Switch from Reagent R to Reagent K |
| Met oxidation (M+16 by MS) | Oxidizing conditions during cleavage | Add 1% EDT; ensure inert atmosphere |
| Peptide precipitation during cleavage | Cocktail too non-polar | Add 2.5% H₂O; sometimes 5% thioanisole |
| Yellow peptide product | Trityl cation adducts | Increase TIS to 5%; extend cleavage time |
| Residual odor in product | EDT or thioanisole not fully removed | Additional ether washes; preparative HPLC |
| Low recovery | Peptide retained on resin | Extend cleavage time; check temperature |
| Cys dimerization | Air oxidation during workup | Include 1% EDT or 2% β-mercaptoethanol in precipitation |

## Key Recommendations

1. **Start with Reagent R** (TFA/TIS/H₂O 95:2.5:2.5) — it works for 70% of standard peptides
2. **Add phenol when Trp is present** — switch to Reagent B
3. **Add EDT when Trp + Arg(Pbf) are both present** — switch to Reagent K
4. **Never use less than 2% TIS** — insufficient TIS is the #1 cause of Trp and Met damage
5. **Always pre-cool TFA** before mixing to avoid exothermic fuming
6. **Test on 10–20 mg of resin-peptide** before committing the full batch

> **🔗 Related:** [Fmoc Amino Acid Side Chains](./fmoc-amino-acid-side-chains.md) | [Resin Comparison Guide](./resin-comparison-guide.md) | [Coupling Reagent Comparison](./coupling-reagent-comparison.md) | [Solvent Purity Guide](./solvent-purity-guide.md) | [Bulk Peptide Manufacturing & OEM Services](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
