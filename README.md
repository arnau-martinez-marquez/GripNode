# GripNode

GripNode is a compact telemetry device based on **ESP32** designed for vehicles (cars and motorcycles).  
It records motion (IMU), position (GPS), and speed, storing all data on a microSD card for later analysis.

---

## Features

- ESP32-based system
- IMU sensor for acceleration and rotation data
- GPS for position, speed, and time
- microSD logging (CSV format)
- Modular and extensible firmware (C / PlatformIO)

---

## Hardware

- ESP32 development board
- IMU sensor (MPU6050 / MPU9250 or similar)
- GPS module (NEO-6M / NEO-M8N or similar)
- microSD card module

---

## Firmware

The project uses **PlatformIO** with C code structure.

Main modules:
- `main.c` → system loop
- `imu.c` → motion sensor handling
- `gps.c` → GPS parsing
- `sd_logger.c` → data logging

---

## Data Format

Example CSV output:
