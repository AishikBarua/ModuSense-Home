# 📅 Day 10 — ESP32 Connectivity (Wi-Fi, Bluetooth, Pairing & Security Basics)

## 📌 Objective
Understand how ESP32 connects to mobile applications and networks using Wi-Fi and Bluetooth, and learn basic pairing and security concepts required for smart home systems.

---

## ⏱ Time Allocation (1.5 Hours)

| Time | Topic |
|----|----|
| 10 min | Importance of connectivity |
| 15 min | ESP32 connectivity options |
| 25 min | Wi-Fi fundamentals |
| 25 min | Bluetooth (BLE) fundamentals |
| 20 min | Pairing & security basics |

---

## 🔹 Why Connectivity Matters in Smart Home Systems

Connectivity enables:
- Remote monitoring
- Mobile app control
- Automation
- Multi-device coordination

📌 **Interview Line**  
> Connectivity enables communication between devices, users, and cloud services in smart home systems.

---

## 🔹 ESP32 Connectivity Options

ESP32 supports:
- **Wi-Fi**
- **Bluetooth Classic**
- **Bluetooth Low Energy (BLE)**

This makes ESP32 suitable for IoT and smart home hubs.

---

## 🔹 Wi-Fi on ESP32

### Wi-Fi Modes
| Mode | Description |
|----|------------|
| Station (STA) | Connects to router |
| Access Point (AP) | ESP32 creates network |
| AP + STA | Both simultaneously |

### Smart Home Use
- ESP32 connects to home router
- Mobile app communicates over local network or internet

📌 **Interview Line**  
> Wi-Fi is used for high-bandwidth and internet-based communication.

---

## 🔹 Bluetooth (BLE) on ESP32

### Why BLE?
- Low power consumption
- Short range
- Secure pairing

### Smart Home Use
- Device discovery
- First-time setup
- Local configuration

📌 **Interview Line**  
> BLE is ideal for device discovery and initial pairing in IoT systems.

---

## 🔹 Device Discovery & Pairing

### Discovery Process
1. ESP32 advertises itself
2. Mobile app scans nearby devices
3. User selects the device

### Pairing
- Secure connection established
- Credentials exchanged

📌 Used mainly during first-time setup.

---

## 🔹 Communication Flow

