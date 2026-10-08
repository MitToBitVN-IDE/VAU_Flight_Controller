# 🚀 VAA Flight Controller (RP2350 UAV FC)

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Hardware](https://img.shields.io/badge/KiCad-v8.0-orange.svg)
![MCU](https://img.shields.io/badge/MCU-RP2350-green.svg)

An open-source High-Performance Flight Controller for micro UAVs/Drones based on the next-generation **Raspberry Pi RP2350** microcontroller (Dual ARM Cortex-M33 / Hazard3 RISC-V). Designed by **Ngô Quang Trưởng** (Vietnam Aviation Academy - VAA).

---

## 📌 Project Overview

* **Board Name:** `26AE202_RP2350_VAUFC`
* **Revision:** `REV_01`
* **Application:** Autonomous Micro UAVs, Custom Quadcopters, Embedded Flight Systems.
* **EDA Tool:** KiCad 8.0

---

## 🛠 Features & Hardware Specifications

* **Main MCU:** Raspberry Pi RP2350 (Dual ARM Cortex-M33 @ 150MHz / RISC-V Hazard3).
* **IMU Sensor:** High-precision 6-DOF Gyro & Accelerometer via high-speed SPI bus (BMI160 / MPU6000 compatible).
* **Power Supply:** 
  * High-efficiency low-noise LDO (`AMS1117-3.3` / `TP554302`).
  * On-board ESD protection on USB lines (`USB_C_Receptacle_USB2.0_16P`).
* **Flash Memory:** Winbond `W25Q32JVSS` 32Mb (4MB) Quad-SPI NOR Flash for logs and firmware storage.
* **Connectivity & I/O:**
  * Dedicated high-speed SPI/I2C/UART headers for receiver (SBUS/CRSF/ELRS), GPS, and Telemetry.
  * Multi-channel PWM/DShot outputs for ESC control.
  * On-board status LEDs (Power, Status, Error).

---

## 📐 PCB Specifications

* **Dimensions:** Standard 20x20mm / 30.5x30.5mm mounting hole layout.
* **Layers:** 2-Layer / 4-Layer PCB with optimized Ground Planes for low EMI/noise.
* **Copper Thickness:** 1 oz / 2 oz.

---

## 📂 Repository Structure

```text
├── Hardware/
│   ├── Schematic/          # KiCad Schematic files (.kicad_sch)
│   ├── Layout/             # KiCad PCB Layout files (.kicad_pcb)
│   ├── Gerber/             # Fabrication output files for PCB manufacturing
│   └── Bill_of_Materials/  # BOM component lists (.csv / .xlsx)
├── Images/                 # Schematic screenshots & 3D Render views
└── README.md
