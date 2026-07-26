---
description: "Leak testing and container-closure integrity for peptide products — deterministic and probabilistic methods for vial and packaging validation."
---

# Leak & Integrity Testing

## Container-Closure Integrity for Peptide Products

## Introduction

Container-closure integrity testing (CCIT) is critical for lyophilized peptides packaged in vials or pre-filled syringes. A compromised seal can allow ingress of moisture, oxygen, and microorganisms, leading to product degradation, loss of potency, or contamination. CCIT must be demonstrated during development (package validation) and verified during routine production (100% or statistical testing). The selection of CCIT method depends on the product's dosage form, container type, sensitivity requirements, and whether the method is deterministic or probabilistic.

USP <1207> (Package Integrity Evaluation) provides the regulatory framework. For sterile peptides intended for injectable use, a deterministic method (e.g., vacuum decay, high-voltage leak detection) is preferred, as these methods provide objective, quantifiable results for every container tested.

## Method Comparison: Deterministic vs. Probabilistic

| Method | Type | Sensitivity (µm) | Destructive | Throughput | Container Compatibility | Quantitative |
|---|---|---|---|---|---|---|
| **Vacuum decay** | Deterministic | 5–15 | No | High (100% in-line possible) | Rigid vials only | Yes |
| **Pressure decay** | Deterministic | 5–20 | No | Moderate | Rigid vials, syringes | Yes |
| **Helium leak** | Deterministic | 1–5 | No | Moderate (requires tracer gas) | Vials, syringes (sealed under He) | Yes |
| **High-voltage leak (HVLD)** | Deterministic | 5–10 | No | High | Liquid-filled only | Yes (qualitative pass/fail) |
| **Dye ingress** | Probabilistic | 5–10 | Yes | Low | All containers | No (pass/fail) |
| **Bubble emission** | Probabilistic | 20–50 | Yes | Low | Flexible packaging | No |
| **Microbial challenge** | Probabilistic | <0.5 (will pass only if seal is intact) | Yes | Very low (weeks incubation) | All containers | No |

For lyophilized peptide products, **vacuum decay** is the most widely adopted deterministic method because it requires no tracer gas or liquid fill, works directly on the sealed vial, and provides results within seconds.

## Vacuum Decay Method — Detailed Procedure

### Principle
The vial is placed in a sealed test chamber. A vacuum is drawn and the chamber is isolated. Any leak through the vial closure causes air ingress, resulting in a measurable pressure increase over time.

### Parameters and Acceptance Criteria

| Parameter | Setting |
|---|---|
| Test chamber pressure | −250 to −400 mbar (gauge) |
| Fill time (vacuum draw) | 2–5 seconds |
| Stabilization time | 1–3 seconds |
| Test (measurement) time | 5–15 seconds |
| Leak threshold (pressure rise) | 0.1–0.5 mbar (dependent on headspace volume) |
| Equivalent leak diameter | 5–15 µm |
| Reference standard | ASTM F2338 |

### Method Qualification (per USP <1207>)

| Criterion | Requirement |
|---|---|
| Positive control (laser-drilled 5 µm hole) | Detected with ≥95% probability |
| Negative control (intact, sealed vial) | Pass with margin ≥2× threshold |
| Specificity | No false positives from container deformation |
| Precision | CV ≤15% across 10 replicate measurements |
| Robustness | Insensitive to vial position, surface texture, label placement |

## Dye Ingress Method (Probabilistic)

### Procedure
1. Place vials in a vacuum chamber submerged in dye solution (e.g., methylene blue, 0.1%)
2. Apply vacuum (−500 mbar) for 30 minutes
3. Release vacuum; maintain ambient pressure for 30 minutes
4. Remove vials, rinse exterior
5. Inspect: any dye visible inside the vial = leak

Sensitivity: ~5–10 µm (equivalent hole diameter). The method is destructive — each vial tested cannot be released for use. Dye ingress is used primarily during package development and validation rather than routine release testing.

## Test Frequency Requirements (per USP <1207>)

| Product Risk Level | Development Stage | Validation Requirement | Routine Production |
|---|---|---|---|
| Sterile / injectable (highest) | 3 positive controls + 10 intact vials per package type | ≥100 vials (or ≤3 defects in sample) | 100% testing for new lines; statistical sampling for established lines |
| Non-sterile liquid (e.g., ophthalmic) | 2 positive controls + 5 intact vials | Statistical sample per ASTM E2559 | Reduced statistical sampling |
| Lyophilized (high moisture sensitivity) | 3 positive controls + 10 intact vials | Statistical per ASTM E2559 | In-line vacuum decay preferred |

### Sampling Table for Routine CCIT (USP <1207> and ASTM E2559)

| Batch Size (units) | Sample Size (normal) | Acceptance Number (defects allowed) |
|---|---|---|
| ≤1,000 | 30 | 0 |
| 1,001–10,000 | 50 | 0 |
| 10,001–50,000 | 80 | 1 |
| >50,000 | 125 | 1 |

## Interpretation Guide

A vacuum decay pass indicates the container-closure system is intact within the detection limit of the method (typically 5–15 µm). A fail indicates a leak ≥ the method's sensitivity threshold. Confirmed failures should be investigated by:
1. Visual inspection of the vial, stopper, and crimp seal
2. Dimensional measurement of stopper seating depth and crimp height
3. Review of the stoppering/crimping process parameters (vacuum level, seating time, crimp force)

For lyophilized products, leaks that appear only after freeze-drying (e.g., cracked vial due to thermal stress) require increased temperature control during the lyophilization cycle.

## Common Issues

- **Edge-of-specification failures**: Leaks near the threshold (5–10 µm) may intermittently pass or fail. Set the threshold conservatively (≤5 µm equivalent) for sterile products.
- **False positives from stopper movement**: A stopper that reseats during vacuum application may generate a transient pressure change. Increase stabilization time or use a slower vacuum ramp.
- **Labelled vial interference**: Labels covering the vial shoulder can mask leak paths. Test unlabeled vials or ensure labels are positioned below the crimp seal.
- **Moisture condensation in test chamber**: For lyophilized product tested immediately after freeze-drying, residual moisture can evaporate into the vacuum chamber and trigger false failures. Allow vials to equilibrate at room temperature for 1–2 hours before testing.

> 🔗 Related: [Packaging Guide](../manufacturing/peptide-packaging.md) | [Stability Testing](./stability-testing.md) | [Quality Control Overview](./index.md) | [Custom Peptide Synthesis OEM Manufacturing Quality Standards](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
