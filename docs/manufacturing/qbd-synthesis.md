---
description: "Quality by Design (QbD) for SPPS — critical process parameters, Design of Experiments for coupling optimization, and risk assessment."
---

# Quality by Design (QbD) in Peptide Synthesis

## TL;DR

QbD is a systematic approach to peptide manufacturing that defines quality targets upfront, maps critical process parameters (CPPs), and uses Design of Experiments (DoE) to build robustness into the process rather than testing quality into the final product. For SPPS, QbD focuses on identifying which coupling, deprotection, and purification variables most impact final purity.

---

## The QbD Framework for SPPS

The ICH Q8–Q11 framework applies directly to peptide manufacturing:

| QbD Element | SPPS Application |
|---|---|
| **QTPP** (Quality Target Product Profile) | Purity ≥98%, correct mass, specified content, defined impurity profile |
| **CQA** (Critical Quality Attributes) | Purity, identity, content, endotoxin, residual solvents, microbial limits |
| **CPP** (Critical Process Parameters) | Coupling time, temperature, reagent excess, deprotection time, wash volume |
| **CMA** (Critical Material Attributes) | Amino acid purity, resin loading, activator quality, solvent grade |
| **Design Space** | Proven acceptable ranges for temperature, excess, and time |
| **Control Strategy** | In-process tests (Kaiser, UV), hold points, release testing |
| **RTRT** (Real-Time Release Testing) | In-line UV monitoring, PAT-based release |

---

## Critical Process Parameters in SPPS

| Process Step | CPPs | Impact on CQA | Risk Level |
|---|---|---|---|
| Resin loading | Temperature, time, DMAP eq | Loading capacity, initial purity | Medium |
| Coupling | Amino acid eq, activator eq, time, temp, concentration | Deletion sequences, epimerization | High |
| Deprotection | Piperidine %, time, washes | Aspartimide formation, Fmoc removal | High |
| Capping | Ac₂O eq, time | Truncated impurities | Medium |
| Cleavage | TFA %, time, scavenger selection | Side-chain deprotection, peptide degradation | High |
| Purification | Gradient slope, flow rate, load | Purity, recovery | High |

---

## Design of Experiments (DoE) for Coupling Optimization

A well-designed DoE identifies which factors matter and their interactions.

### Example: 2³ Full Factorial for a Difficult Coupling

**Factors:**
- A: Amino acid excess (2 eq vs. 4 eq)
- B: Coupling time (30 min vs. 60 min)
- C: Temperature (25 °C vs. 50 °C)

**Response:** Coupling efficiency by UV tracking (%)

| Run | A (eq) | B (min) | C (°C) | Efficiency (%) |
|---|---|---|---|---|
| 1 | 2 | 30 | 25 | 96.2 |
| 2 | 4 | 30 | 25 | 98.1 |
| 3 | 2 | 60 | 25 | 97.0 |
| 4 | 4 | 60 | 25 | 98.8 |
| 5 | 2 | 30 | 50 | 97.8 |
| 6 | 4 | 30 | 50 | 99.2 |
| 7 | 2 | 60 | 50 | 98.5 |
| 8 | 4 | 60 | 50 | 99.5 |

**Analysis:**
- Main effects: A (most significant), C (significant), B (moderate)
- Interaction A×C: Higher temperature reduces the benefit of higher excess
- Optimum: 4 eq, 60 min, 50 °C — but 4 eq, 30 min, 50 °C gives 99.2%, nearly equivalent

---

## Risk Assessment Matrix for SPPS

A Failure Mode and Effects Analysis (FMEA) approach.

| Process Step | Failure Mode | Effect | Severity (1–5) | Occurrence (1–5) | Detectability (1–5) | RPN |
|---|---|---|---|---|---|---|
| Coupling | Inefficient activation | Deletion sequences | 5 | 3 | 2 | 30 |
| Coupling | Activator degradation | Low coupling efficiency | 4 | 2 | 3 | 24 |
| Deprotection | Incomplete Fmoc removal | Double-hit truncation | 5 | 2 | 2 | 20 |
| Deprotection | Aspartimide formation | Side product | 4 | 3 | 3 | 36 |
| Capping | Insufficient reagent | Uncapped deletions | 3 | 2 | 2 | 12 |
| Cleavage | Insufficient scavenger | Alkylation of Trp/Met/Cys | 5 | 2 | 3 | 30 |
| Purification | Column overload | Low resolution | 4 | 3 | 2 | 24 |
| Lyophilization | Incomplete drying | High residual moisture | 3 | 2 | 1 | 6 |

**RPN = Severity × Occurrence × Detectability** (higher = higher priority for mitigation)

---

## Design Space Definition

The design space is the multidimensional combination of process parameters proven to deliver acceptable quality.

### Example Design Space: Fmoc Deprotection

| Parameter | Proven Acceptable Range (PAR) | Normal Operating Range (NOR) |
|---|---|---|
| Piperidine concentration | 10–30% in DMF | 20% |
| Stage 1 deprotection time | 2–5 min | 3 min |
| Stage 2 deprotection time | 8–20 min | 12 min |
| Wash volume (per wash) | 5–15 mL/g resin | 10 mL/g resin |
| Number of washes | 3–6 | 4 |

Operating outside the PAR requires a post-approval change submission (for GMP). Operating within the NOR is routine.

---

## Control Strategy for SPPS

### In-Process Controls (IPC)

| Control | Method | Frequency | Acceptance Criteria |
|---|---|---|---|
| Fmoc removal | UV at 301 nm | Every cycle | Consistent with theoretical |
| Coupling completion | Kaiser test | Every cycle | Negative (yellow) |
| Resin loading | UV quantitation | Start + end | ±10% of target |
| Crude purity | HPLC | Per batch | ≥70% (typical) |
| pH of cleavage solution | pH strip | Per batch | ≤1 |

### Material Attribute Control

- **Amino acids**: HPLC purity ≥99%, chiral purity ≥99.5% ee
- **Resin**: Lot-to-lot consistency within ±0.05 mmol/g loading
- **Solvents**: Water content <0.02% for DMF, <50 ppm for DCM

---

## Key Takeaways

- QbD defines quality targets before process development begins
- For SPPS, coupling and deprotection are the highest-risk process steps
- DoE efficiently identifies critical parameters and their interactions
- A risk assessment matrix (FMEA) highlights where process control is most needed
- The design space (PAR + NOR) provides operational flexibility without compromising quality
- In-process controls (UV tracking, Kaiser tests) ensure real-time quality assurance

> 🔗 Related: [Coupling Reaction](../process/coupling-reaction.md) | [Deprotection](../process/deprotection.md) | [Manufacturing Workflow](./manufacturing-workflow.md) | [Process Analytical Technology](../process/process-analytical-technology.md) | [Method Validation](../quality-control/method-validation.md) | [Purity Analysis](../quality-control/purity-analysis.md)
