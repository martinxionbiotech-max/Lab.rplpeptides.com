---
description: "Freeze dryer specifications for peptide lyophilization — shelf temperature, vacuum, condenser capacity, and batch sizing."
---
# Freeze Dryer (Lyophilizer)

## Peptide Drying Equipment

## Category
Drying Equipment

## Application
Remove solvents from purified peptide solutions to produce stable powder

## Function
Freeze peptide solution and sublime ice under vacuum.

---

## Introduction

Freeze drying (lyophilization) is the final drying step in peptide manufacturing, converting the purified peptide solution from HPLC purification into a stable, free-flowing powder. The process works by freezing the peptide solution and then reducing the chamber pressure to enable sublimation of ice directly to water vapor, bypassing the liquid phase. This gentle drying method preserves peptide structure, minimizes aggregation, and produces a product with excellent shelf stability and rapid reconstitution properties. A well-designed and validated freeze-drying cycle is essential for maintaining peptide quality during this critical unit operation.

## Primary vs. Secondary Drying Phases

Freeze drying consists of three distinct phases: freezing, primary drying (sublimation), and secondary drying (desorption).

### Phase 1: Freezing
The solution is cooled below its eutectic point or glass transition temperature (Tg') to completely solidify the product. The freezing rate and annealing steps determine the ice crystal structure, which directly influences primary drying efficiency.

| Freezing Parameter | Typical Range | Effect on Drying |
|-------------------|--------------|------------------|
| Cooling rate | 0.5–5.0 °C/min | Faster cooling = smaller ice crystals = slower sublimation |
| Shelf temperature setpoint | -40 to -50 °C | Must be below Tg' of the peptide formulation |
| Hold time at final temperature | 1–3 hours | Ensures complete solidification |
| Annealing step (optional) | Hold at -10 to -20 °C for 2–4 h | Promotes larger ice crystals, faster primary drying |

### Phase 2: Primary Drying (Sublimation)
Chamber pressure is reduced to below the vapor pressure of ice at the product temperature, causing ice crystals to sublime. This is the longest phase.

| Primary Drying Parameter | Research Scale | Production Scale |
|------------------------|---------------|-----------------|
| Chamber pressure | 0.05–0.30 mbar | 0.05–0.30 mbar |
| Shelf temperature | -10 to +10 °C | -10 to +10 °C |
| Product temperature | -30 to -20 °C | -30 to -20 °C |
| Typical duration | 12–48 hours | 24–72 hours |
| Sublimation rate | 0.5–2.0 mm/hour (ice front) | 0.5–2.0 mm/hour |

### Phase 3: Secondary Drying (Desorption)
Bound water remaining after sublimation is removed by gradually raising the shelf temperature under high vacuum.

| Secondary Drying Parameter | Typical Range | Endpoint Criteria |
|--------------------------|--------------|-------------------|
| Shelf temperature ramp | +0.1 to +0.5 °C/min | Product temperature tracks shelf |
| Final shelf temperature | +20 to +40 °C | Pirani vs. capacitance manometer convergence |
| Vacuum level | 0.01–0.10 mbar | No further pressure rise with isolation |
| Duration | 4–12 hours | Residual moisture ≤1–2% (by Karl Fischer) |

## Shelf Ramp Rates and Product Temperature Monitoring

| Shelf Ramp Step | Ramp Rate | Duration | Monitoring Method | Critical Limits |
|----------------|-----------|----------|-------------------|----------------|
| Ambient to freezing | 1.0–3.0 °C/min | 20–60 min | Product thermocouple | Product must reach ≤ -40 °C |
| Freezing hold | 0 °C/min (isothermal) | 1–3 hours | Product thermocouple | Product stable at setpoint |
| Freezing to primary | 0.5–1.0 °C/min | 30–60 min | Pirani + capacitance manometer | Ed = Pirani/CM ratio, target <2 |
| Primary hold | 0 °C/min (isothermal) | 24–72 hours | Product T, Pirani/CM, pressure rise | Sublimation endpoint |
| Primary to secondary | 0.1–0.3 °C/min | 1–2 hours | Product thermocouple | Product T ≤ collapse temperature |
| Secondary ramp | 0.2–0.5 °C/min | 1–4 hours | Product thermocouple | Avoid degradation above 40 °C |
| Secondary hold | 0 °C/min (isothermal) | 4–12 hours | Pirani/CM, pressure rise test | Pressure rise <10 µbar/min |

**Product temperature monitoring** is achieved by placing thermocouples directly into representative vials (typically 5–10 per batch). The thermocouple tip must be positioned in the center-bottom of the vial to accurately measure the product temperature at the ice sublimation front.

## Cycle Development Table

| Formulation Type | Tg' / Eutectic | Freeze Temp | Primary Shelf T | Vacuum | Secondary T | Typical Total Time |
|-----------------|---------------|-------------|----------------|--------|-------------|-------------------|
| Simple salt (e.g., NaCl peptide) | -21 °C | -40 °C | -10 °C | 0.10 mbar | +20 °C | 24–36 h |
| Trehalose/sucrose formulation | -32 °C | -45 °C | -15 °C | 0.08 mbar | +25 °C | 36–48 h |
| Mannitol bulking agent | -1.5 °C (eutectic) | -40 °C | -5 °C | 0.15 mbar | +30 °C | 28–40 h |
| Unformulated peptide (TFA salt) | -15 to -25 °C | -40 °C | -10 °C | 0.10 mbar | +20 °C | 24–48 h |
| Peptide with acetate buffer | -35 °C | -50 °C | -20 °C | 0.06 mbar | +25 °C | 48–60 h |
| Large peptide (>30 AA) | -20 to -30 °C | -45 °C | -15 °C | 0.08 mbar | +20 °C | 36–56 h |

Cycle development typically begins with differential scanning calorimetry (DSC) to determine Tg' or the eutectic temperature, then proceeds through freeze-dry microscopy (FDM) to establish the collapse temperature. The target product temperature during primary drying should be 2–5 °C below the collapse temperature to ensure a pharmaceutically elegant cake structure.

## Batch Record Keeping for GMP Lyophilization

| Parameter | Recording Method | Frequency | Acceptable Range | GMP Requirement |
|-----------|-----------------|-----------|------------------|----------------|
| Chamber pressure | Capacitance manometer + Pirani | Every 5 min | ±0.01 mbar | Continuous chart or electronic log |
| Shelf temperature | Resistance temperature detector (RTD) | Every 5 min | ±1.0 °C | Continuous recording |
| Product temperature | Type T thermocouple in product vials | Every 5 min | ±0.5 °C | Minimum 5 representative vials |
| Condenser temperature | RTD | Every 15 min | ±2.0 °C | Continuous recording |
| Vacuum pump status | Digital or analog | At start/end | On/off | Operator sign-off |
| Pressure rise test (endpoint) | Isolate chamber, measure rise | Every 2 h near endpoint | <10–20 µbar/min | Recorded in batch log |
| Residual moisture | Karl Fischer titration | At cycle end | ≤2.0% w/w | Certificate of analysis |
| Cake appearance | Visual inspection | At cycle end | Pharmaceutically elegant | Batch record photo |

For validated lyophilization cycles, the critical process parameters (CPP) — shelf temperature, chamber pressure, and ramp rates — are maintained within validated ranges. Deviations must be documented with deviation reports. Batch records include a time-stamped temperature/pressure chart signed by both the operator and QA reviewer.

## Key Takeaways

- **Three-Phase Process:** Freeze drying comprises freezing (solidification), primary drying (sublimation of ice at 0.05–0.30 mbar), and secondary drying (desorption of bound water to ≤2% residual moisture).
- **Temperature Management:** Product temperature during primary drying must be maintained 2–5 °C below the collapse temperature. Shelf ramp rates of 0.1–0.5 °C/min prevent product overheating.
- **Cycle Development:** Tg' (determined by DSC) and collapse temperature (by FDM) guide cycle parameters. Typical total cycle times range from 24–60 hours depending on formulation and batch size.
- **Batch Records:** Continuous monitoring of pressure, shelf temperature, product temperature, and pressure rise tests provides the documentation required for GMP compliance and batch release.
- **Equipment Sizing:** Condenser capacity must exceed batch water load by at least 20% to prevent ice buildup on condenser coils from reducing drying efficiency.

> 🔗 Related: [Lyophilization Process](../process/lyophilization.md) | [Vacuum Drying System](./vacuum-drying-system.md) | [Custom Peptide Synthesis & OEM](https://rplpeptides.com/custom-peptide-synthesis-oem-manufacturing-quality-standards-for-bulk-procurement/)
