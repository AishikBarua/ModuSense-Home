# 📅 Day 11 — Native Android App Architecture & ESP32 API Communication

## 📌 Objective
Understand how a native Android application is structured and how it communicates with an ESP32-based smart home system using APIs.

---

## ⏱ Time Allocation (1.5 Hours)

| Time | Topic |
|----|----|
| 10 min | Role of mobile app |
| 10 min | Native Android choice |
| 20 min | App architecture |
| 15 min | Navigation & UI flow |
| 15 min | Device discovery |
| 20 min | ESP32 API communication |
| 10 min | Security basics |

---

## 🔹 Why a Mobile App is Required

A mobile application enables:
- User-friendly control
- Remote monitoring
- Device management
- Data visualization

📌 **Interview Line**  
> A mobile app acts as the primary user interface for smart home systems.

---

## 🔹 Why Native Android?

Native Android is preferred because:
- Better performance
- Stable Bluetooth (BLE) support
- Direct access to system hardware
- More reliable network handling

📌 **Interview Line**  
> Native Android provides better hardware access and stability for IoT applications.

---

## 🔹 High-Level Android App Architecture

UI Layer
│
├── ViewModel / Business Logic
│
├── Network Layer (API)
│
└── Device Manager
