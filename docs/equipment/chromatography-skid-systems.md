---
description: "Technical guide to production-scale chromatography skid systems for peptide purification — covering DAC columns, flow distribution, and skid specification tables by throughput capacity."
---

# Production-Scale Chromatography Skid Systems

## Introduction

As peptide synthesis scales from bench to production, preparative chromatography shifts from manual glass columns to integrated chromatography skid systems. These skids combine pumps, columns, detectors, fraction collectors, and process control into a single platform designed for continuous, repeatable, and GMP-compliant purification. This guide covers the key components, configurations, and specifications for production-scale peptide chromatography.

## System Components

### 1. Solvent Delivery System

- **High-flow pumps:** Dual-piston or quaternary pumps capable of 1–500 L/min
- **Solvent selectors:** Multi-port valves for buffer, organic modifier, cleaning, and storage solvents
- **Degassing:** Online vacuum degassers or helium sparging for reproducible gradient formation
- **Mixing:** Dynamic or static mixers for gradient homogeneity

### 2. Column Hardware

Most production-scale peptide columns use Dynamic Axial Compression (DAC) technology:

| Feature | DAC Column | Fixed-Bed Column |
|---------|-----------|------------------|
| Packing method | Pneumatic or hydraulic piston compression | Slurry packing at high pressure |
| Bed stability | Maintained during operation | Can settle over time |
| Reproducibility | Excellent — re-packable in situ | Requires full re-packing |
| Scale range | 50 mm to 1600 mm ID | Typically <100 mm ID |
| Typical operating pressure | ≤100 bar | ≤200 bar |
| Cost | Higher capital, lower per-run | Lower capital, higher per-run |

### 3. Dynamic Axial Compression (DAC) Columns

DAC columns use a movable piston to compress the stationary phase bed, eliminating voids that would otherwise form during operation. Key specifications:

| Parameter | Typical DAC Column Performance |
|-----------|-------------------------------|
| Piston travel | 5–50 cm adjustable |
| Compression pressure | 20–60 bar (pneumatic) or 50–100 bar (hydraulic) |
| Bed height range | 5–40 cm depending on column diameter |
| Packing uniformity | CV <3% across bed cross-section |
| Re-packing frequency | Every 20–100 cycles depending on sample load |

### 4. Flow Distribution

Proper flow distribution across the full column cross-section is critical at production scale:

- **Dual-mesh distribution plates** at inlet and outlet
- **Radial flow distributors** for very large columns (>300 mm ID)
- **Specification:** Flow distribution uniformity should produce ≤5% variation in breakthrough front

Poor flow distribution is the leading cause of reduced resolution in scaled-up chromatography. At large diameters (>200 mm), even small packing irregularities create preferential channels that destroy resolution.

### 5. Detection and Fractionation

| Component | Function | Typical Specification |
|-----------|----------|----------------------|
| UV detector (PDA) | Peak detection, purity assessment | 190–800 nm, 2–10 mm pathlength flow cell |
| Conductivity monitor | Salt gradient tracking | 0–500 mS/cm |
| pH probe | Online pH monitoring | ±0.05 pH units |
| Automated fraction collector | Peak-based collection | UV threshold + time window |
| Fraction weight verification | Confirm collected volume | Load cell or flow meter |

### 6. Process Control System

- **SCADA or PLC-based** control with recipe management
- **21 CFR Part 11 compliant** data logging and audit trail
- **Automated column equilibration, injection, gradient, wash, and strip cycles**
- **Real-time purity-based fraction cutting** using UV ratio or spectral analysis
- **Oscilloscope-mode peak display** for manual fine-tuning of fraction windows

## Skid Specification Table by Throughput

| Parameter | Analytical | Semi-Prep | Process (Small) | Process (Medium) | Production (Large) |
|-----------|------------|-----------|-----------------|------------------|-------------------|
| **Column ID** | 2–4.6 mm | 10–30 mm | 50–100 mm | 100–300 mm | 300–800 mm |
| **Flow rate** | 0.2–2 mL/min | 5–50 mL/min | 0.1–1 L/min | 1–10 L/min | 10–100 L/min |
| **Max pressure** | 400–1000 bar | 200–400 bar | 100–200 bar | 50–100 bar | 30–50 bar |
| **Load per cycle** | 1–100 µg | 10–50 mg | 0.5–5 g | 5–50 g | 50–500 g |
| **Cycle time** | 10–30 min | 15–45 min | 20–60 min | 30–90 min | 45–120 min |
| **Productivity (day)** | 0.1–5 mg | 0.5–5 g | 10–100 g | 0.1–1 kg | 1–10 kg |
| **DAC option** | No | Optional | Recommended | Required | Required |
| **Approx. capital (USD)** | $50K–$100K | $100K–$250K | $250K–$500K | $500K–$1.5M | $1.5M–$5M |
| **Application** | QC, method dev | Scale-up studies | Clinical supply | Commercial small | Commercial large |

## Packing Methods for Large Columns

### Slurry Packing (Fixed Bed)

- Stationary phase suspended in packing solvent (e.g., 70:30 acetone:water)
- Pushed into column at high flow rate and pressure
- Best for smaller columns (<100 mm ID)
- Requires careful slurry concentration and flow control

### Dry Packing (Vibratory)

- Stationary phase poured as dry powder while column is vibrated
- Simpler and faster but produces less uniform beds
- Only suitable for larger particle sizes (>15 µm)

### Compression Packing (DAC)

- Slurry poured into column, then piston mechanically compresses the bed
- Most reproducible packing method for production-scale columns
- Allows occasional re-tightening (re-compression) between runs to maintain bed integrity

## Resin Considerations for Production Scale

| Parameter | Lab Scale | Production Scale | Impact |
|-----------|-----------|-----------------|--------|
| Particle size | 3–5 µm | 10–30 µm | Larger particles reduce back pressure at high flow |
| Particle size distribution | Narrow (CV <15%) | Narrow (CV <15%) | Broad distribution causes uneven bed packing |
| Mechanical strength | Moderate | High (cross-linked agarose or polymer) | Soft gels compress under production flow rates |
| Pore size | 100–300 Å | 300–1000 Å | Larger peptides need larger pores at scale |
| Cost per liter | $1,000–$5,000 | $500–$3,000 | Economies of scale matter |

## System Scalability Considerations

When scaling a method from analytical to production:

1. **Keep linear velocity constant** — maintain the same cm/hr flow rate across scales
2. **Keep bed height similar** — do not increase column length proportionally to diameter
3. **Scale loading proportionally** — load per mL of resin should remain constant
4. **Validate resolution at each scale** — resolution almost always decreases at larger diameters
5. **Account for system dispersion** — larger skids have more extra-column volume

## Common Skid Configurations

| Configuration | Description | Best For |
|--------------|-------------|----------|
| **Single column** | One column, batch gradient | Simple purification, low throughput |
| **Recycle chromatography** | Peak re-injected for additional passes | High-purity requirements (>99%) |
| **Simulated Moving Bed (SMB)** | Continuous countercurrent operation | Binary separations, very high throughput |
| **Stacked column / MCC** | Sequential columns with staggered cycles | Productivity increase 2–3× vs batch |

## Operational Maintenance

| Maintenance | Frequency | Action |
|------------|-----------|--------|
| Pressure test | Daily | Verify system pressure limits |
| Pump calibration | Weekly | Gravimetric flow check |
| Column re-compression | Every 5–20 runs | Piston adjustment (DAC only) |
| UV lamp replacement | Every 2,000 hours or annual | Document with log entry |
| Seal replacement (pump) | Every 3–6 months | Dependent on solvent usage |
| Full skid PM | Every 6–12 months | Valve rebuild, sensor calibration |
| Column re-packing | Every 20–100 cycles | Based on resolution decline |

> **🔗 Related:** [Column Selection Guide](./column-selection-guide.md) | [Column Care and Maintenance](./column-care-maintenance.md) | [Laboratory-Scale Reactors](./laboratory-scale-reactors.md) | [Cleanroom Classification](./cleanroom-classification.md)
