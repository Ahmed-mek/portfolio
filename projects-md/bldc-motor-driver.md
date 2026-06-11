# Industrial BLDC Motor Driver

**Category:** Embedded Control · Hardware & PCB  
**Status:** 🟡 Ongoing (2026 – Present)  
**Organization:** Zenopix Technology, Konya, Turkey

---

## Overview

A high-reliability industrial BLDC (Brushless DC) motor driver platform engineered for demanding electromechanical applications. The project focuses on building a complete motor-control architecture — from hardware design through firmware — optimized for stability, thermal robustness, and long-term industrial deployment.

---

## Key Contributions

### Motor Control Architecture
- Defined the full hardware architecture for a robust industrial BLDC motor driver, selecting appropriate power MOSFET switches, gate driver ICs, and control topology.
- Structured the design around both **Field-Oriented Control (FOC)** and **Six-Step Commutation** algorithms, providing flexibility for different torque and efficiency requirements.
- Formulated motor-control loop requirements covering current sensing, Clarke/Park transforms, PI controllers, and Space Vector PWM generation.

### Hardware Design
- Designed the 3-phase H-bridge power stage with high-current PCB layout techniques — wide copper pours, thermal relief vias, and optimized switch placement to minimize parasitic inductance.
- Selected and integrated gate drivers capable of driving high-side and low-side MOSFETs with appropriate dead-time control and shoot-through protection.
- Planned buck/boost stage integration for bus voltage regulation and regenerative braking support.

### Protection & Reliability
- Designed comprehensive protection logic: overcurrent (cycle-by-cycle), overvoltage, undervoltage, overtemperature, and phase-loss detection.
- Integrated hardware fault latch and firmware-level fault recovery state machine for fail-safe operation in industrial environments.

### Firmware Interface
- Defined firmware interfaces for real-time control loop execution, hall-sensor and encoder feedback, CAN-bus communication, and parameter configuration via serial interface.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **Motor Control** | FOC, Six-Step Commutation, SVPWM, PID Control |
| **Power Stage** | 3-Phase MOSFET Bridge, Gate Drivers, Current Sensing |
| **MCU / Firmware** | STM32, Embedded C, Real-Time Control Loops |
| **PCB Design** | KiCad, High-Current Layout, Thermal Management |
| **Communication** | CAN Bus, UART |

---

## Outcome

The project establishes a solid design foundation for a production-grade industrial motor driver, directly applicable to robotics actuators, CNC systems, conveyor drives, and electromechanical automation platforms.
