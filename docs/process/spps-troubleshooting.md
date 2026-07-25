---
description: "SPPS troubleshooting guide — common failures, root causes, and corrective actions for coupling, cleavage, and purification."
---

# SPPS Troubleshooting Guide

## Common Problems and Solutions

> **TL;DR:** Most SPPS failures fall into six categories: incomplete coupling, slow deprotection, cleavage damage, purification loss, HPLC artifacts, and low yield. Each has known root causes and proven corrective actions. The Kaiser test is the frontline diagnostic — positive (blue) after coupling means repeat the cycle. Chain aggregation is the most common hidden culprit for difficult sequences.

## Key Takeaways

- **Kaiser test positive** after coupling → increase activator eq, double couple, or add LiCl.
- **Deletion sequences** → capping is essential; use fresh piperidine.
- **Aspartimide** → use 5% HOBt in deprotection or switch to Asp(OMpe).
- **Low crude yield** → check cleavage scavenger system; extend cleavage time.
- **Broad HPLC peaks** → reduce column load by 50%; optimize gradient slope.
- **Poor peak shape** → check column condition and mobile phase pH.

## Coupling Problems

| Symptom | Likely Cause | Solution |
|---|---|---|
| **Kaiser test remains positive** | Insufficient activator | Increase to 5 eq AA + 5 eq activator |
| | Steric hindrance | Double couple, switch to HATU |
| | Chain aggregation | Add 0.4 M LiCl in DMF |
| | Resin inaccessible | Use lower-loading resin (0.3 mmol/g) |
| **Deletion sequences in final** | Missed coupling | Capping essential; check Kaiser |
| | Racemization | Use DIC/Oxyma, lower temperature |
| | Aspartimide | Use Asp(OMpe), 5% HOBt in deprotection |
| **Low crude yield** | Resin lost during handling | Use PTFE frit vessels |
| | Cleavage incomplete | Extend time, increase temperature |
| | Precipitation loss | Use more cold ether, centrifuge well |

---

## Deprotection Problems

| Symptom | Likely Cause | Solution |
|---|---|---|
| **Slow deprotection** | Degraded piperidine | Use fresh, store under N₂ |
| | N-terminal aggregation | Use chaotropic agents |
| | Trityl groups present | Separate deprotection step |
| **Aspartimide (Asp-Gly)** | Base exposure | 5% piperidine + 5% HOBt |
| | Asp(OtBu) protecting group | Switch to Asp(OMpe) |
| **Racemization at His/Cys** | Base sensitivity | Use HATU, reduce DIEA, cool |

---

## Cleavage Problems

| Symptom | Likely Cause | Solution |
|---|---|---|
| **Tert-butylation** | Insufficient scavenger | Add TIS; use EDT for Trp |
| **TFA adducts** | Scavenger system inadequate | Increase TIS/H₂O |
| **Residual protecting groups** | Cleavage incomplete | Extend time to 3-4 h |
| **Peptide precipitation fails** | Ether volume too low | 10× volume cold ether |
| | Wrong ether | Use methyl tert-butyl ether |

---

## Purification Problems

| Symptom | Likely Cause | Solution |
|---|---|---|
| **Broad peaks** | Column overload | Reduce load by 50% |
| | Poor gradient | Extend gradient, optimize slope |
| **Peptide won't elute** | Too hydrophobic | Increase organic, use IPA |  |
| | Aggregation | Add 0.1% TFA, warm column |
| **Low recovery** | Precipitation on column | Add organic wash step |
| | Irreversible binding | Regenerate column, check pH |

---

## HPLC QC Problems

| Symptom | Likely Cause | Solution |
|---|---|---|
| **Multiple peaks** | Degradation | Test fresh sample |
| | Disulfide scrambling | Reduce/alkylate before testing |
| | Impurities expected | Compare with reference |
| **Poor peak shape** | Column fouled | Regenerate/replace |
| | Wrong pH | Optimize mobile phase pH |

> 🔗 Related: [Coupling Reaction](../process/coupling-reaction.md) | [Cleavage](../process/cleavage.md) | [Purification](../process/purification.md) | [Difficult Sequences](../process/difficult-sequences.md)
