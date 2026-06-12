## Track: A <br>Team: SAR ADC <br>Project: Low-Power ECG Acquisition System with Fully Differential SAR ADC

## Team Members

- Chun-Chi Lu
- Ziyu Zhang
- Yi-Hsiang Wei

**Affiliation:** Columbia University, Department of Electrical Engineering

---

## Project Overview

This project aims to develop a low-power integrated ECG acquisition system for wearable and portable cardiac monitoring applications.

The proposed system combines an analog front-end (AFE) for ECG signal conditioning with a fully differential Successive Approximation Register (SAR) Analog-to-Digital Converter for digitization.

### System Architecture

```text
ECG Electrodes
      │
      ▼
Instrumentation Amplifier (INA)
      │
      ▼
Band-Pass Filter (BPF)
      │
      ▼
Programmable Gain Amplifier (PGA)
      │
      ▼
Output Buffer
      │
      ▼
Fully Differential 10-bit SAR ADC
      │
      ▼
Digital Output
```

The SAR ADC employs bottom-plate sampling and synchronous SAR logic to achieve low power consumption while maintaining sufficient resolution for ECG signal acquisition.

---

## Design Targets

| Parameter | Target |
|------------|------------|
| ADC Architecture | Fully Differential SAR ADC |
| Resolution | 10-bit |
| Sampling Method | Bottom-Plate Sampling |
| SAR Logic | Synchronous |
| Application | Wearable ECG Monitoring |
| Estimated Core Area | 0.5–1.0 mm² |
| Proposed Core Size | 1 mm × 1 mm |
| Full Chip Size (with Pads) | 2 mm × 2 mm |

---

## Motivation

Continuous ECG monitoring is becoming increasingly important in wearable healthcare devices. Such systems require:

- Low power consumption
- Compact silicon area
- Reliable signal acquisition
- High integration level

SAR ADCs provide an attractive trade-off between power, area, and performance, making them suitable for battery-powered biomedical applications.

---

## Repository Structure

```text
docs/
├── Proposal.pdf
├── Schematic_Review.pdf
└── Layout_Review.pdf

analog/
├── INA/
├── BPF/
├── PGA/
├── Buffer/
└── SAR_ADC/

digital/
└── SAR_Logic/

simulations/

reports/
```

---

## References

1. B. Razavi, *Design of Analog CMOS Integrated Circuits*
2. R. Jacob Baker, *CMOS Circuit Design, Layout, and Simulation*
3. Tony Chan Carusone, *Analog Integrated Circuit Design*

---

## Chipathon 2026

This repository is maintained as part of the IEEE SSCS Chipathon 2026 project.
