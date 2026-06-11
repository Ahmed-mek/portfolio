# Laser Vibrometer PCB & System Design

**Category:** Hardware & PCB  
**Status:** ✅ Completed (2024)  
**Type:** Freelance Project

---

## Overview

A custom embedded instrumentation platform designed for precision laser vibrometry — measuring vibration frequency, amplitude, and displacement using a laser module and Time-of-Flight (ToF) sensor. The system includes battery management, SD-card data logging, and PC communication, forming a standalone portable measurement instrument.

---

## Key Contributions

### PCB Hardware Design
- Designed a custom **multi-function PCB** integrating:
  - **Precision laser control circuit** for stable, controlled laser output suitable for vibrometry measurements.
  - **ToF (Time-of-Flight) sensor** interface for accurate distance and vibration displacement measurement via I2C.
  - **Battery charging and power-management circuitry** — Li-Po charger IC, fuel gauge, and multi-rail LDO regulators for clean analog and digital power domains.
  - **MicroSD card interface** for high-speed data logging of captured vibration waveforms.
  - **UART/USB interface** for real-time PC communication and firmware updates.

### Embedded Firmware
- Developed embedded firmware for sensor data acquisition, laser control, real-time signal processing, and SD-card logging.
- Implemented digital filtering to extract clean vibration signals from raw ToF sensor data in real time.

### Data Logging & PC Communication
- Developed PC communication protocols over UART/USB for streaming measurement data to a host computer for analysis and post-processing.
- Implemented high-speed SD-card data logging to support repeatable test capture and long-duration vibration measurements.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32 |
| **Sensors** | ToF Sensor (I2C), Precision Laser Module |
| **Power** | Li-Po Charger, Fuel Gauge, LDO Regulators |
| **Interfaces** | I2C, UART, SPI (SD Card), USB |
| **Data** | MicroSD Logging, PC Serial Communication |
| **PCB Design** | KiCad, Mixed-Signal Layout |
| **Firmware** | Embedded C, Digital Signal Filtering |

---

## Outcome

A fully functional portable laser vibrometer instrument delivered to the client, capable of capturing, logging, and transmitting vibration waveform data for mechanical testing and quality-control applications.
