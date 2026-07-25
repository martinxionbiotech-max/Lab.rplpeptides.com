---
description: "Cyclic peptide synthesis — head-to-tail and side-chain-to-side-chain cyclization strategies, on-resin vs. in-solution methods."
---

# Cyclic Peptide Synthesis

## TL;DR

Cyclization constrains peptide structure, improving metabolic stability, receptor binding affinity, and selectivity. Two main approaches dominate: head-to-tail (N-terminus to C-terminus) amide cyclization and side-chain-to-side-chain (lactam or disulfide) cyclization. On-resin cyclization offers purification advantages; in-solution cyclization allows higher dilution control to minimize oligomerization.

---

## Why Cyclize?

| Benefit | Explanation | Example Peptide |
|---|---|---|
| Metabolic stability | Cyclic peptides resist exopeptidases | Octreotide |
| Conformational constraint | Reduced entropy penalty on binding | Cyclosporine A |
| Improved selectivity | Fixed conformation discriminates receptor subtypes | Vasopressin analogs |
| Membrane permeability | Cyclization reduces charge and H-bond donors | Cyclic RGD peptides |
| Oral bioavailability | More stable, cell-permeable | Cyclosporine, Gramicidin S |

---

## Cyclization Chemistries

### Head-to-Tail Amide Cyclization

The N-terminus amine couples to the C-terminus carboxylic acid to form an amide bond.

| Parameter | On-Resin | In-Solution |
|---|---|---|
| Dilution | 0.05–0.1 M (limited by resin) | 0.1–1 mM (high dilution to avoid oligomers) |
| Activator | DIC/Oxyma, HATU/DIEA | HATU/DIEA, PyBOP/DIEA, DPPA/NaHCO₃ |
| Temperature | RT | RT to 50 °C |
| Time | 1–4 h | 2–24 h |
| Monitoring | Kaiser test | TLC, HPLC |
| Yield range | 50–85% | 40–80% |
| Purity | Generally higher | Requires purification from oligomers |

**Key challenge**: The intramolecular ring closure competes with intermolecular oligomerization. High dilution (0.1–1 mM for solution, 0.05 M for on-resin) suppresses dimers and trimers.

### Side-Chain-to-Side-Chain Cyclization (Lactam)

Forms a bridge between two amino acid side chains — commonly Lys (ε-NH₂) to Glu/Asp (γ/β-COOH).

| Bridge Type | Amino Acid 1 | Amino Acid 2 | Protecting Group Strategy |
|---|---|---|---|
| Lys–Asp lactam | Lys(Alloc) | Asp(OAll) | Alloc/Allyl orthogonal deprotection |
| Lys–Glu lactam | Lys(Alloc) | Glu(OAll) | Alloc/Allyl orthogonal deprotection |
| Orn–Asp lactam | Orn(Alloc) | Asp(OAll) | Shorter bridge, tighter constraint |
| Dab–Asp lactam | Dab(Alloc) | Asp(OAll) | Minimal bridge length |

**Protocol for Lys–Glu lactam**:
1. Synthesize full sequence with Lys(Alloc) and Glu(OAll)
2. Selectively deprotect: Pd(PPh₃)₄ (0.1 eq) + PhSiH₃ (10 eq) in DCM (15 min × 2)
3. Wash with DCM, DMF, 0.5% DIEA/DMF, 0.5% DEDTC/DMF
4. Cyclize on-resin: HATU (3 eq) + DIEA (6 eq) in DMF, 2 h
5. Global deprotection and cleavage

### Disulfide Cyclization

Head-to-tail disulfides (Cys-N to Cys-C) are the simplest form. See [Disulfide Bridge Strategies](./disulfide-bridge-strategies.md) for detailed protocols.

---

## On-Resin vs. In-Solution Cyclization

| Factor | On-Resin | In-Solution |
|---|---|---|
| Dilution effect | Pseudo-dilution by resin reduces oligomers | Requires 0.1–1 mM concentration |
| Purification | Wash away side products | Chromatography needed |
| Yield | 50–85% | 40–80% (lower at small scale) |
| Scalability | Limited by resin loading | Better at larger scale |
| Monitoring | Kaiser or chloranil test | HPLC, TLC |
| Best ring sizes | 5–12 AA | 5–20+ AA |
| Equipment | Standard SPPS reactor | Slow addition pump may be needed |

---

## Cyclization Methods and Typical Yields

| Method | Conditions | Ring Size | Typical Yield | Notes |
|---|---|---|---|---|
| HATU/DIEA (solution) | 0.5 mM, DMF, RT, 4 h | 5–12 | 60–80% | Most common for solution |
| PyBOP/DIEA (solution) | 0.5 mM, DMF/DCM, RT | 5–14 | 55–75% | Alternative to HATU |
| DPPA/NaHCO₃ (solution) | 1 mM, DMF, 0 °C → RT | 6–14 | 50–70% | Low racemization |
| EDC/HOAt (solution) | 1 mM, DCM, RT | 5–10 | 50–65% | Water-soluble byproducts |
| DIC/Oxyma (on-resin) | 0.1 M, DMF, RT, 4 h | 5–10 | 60–85% | Minimal racemization |
| HATU/DIEA (on-resin) | 0.1 M, DMF, RT, 2 h | 5–12 | 55–80% | Faster, racemization possible |
| COMU/collidine (on-resin) | 0.1 M, DMF, RT, 1 h | 5–10 | 65–85% | Fast, low epimerization |

---

## Practical Cyclization Decision Tree

```
Is the peptide ≤12 AA?
├── Yes → On-resin cyclization preferred
│   └── Use DIC/Oxyma for amide; I₂ for disulfide
└── No → In-solution preferred
    ├── Can you add a solubilizing tag at C-terminus?
    │   ├── Yes → On-resin with tag, cleave, cyclize, remove tag
    │   └── No → High-dilution solution cyclization
```

---

## Characterization of Cyclic Peptides

| Method | What It Confirms |
|---|---|
| LC-MS | Mass shift: −18 Da per amide bond formed (H₂O loss) |
| MS/MS fragmentation | Sequencing confirms cyclization site |
| NMR (1D/2D) | Conformational homogeneity |
| HPLC retention shift | Cyclic peptides elute differently from linear |
| Ellman's test | Free thiols absent (disulfide cyclization) |

---

## Key Takeaways

- Cyclization improves metabolic stability, binding affinity, and conformational control
- Head-to-tail lactamization: solution method for ≤1 mM, on-resin for pseudo-dilution advantage
- Side-chain bridging (Lys–Glu lactam, disulfide) requires orthogonal protection (Alloc/Allyl or Trt/Acm)
- On-resin cyclization yields 60–85% with DIC/Oxyma; solution yields 50–80% with HATU/DIEA
- High dilution in solution is critical — use slow addition pumps for scales >100 mg
- Characterization requires LC-MS mass confirmation + MS/MS for regiochemistry

> 🔗 Related: [Disulfide Bridge Strategies](./disulfide-bridge-strategies.md) | [Coupling Reaction](./coupling-reaction.md) | [On-Resin Modifications](./on-resin-modifications.md) | [Custom Synthesis](./custom-synthesis.md) | [Peptide Folding](./peptide-folding.md) | [Protecting Group Strategies](../manufacturing/protecting-group-strategies.md)
