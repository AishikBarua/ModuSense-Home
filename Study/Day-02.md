# 📘 Day 02 – Electrical Basics & GPIO Fundamentals

## 📌 Objective
Understand the **basic electrical concepts** required for embedded systems and learn how **GPIO pins** connect the ESP32 to real-world sensors and devices.

---

## 🧠 Key Concepts Learned

### 1️⃣ Voltage (V)
**Voltage** is the electrical pressure that pushes electric charge through a circuit.

- Measured in volts (V)
- ESP32 typically operates at **3.3V**
- USB power provides **5V**

🔹 Analogy: Voltage is like water pressure in a pipe.

---

### 2️⃣ Current (A)
**Current** is the flow of electric charge through a conductor.

- Measured in amperes (A)
- Depends on voltage and resistance

🔹 Analogy: Current is the amount of water flowing through the pipe.

---

### 3️⃣ Ground (GND)
**Ground** is the reference point (0V) in an electrical system.

Why ground is important:
- Provides a common voltage reference
- Completes the electrical circuit
- Ensures stable and predictable operation

📌 Interview tip:
> Ground provides a common reference point for all voltages in a circuit.

---

### 4️⃣ Digital vs Analog Signals

#### 🔵 Digital Signals
- Two states only: `0` or `1`
- Used for ON/OFF type devices

Examples:
- Motion sensor
- Button
- Relay

