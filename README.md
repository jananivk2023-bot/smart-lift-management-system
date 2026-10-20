 # Smart Lift Management System

An IoT-driven elevator automation and scheduling solution designed to optimize lift dispatching, minimize passenger wait times, and enable secure, real-time telemetry monitoring.

## Overview

Conventional elevator dispatching systems often result in long waiting times, redundant trips, and uneven passenger distribution. This project implements a microcontroller-based smart elevator management system that dynamically monitors passenger demand, controls floor access through RFID authentication, and transmits system status data to the cloud for real-time monitoring and simulation.

## Key Features

- **Dynamic Proximity & Presence Sensing:** Uses HC-SR04 ultrasonic sensors to detect passenger presence and monitor lift position.
- **Secure Access Control:** Integrates RFID authentication to enable restricted or prioritized floor access.
- **Cloud Telemetry & Logging:** Synchronizes lift status, current floor, and passenger traffic data with Firebase Realtime Database.
- **Real-Time Passenger Feedback:** Displays system status, direction of travel, and arrival notifications using an I2C LCD.
- **Simulation Validation:** Tests firmware logic through simulated elevator load and passenger traffic scenarios.

## Tech Stack & Hardware Components

- **Microcontroller:** ESP32 (Dual-Core Wi-Fi Microcontroller)
- **Firmware Development:** Embedded C/C++ (Arduino Framework)
- **Sensors & Actuators:** HC-SR04 Ultrasonic Sensor, RC522 RFID Module, 16x2 I2C LCD Display
- **Cloud & Networking:** Firebase Realtime Database, Wi-Fi (HTTP/REST)
- **Simulation Tools:** Wokwi / Tinkercad / Proteus

## Circuit & Pin Configuration

| Component | ESP32 Pin | Interface |
|-----------|-----------|-----------|
| HC-SR04 (Trig/Echo) | GPIO 5 / GPIO 18 | Digital GPIO |
| RC522 RFID Module | GPIO 21 (SDA), GPIO 19 (SCK), GPIO 23 (MOSI), GPIO 18 (MISO) | SPI |
| LCD Display (16x2) | GPIO 22 (SCL), GPIO 21 (SDA) | I2C |
| Status LED / Buzzer | GPIO 2 / GPIO 4 | Digital Output |

## Documentation Status

Physical prototype schematics, simulation models, and firmware source files will be uploaded upon completion of the final documentation.
