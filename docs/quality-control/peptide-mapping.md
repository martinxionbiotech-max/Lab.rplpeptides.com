---
description: "Peptide mapping by HPLC-MS/MS — tryptic digestion, fragment analysis, and sequence confirmation for identity verification."
---

# Peptide Mapping

## Sequence Confirmation by HPLC-MS/MS

## Purpose

Peptide mapping confirms the primary sequence and detects sequence variants, post-translational modifications, and degradation products. It is the most definitive identity test for peptide therapeutics.

---

## Workflow

``` mermaid
flowchart LR
    A[Sample] --> B[Reduce & Alkylate];
    B --> C[Proteolytic Digestion];
    C --> D[HPLC Separation];
    D --> E[MS/MS Fragmentation];
    E --> F[Sequence Assignment];
    F --> G[Coverage Report];
```

---

## Proteolytic Enzymes

| Enzyme | Cleavage Site | Avg Fragment Length | Application |
|---|---|---|---|
| Trypsin | C-term of Lys, Arg | 5–15 AA | Standard mapping |
| Glu-C (V8) | C-term of Glu, Asp | 8–20 AA | Hydrophobic regions |
| Lys-C | C-term of Lys | 10–25 AA | Long peptides |
| Chymotrypsin | C-term of Phe, Tyr, Trp | 4–12 AA | Complementary coverage |
| Pepsin | Broad specificity | 3–10 AA | Acidic conditions |

---

## Digestion Protocol (Trypsin)

| Step | Condition | Duration |
|---|---|---|
| Denature | 6 M guanidine-HCl, pH 8.0 | 30 min |
| Reduce | 10 mM DTT, 56 °C | 30 min |
| Alkylate | 25 mM iodoacetamide, RT, dark | 30 min |
| Buffer exchange | 50 mM ammonium bicarbonate | — |
| Digestion | Trypsin 1:50 (w/w), 37 °C | 4–16 h |
| Quench | 0.1% TFA final | — |

---

## Sequence Coverage Targets

| Application | Target Coverage |
|---|---|
| Identity confirmation | ≥80% sequence coverage |
| Variant detection | ≥95% sequence coverage |
| Biosimilar comparability | ≥95% + 100% disulfide mapping |
| Release testing | Matches reference map |

---

## Data Interpretation

- **MS1**: Identify peptide mass → match predicted digest
- **MS/MS (CID/HCD)**: b/y ion series → confirm sequence
- **Coverage**: % of amino acids confirmed by MS/MS
- **Modifications**: +57 Da (carbamidomethyl Cys), +16 Da (Met oxidation)

> 🔗 Related: [LC-MS Testing](./lc-ms-testing.md) | [Mass Confirmation](./mass-confirmation.md) | [Peptide Quality Control Guide](https://rplpeptides.com/peptide-quality-control/)
