---
description: "Capping (acetylation) strategies in SPPS — reagents, protocols, and impact on final peptide purity by preventing deletion sequences."
---

# Capping Strategies

## TL;DR

Capping acetylates unreacted N-terminal amines after each coupling cycle to prevent deletion sequences from propagating. The standard reagent is acetic anhydride/DIEA in DMF. Capping is one of the most cost-effective steps for improving crude peptide purity, particularly in long or difficult sequences.

---

## Why Cap?

In SPPS, each coupling cycle aims for 100% efficiency, but in practice efficiencies range from 98.0% to 99.8%. Without capping, the 0.2–2% of chains that fail to couple at each position produce deletion sequences that are extremely difficult to separate from the target peptide during purification.

| Cycle Efficiency | Purity After 20 Cycles (uncapped) | Purity After 20 Cycles (capped) |
|---|---|---|
| 99.5% | 90.5% | ~99.5% (deletion sequences truncated) |
| 99.0% | 81.8% | ~99.0% |
| 98.0% | 66.8% | ~98.0% |
| 95.0% | 35.8% | ~95.0% |

Capping shifts the impurity profile from near-homologue deletion sequences (hard to purify) to short, capped truncation fragments (easy to remove by HPLC).

---

## Standard Capping Protocol

### Reagent Composition

| Component | Concentration | Function |
|---|---|---|
| Acetic anhydride (Ac₂O) | 5–10% v/v in DMF | Acetylating agent |
| DIEA (N,N-diisopropylethylamine) | 5–10% v/v in DMF | Base catalyst |
| DMF | Balance | Solvent |

### Procedure

1. After coupling and DMF washes, add capping solution
2. React 5–15 minutes at room temperature
3. Drain and wash with DMF (×3)
4. Proceed to Fmoc deprotection

### Alternative Capping Protocols

| Protocol | Reagent | Time | Notes |
|---|---|---|---|
| Standard | Ac₂O/DIEA/DMF (1:1:8) | 10 min | General purpose |
| Fast | Ac₂O/DIEA/DMF (1:1:3) | 5 min | Accelerated, use for routine automation |
| Mild | Ac₂O/NMM/DMF (1:2:17) | 15 min | NMM (N-methylmorpholine) alternative base |
| Extended | Ac₂O/DIEA/DMF (1:1:8) | 30 min | Difficult sequences, hydrophobic regions |

---

## Capping vs. No-Capping: Impact on Final Purity

The effect of capping is most dramatic in longer peptides where cumulative coupling inefficiencies compound.

| Peptide Length | No Capping — Crude Purity | Capped — Crude Purity | Improvement |
|---|---|---|---|
| 10 AA | 88–94% | 92–97% | +2–5% |
| 15 AA | 78–88% | 85–94% | +5–10% |
| 20 AA | 65–80% | 78–92% | +8–15% |
| 30 AA | 45–65% | 65–85% | +15–25% |

Purification yield improves proportionally. A crude purity increase from 70% to 85% can reduce prep-HPLC time by 40–60% and improve final recovery by 2–3×.

---

## Special Capping Considerations

### Acetylation of Side-Chains
Acetic anhydride can acetylate unprotected Ser, Thr, and Tyr hydroxyl groups. This is reversed during TFA cleavage, so it is generally not a concern for standard Fmoc synthesis.

### Capping with Alternative Reagents

| Reagent | Reactivity | Byproduct | Use Case |
|---|---|---|---|
| Acetic anhydride/DIEA | High | Acetic acid | Standard |
| Acetyl chloride/DIEA | Very high | HCl | Rapid capping |
| N-Acetylimidazole | Moderate | Imidazole | Mild conditions |
| (Boc)₂O (Boc-anhydride) | Moderate | CO₂, tBuOH | When acetyl is undesirable |

### Capping of Proline
Proline (secondary amine) requires longer capping times — 20–30 minutes with standard Ac₂O/DIEA.

---

## Integration into Automated Synthesis

Most commercial peptide synthesizers include a capping step in each cycle. A typical automated cycle:

```
1. Deprotect (20% piperidine/DMF, 2 + 10 min)
2. Wash (DMF × 4)
3. Couple (activator + amino acid, 30–60 min)
4. Wash (DMF × 3)
5. Cap (Ac₂O/DIEA/DMF, 10 min)
6. Wash (DMF × 3)
```

Capping adds approximately 15 minutes per cycle. For a 20-mer, this adds ~5 hours to total synthesis time — a small investment for dramatically better crude purity.

---

## When to Skip Capping

Capping can be omitted for:
- Very short peptides (<8 AA) with high coupling efficiency
- Sequences where the target is already ≥95% crude purity
- Cost-sensitive large-scale production where purification is economical
- Special applications where free N-terminal amines are desired for all truncation products

---

## Key Takeaways

- Capping acetylates unreacted N-terminal amines after each coupling, preventing deletion sequence propagation
- Standard reagent: 5–10% acetic anhydride + 5–10% DIEA in DMF, 10 min reaction
- Purity improvement of 8–25% for peptides over 15 AA
- Adds ~15 min per cycle but dramatically reduces purification burden
- Most beneficial for long sequences, difficult couplings, and high-purity requirements

> 🔗 Related: [Coupling Reaction](../process/coupling-reaction.md) | [Difficult Sequences](../process/difficult-sequences.md) | [Manufacturing Workflow](./manufacturing-workflow.md) | [Deprotection](../process/deprotection.md) | [Impurity Profiling](../quality-control/impurity-profiling.md)
