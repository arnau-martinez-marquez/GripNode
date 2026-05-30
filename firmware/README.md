# GripNode

GripNode is a compact ESP32-based device designed for collecting vehicle telemetry data in cars and motorcycles. It records motion, position, and speed using an IMU and GPS, storing everything on a microSD card.

---

## Features

* ESP32 microcontroller
* IMU sensor (acceleration + gyroscope)
* GPS for position and speed
* microSD card logging (CSV format)
* Wi-Fi / Bluetooth support (future use)

---

## Hardware

* ESP32
* IMU (MPU6050 / MPU9250 or similar)
* GPS module (NEO-6M / NEO-M8N or similar)
* microSD module

---

## Data Output

CSV log example:

```
timestamp,lat,lon,speed,ax,ay,az,gx,gy,gz
2025-01-01T12:00:00Z,41.3851,2.1734,45.3,0.12,-0.05,9.81,0.01,0.02,0.00
```

---

## Installation

```bash
git clone https://gitlab.com/your-group/gripnode.git
cd gripnode
pio run
```

Upload firmware:

```bash
pio run --target upload
```

---

## Goal

A simple, low-cost and open telemetry device for vehicles.

---

## License

MIT
