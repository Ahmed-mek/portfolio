# POSYAK — Wearable Assistive Device for Parkinson's Patients

**Category:** Embedded Control  
**Status:** ✅ Completed (2022)  
**Type:** Competition — Barrier-Free Living Technologies (Engelsiz Yaşam Teknolojileri)

---

## Overview

**POSYAK** is a wearable assistive device designed to improve quality of life for **Parkinson's patients** by detecting and alerting on abnormal head/neck posture — a common symptom caused by Parkinson's-related muscle rigidity. The device worn around the neck monitors head orientation continuously and generates a posture alert (vibration feedback) when the neck remains bent beyond a defined angular threshold for a set duration.

The project was developed as a competition entry for the Barrier-Free Living Technologies program focused on accessibility and assistive engineering.

---

## Key Contributions

### Wearable Hardware Design
- Designed and built the **neck wearable device** with an embedded IMU (MPU-6050, 3-axis accelerometer + gyroscope) for real-time head orientation sensing.
- Implemented **I2C bus** communication between the IMU and the microcontroller for continuous motion data acquisition.
- Integrated a **vibration haptic feedback motor** as the primary alert mechanism — providing non-intrusive physical feedback to the patient when posture deviation is detected.
- Designed a **rechargeable battery system** (12-hour operational life) for all-day wearability.

### Posture Detection Algorithm
- Developed the **head posture detection algorithm**: continuously reading IMU orientation data, computing neck tilt angle, and triggering alerts when the bend angle exceeds the threshold for the user-defined hold duration.
- Implemented user-configurable threshold and alert delay parameters to accommodate individual patient needs and disease progression levels.

### Mobile Application Integration
- Integrated the wearable with a **companion mobile application** via Bluetooth (BLE) for:
  - Real-time head-movement behavior recording and visualization.
  - Historical posture data logging and trend analysis for caregiver and clinician review.
  - Alert configuration and device settings management.

---

## Technology Stack

| Domain | Technologies |
|---|---|
| **MCU** | ARM Cortex-M (Arduino / STM32) |
| **Sensors** | MPU-6050 IMU (Accelerometer + Gyroscope) |
| **Communication** | I2C (sensor), Bluetooth 5.0 BLE (mobile) |
| **Output** | Haptic Vibration Motor |
| **Power** | Li-Po Battery, 12h Life |
| **Mobile App** | Android (BLE), Data Logging, Visualization |
| **Firmware** | Embedded C |

---

## Outcome

A functional wearable assistive device demonstrating practical embedded engineering applied to medical assistive technology — validated with posture detection accuracy and mobile app integration for patient data tracking.
