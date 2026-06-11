# Indoor Unmanned Vehicle Localization — Multi-IMU Sensor Fusion

**Category:** Embedded Control  
**Status:** 🟡 Ongoing (2025 – Present)  
**Type:** Master's Thesis | Necmettin Erbakan University — Mechatronics Engineering

---

## Overview

A high-performance embedded research platform designed to solve GPS-denied indoor localization for autonomous UAVs and ground vehicles. The system processes approximately **250 raw data channels** from a custom Multi-IMU sensor array in real time using an STM32H7 processor, FreeRTOS multitasking, and Kalman Filtering algorithms for accurate navigation-state estimation and drift reduction.

This is the author's **Master's Thesis project**, combining hardware design, real-time embedded systems, and advanced estimation theory.

---

## Key Contributions

### High-Performance Embedded Hardware
- Built a high-performance embedded system centered on **STM32H7** (480 MHz, Cortex-M7 + double-precision FPU) to handle the computational demands of multi-sensor real-time processing.
- Designed a **custom Multi-IMU hardware array** with multiple accelerometers and gyroscopes distributed across the platform for redundant, diverse motion sensing.
- Implemented **DMA-driven SPI and I2C** data acquisition pipelines to offload sensor reads from the CPU and sustain ~250 concurrent data channels at the required sampling rates.

### RTOS & Firmware Architecture
- Implemented **FreeRTOS** for deterministic multitasking: sensor acquisition, Kalman filter update, Ethernet telemetry, and system health monitoring running as isolated real-time tasks.
- Applied **FreeRTOS-MPU** for hardware-enforced memory protection, isolating critical control tasks from non-critical software components for research-grade reliability.
- Used **FreeRTOS+TCP** for robust real-time Ethernet communication, streaming processed navigation data to a host workstation for analysis and visualization.

### Sensor Fusion & Navigation Algorithms
- Developed **Kalman Filtering** and sensor-fusion algorithms to combine data from multiple IMU units, estimate position, velocity, and orientation states, and suppress sensor drift.
- Applied redundancy-based fusion logic to cross-validate IMU readings and detect faulty sensor data in real time.
- Targeted application environments: GPS-denied UAV navigation, indoor robotics localization, and autonomous vehicle state estimation.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32H7 (480 MHz, Cortex-M7) |
| **RTOS** | FreeRTOS, FreeRTOS-MPU, FreeRTOS+TCP |
| **Interfaces** | SPI, I2C, Ethernet, DMA |
| **Algorithms** | Kalman Filter, Sensor Fusion, Drift Estimation |
| **Sensors** | Multi-IMU Array (Accelerometer + Gyroscope) |
| **PCB / Tools** | KiCad, Embedded Linux, Python (analysis) |

---

## Outcome

A functioning research platform capable of real-time multi-IMU data acquisition and Kalman-filtered navigation state estimation, directly contributing to the Master's thesis on **indoor localization for autonomous vehicles** in GPS-denied environments.
