# Temperature Control System — Cosmetic Medical Device Furnace

**Category:** Hardware & PCB · Embedded Control  
**Status:** ✅ Completed (2023)  
**Type:** Freelance Project

---

## Overview

A precise embedded temperature control system designed for a specialized **cosmetic medical device furnace** — requiring stable, repeatable, and operator-friendly temperature regulation for medical-grade thermal processes. The system integrates a custom control PCB, PID algorithm implementation, and a NEXTION HMI touchscreen interface for real-time monitoring and control.

---

## Key Contributions

### PCB Hardware Design
- Designed the **primary control PCB** for the medical thermal-control device, including:
  - **Thermocouple interface** (MAX31855) for high-accuracy temperature sensing.
  - **Relay driver circuit** for controlling the ceramic heating element with solid-state relay (SSR) for reliable, noise-free switching.
  - **STM32 microcontroller** for PID computation and HMI communication.
  - **Multi-rail power management** — regulated supplies for MCU, relay logic, and HMI.
  - Protective circuitry: thermal cutoff input, watchdog timer, manual override.

### PID Temperature Control
- Implemented a **PID control algorithm** tuned for stable, precise furnace temperature regulation — maintaining temperature within tight tolerances around the setpoint.
- Implemented anti-windup mechanisms and smooth ramp-up profiles to prevent thermal overshoot during initial heating.
- Designed the control loop around the thermal time constants of the furnace heating element for stable closed-loop behavior.

### NEXTION HMI Interface
- Programmed an interactive **NEXTION HMI touchscreen** interface (4.3") for operator control and real-time monitoring via UART communication:
  - Live temperature curve display (setpoint vs. actual).
  - Setpoint adjustment with numeric input.
  - Status indicators: HEATING, COOLING, TEMP OK, FAULT.
  - Manual start/stop and emergency stop button.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | STM32 |
| **Temperature Sensing** | MAX31855 Thermocouple IC, I2C/SPI |
| **Control Algorithm** | PID (Anti-Windup, Ramp Control) |
| **HMI** | NEXTION 4.3" Touchscreen, UART |
| **Output** | Solid-State Relay (SSR), Ceramic Heater |
| **PCB Design** | KiCad, Mixed-Signal Layout |
| **Firmware** | Embedded C |

---

## Outcome

A fully operational medical furnace temperature controller delivered to the client — providing stable, precise thermal control with an intuitive operator interface suitable for cosmetic medical device applications.
