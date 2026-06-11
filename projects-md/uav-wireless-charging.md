# UAV Wireless Charging Station

**Category:** Hardware & PCB · Embedded Control  
**Status:** 🟡 Ongoing (2026 – Present)  
**Organization:** Zenopix Technology, Konya, Turkey

---

## Overview

An integrated wireless charging platform designed for UAV (drone) applications — enabling autonomous charging cycles without manual battery replacement. The system consists of a ground transmitter (Tx) pad and an onboard receiver (Rx) module embedded within the UAV airframe.

The goal is to remove operator dependency from drone charging, making long-duration autonomous missions viable in real-world deployment environments.

---

## Key Contributions

### Power Electronics Architecture
- Architected the full Tx/Rx power electronics pipeline, from AC/DC conversion to the resonant L-C tank network and onboard rectification.
- Designed the transmitter-side H-bridge inverter to drive the Tx coil at the resonant frequency, maximizing energy transfer efficiency.
- Engineered the receiver-side rectifier and regulation stage to provide clean, stable voltage for the UAV battery pack.

### Battery Management System (BMS)
- Developed a custom BMS tailored for UAV LiPo battery packs, implementing safe charging profiles (CC/CV), State of Charge estimation, and cell balancing logic.
- Integrated real-time battery-health monitoring and embedded fault handling via **SMBus** communication for reliable protection of the energy storage system.
- Designed overvoltage, undervoltage, overcurrent, and thermal cutoff protection circuits.

### Embedded Firmware & Control
- Integrated power conversion, BMS supervision, and embedded control into a unified R&D platform running on STM32 with FreeRTOS.
- Implemented real-time telemetry reporting and system-health logging for research validation and safety monitoring.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **Power Electronics** | Resonant WPT, H-Bridge Inverter, Rectifier, SMPS |
| **BMS** | SMBus, CC/CV Charging, State of Charge, Cell Balancing |
| **MCU / Firmware** | STM32, FreeRTOS, Embedded C |
| **PCB Design** | KiCad, High-Current Layout, Galvanic Isolation |
| **Communication** | SMBus, UART, SPI |

---

## Outcome

The platform serves as a working R&D prototype demonstrating the full system integration of wireless power transfer, intelligent battery management, and embedded control — directly applicable to commercial UAV fleet operations and autonomous charging infrastructure.
