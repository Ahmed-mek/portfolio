# Hyperloop Data Transmission System — STM32F7 Networking

**Category:** Embedded Control · PC Software  
**Status:** ✅ Completed (2023)  
**Type:** Academic Competition — Hyperloop Development Competition

---

## Overview

A real-time **data transmission system** designed for a Hyperloop competition, enabling bidirectional communication between a high-speed train capsule and a ground-based monitoring station. Built around STM32F7's native Ethernet capability and a TCP/IP stack, the system validates embedded networking concepts applicable to high-speed transportation and autonomous systems.

---

## Key Contributions

### Embedded Ethernet & TCP/IP Stack
- Designed and implemented a **data-transmission system** using the **STM32F7's hardware Ethernet MAC** combined with a TCP/IP stack for reliable, low-latency data communication.
- Configured the embedded TCP/IP stack (lwIP) for efficient packet processing on the resource-constrained microcontroller platform.
- Implemented a **TCP client/server architecture** — the train-side STM32F7 acts as a client, streaming sensor and telemetry data to the monitoring station server.

### Network Infrastructure
- Deployed the communication path through **router and Wi-Fi infrastructure** for flexible physical separation between train and monitoring station during tests.
- Validated network reliability and packet integrity across the TCP link under simulated competition conditions.

### Ground Monitoring Station
- Developed the **PC-side monitoring application** to receive, decode, and display real-time train data — including speed, position, sensor readings, and system status.
- Implemented data visualization for operators during competition runs.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32F7 (Cortex-M7, 216 MHz) |
| **Networking** | Ethernet MAC, TCP/IP (lwIP), TCP Client/Server |
| **Interfaces** | Ethernet, UART, SPI, I2C |
| **Infrastructure** | Router, Wi-Fi, LAN |
| **PC Software** | Monitoring Application, Data Visualization |
| **Firmware** | Embedded C |

---

## Outcome

A fully operational real-time telemetry and control link between the Hyperloop train capsule and monitoring station — demonstrating embedded TCP/IP networking capability applicable to high-speed transportation, autonomous vehicle telemetry, and industrial IoT systems.
