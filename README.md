# ModuSense Home
A Modular ESP32-Based Smart Home Monitoring System

## Overview
ModuSense Home is a beginner-friendly smart home system built using an ESP32 microcontroller. 
It supports multiple sensors, dynamic protocol handling, and wireless communication through
Bluetooth and Wi-Fi, controlled via a native Android application.

This project demonstrates core IoT concepts such as modular firmware design, data routing,
fan-out (data splitting), and mobile integration.

## Key Features
- ESP32-based central control hub
- Multiple sensor support (Analog & Digital)
- Protocol-aware sensor handling
- Bluetooth & Wi-Fi communication
- Native Android application
- Modular and expandable firmware design

## Hardware Components
- ESP32 Dev Board (ESP32-WROOM-32)
- DHT11 / DHT22 (Temperature & Humidity)
- MQ-2 Gas Sensor (Analog)
- PIR Motion Sensor
- Ultrasonic Sensor (HC-SR04)

## System Architecture
Sensors send data to the ESP32 central module. The ESP32 processes, routes, and splits
data to multiple outputs such as the Android application and future platforms.

## Communication
- Bluetooth: Device pairing and short-range control
- Wi-Fi: HTTP-based API communication using JSON

## Firmware Design
- Sensor Manager Module
- Protocol Detection Logic
- Data Routing & Fan-out
- Basic Error Handling
- Expandable architecture

## Android Application
App Name: ModuSense Control

Features:
- Device scanning
- Connectivity mode selection
- Sensor list and dashboard
- Real-time sensor data visualization

## Future Improvements
- Cloud integration (MQTT)
- OTA firmware updates
- User access control
- Automation rules

## Author
Aishik Barua
