# Hologram Fan System — TUBITAK R&D Project

**Category:** Embedded Control · Hardware & PCB  
**Status:** ✅ Completed (2024 – 2026)  
**Organization:** Zenopix Technology — Government-Funded TUBITAK R&D Program

---

## Overview

A government-funded R&D project to engineer a high-performance holographic Persistence of Vision (PoV) display system. A custom 0.5-meter LED fan blade rotates at high speed to project 3D holographic images mid-air, driven by an integrated BLDC motor-control system, high-density LED driver PCB, and a 200W resonance-based wireless power transfer subsystem for powering the rotating assembly without slip rings.

This project spans the full engineering lifecycle — from power electronics and PCB design to embedded firmware and wireless power delivery — representing one of the most technically demanding R&D projects in the portfolio.

---

## Key Contributions

### High-Density LED PCB Design
- Engineered a custom **0.5-meter LED PCB** for the rotating fan blade with high-density LED placement and driver IC selection capable of MHz-range switching frequencies.
- Designed high-current KiCad PCBs with strict **galvanic isolation** between the power electronics and high-speed control circuitry to eliminate interference and ensure safe operation.

### BLDC Motor Control
- Implemented **FOC (Field-Oriented Control)**, **Space Vector PWM (SVPWM)**, **Six-Step Commutation**, and **PID speed control** loops to achieve precise rotational stability required for stable holographic image projection.
- Tuned speed control loops for sub-millisecond response times to maintain synchronization between rotation position and LED pixel timing.

### STM32 FreeRTOS Firmware
- Architected **STM32 firmware running FreeRTOS** for deterministic, multitasking embedded control covering: motor control, LED data update, wireless power telemetry, fault detection, and system recovery.
- Implemented real-time safety monitoring, emergency stop handling, and error recovery to meet R&D safety requirements.

### 200W Wireless Power Transfer
- Designed a resonance-based wireless power transfer (WPT) system, engineering custom Tx/Rx coil circuits to achieve **continuous 200W power transmission** across the rotating air gap.
- Applied **Fuzzy Logic Control** to dynamically regulate wireless power delivery and maintain stable energy transfer under varying operating conditions (load, temperature, coil alignment).

### Validation & Debugging
- Validated power electronics, PCB assemblies, and embedded control behavior using oscilloscopes, function generators, and hands-on hardware debugging.
- Performed EMC analysis and iterative hardware revision cycles to meet project performance targets.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **Embedded Firmware** | STM32, FreeRTOS, Embedded C, DMA, UART, SPI |
| **Motor Control** | FOC, SVPWM, Six-Step, PID, Hall Sensors |
| **Power Electronics** | Resonant WPT (200W), Galvanic Isolation, Buck/Boost |
| **PCB Design** | KiCad, High-Density LED PCB, High-Current Layout |
| **Control Algorithms** | PID, Fuzzy Logic Control |
| **Tools** | Oscilloscope, Function Generator, Rapid Prototyping |

---

## Outcome

Successfully delivered a fully integrated PoV hologram fan prototype as part of a TUBITAK-funded R&D program — demonstrating system-level engineering competence across power electronics, motor control, embedded firmware, and advanced control algorithms in a single demanding project.
