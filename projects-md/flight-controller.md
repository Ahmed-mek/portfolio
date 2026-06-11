# Flight Controller Architecture & Prototyping — ArduPilot / PX4

**Category:** Hardware & PCB · Embedded Control  
**Status:** 🟡 Ongoing (2025 – Present)  
**Type:** Independent R&D Project

---

## Overview

A custom UAV flight controller designed from the ground up — reverse-engineering and analyzing industry-standard ArduPilot and PX4 flight stacks to extract hardware requirements, then designing an original PCB layout and bare-metal firmware strategy for a custom flight controller tailored to the team's UAV development objectives.

---

## Key Contributions

### Flight Stack Analysis & Requirements Engineering
- Conducted comprehensive **architectural analysis and reverse engineering** of both ArduPilot and PX4 open-source flight stacks, studying sensor requirements, communication protocols, timing constraints, and power distribution architectures.
- Defined hardware, firmware, and communication protocol requirements for the custom controller based on best-practice patterns extracted from production flight controllers.

### Custom PCB Design
- Designed the first iteration of a custom **flight controller PCB** in KiCad with focused attention to:
  - **Sensor isolation:** Physically separating the IMU sensor zone from high-current switching circuits to minimize electromagnetic interference on inertial measurements.
  - **Power distribution:** Multi-rail power architecture (servo rail, logic rail, payload power) with filtering and protection per rail.
  - **Component placement:** IMU on vibration-isolated mount, GPS connector away from power stages, barometer protected from airflow.
  - **Layout constraints:** 4-layer PCB stack-up with dedicated ground plane for EMC and signal integrity.

### Firmware Strategy
- Formulated a **bare-metal firmware architecture** strategy covering:
  - Sensor driver interfaces (SPI/I2C for IMU, baro, compass)
  - Flight control loops (attitude, rate, position)
  - Embedded safety behaviors (arming/disarming, failsafe)
  - Future compatibility with ArduPilot/PX4 HAL layer

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32 (Cortex-M7) |
| **PCB Design** | KiCad, 4-Layer Stack-Up, EMC Layout |
| **Flight Stack Reference** | ArduPilot, PX4 |
| **Interfaces** | SPI, I2C, UART, CAN, PWM/DShot |
| **Sensors** | IMU (ICM-42688), Barometer, Compass, GPS |
| **Firmware** | Bare-Metal C, HAL Layer Design |

---

## Outcome

First PCB iteration completed with sensor isolation zones, power distribution architecture, and full component placement finalized in KiCad. Firmware architecture strategy documented. Project continues with PCB manufacturing and firmware bring-up.
