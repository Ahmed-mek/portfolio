# End-to-End Control System — Abrasion Tester Machine

**Category:** Embedded Control · PC Software  
**Status:** ✅ Completed (2021 – 2023)  
**Organization:** Zenopix Technology, Konya, Turkey

---

## Overview

A complete end-to-end embedded control system developed for an industrial **abrasion tester machine** — used in material testing laboratories to measure material wear resistance under controlled friction conditions. The project covers the full chain from sensor acquisition and embedded motor control to PC-based test management software.

---

## Key Contributions

### Signal Processing & Sensor Acquisition
- Built the complete signal-processing pipeline for accurate sensor-data acquisition using:
  - **Digital filtering** (FIR/IIR) to remove noise from load cell and encoder readings.
  - **Analog filtering** with hardware RC networks at the ADC inputs for anti-aliasing.
  - **SPI and I2C** interfaces for connecting precision sensors (load cell transmitter, position encoder, temperature/humidity sensor).

### DC Motor Driver & PID Speed Control
- Developed a **custom DC motor driver** with embedded **PID algorithm** for accurate speed calibration and repeatable mechanical testing.
- Tuned PID gains for stable speed regulation under varying friction loads during the abrasion test cycle.
- Implemented test-cycle state machine: ramp-up → constant speed → ramp-down → data capture → cycle count tracking.

### PC Software (C# GUI)
- Programmed a **PC-based C# graphical user interface** (Windows Forms) for complete machine control:
  - Real-time speed, load, and cycle data display with live graphs.
  - Test parameter configuration: RPM setpoint, load threshold, cycle count target.
  - **Real-time UART communication** with the embedded control board for bidirectional control and monitoring.
  - Data logging: export test results to CSV for laboratory records and analysis.
  - Calibration wizard for encoder and load cell zero-point setup.

### Hardware Bring-Up & Validation
- Delivered the control-board hardware and firmware from concept through debugging, calibration, and operational validation.
- Conducted full machine integration testing with the mechanical team to validate end-to-end system behavior.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32 |
| **Interfaces** | SPI, I2C, UART, ADC |
| **Signal Processing** | Digital Filtering, Analog RC Filtering |
| **Motor Control** | DC Motor Driver, PID Speed Control |
| **PC Software** | C#, Windows Forms, Serial Communication |
| **Data** | CSV Logging, Real-Time Graph |
| **PCB Design** | KiCad |

---

## Outcome

A production-ready abrasion tester machine control system delivered and deployed at Zenopix Technology — providing accurate, repeatable material wear testing with full PC-based monitoring and data export capabilities.
