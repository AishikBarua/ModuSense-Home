# 📅 Day 06 — Communication Protocols (UART, I2C, SPI)

## 📌 Objective
Understand why communication protocols are required in embedded systems and learn the basics of **UART**, **I2C**, and **SPI**, including when and why each is used in a smart home system.

---

## ⏱ Time Allocation (1.5 Hours)

| Time | Topic |
|----|----|
| 20 min | Why communication protocols exist |
| 30 min | UART |
| 20 min | I2C |
| 15 min | SPI |
| 5 min | Self-evaluation |

---

## 🔹 Why Communication Protocols Exist

### The Problem
GPIO pins can only:
- Read ON/OFF states
- Read simple analog values

They **cannot**:
- Transfer structured data
- Communicate with complex sensors or displays
- Support multiple devices efficiently

### The Solution
**Communication protocols** define standardized rules for:
- How data is sent
- When data is sent
- How devices understand each other

📌 **Interview Definition**  
> Communication protocols define the rules for reliable data exchange between electronic devices.

---

## 🔹 UART (Universal Asynchronous Receiver-Transmitter)

### What is UART?
UART is a **point-to-point**, asynchronous communication protocol using:
- TX (Transmit)
- RX (Receive)

No clock signal is required.

### Characteristics
| Feature | Description |
|------|------------|
| Devices | 2 only |
| Pins | TX, RX |
| Speed | Medium |
| Use case | Debugging, logs, serial communication |

### UART in Smart Home Systems
- ESP32 debugging
- Serial monitor output
- Configuration messages

📌 **Interview Line**  
> UART is commonly used for debugging and simple serial communication between two devices.

---

## 🔹 I2C (Inter-Integrated Circuit)

### What is I2C?
I2C is a **two-wire**, multi-device communication protocol using:
- SDA (Data)
- SCL (Clock)

Each device has a unique address.

### Characteristics
| Feature | Description |
|------|------------|
| Devices | Multiple |
| Pins | SDA, SCL |
| Speed | Low to Medium |
| Use case | Sensors, OLED displays |

### I2C in Smart Home Systems
- Temperature sensors
- Humidity sensors
- OLED displays

📌 **Interview Line**  
> I2C allows multiple devices to communicate using only two wires through addressing.

---

## 🔹 SPI (Serial Peripheral Interface)

### What is SPI?
SPI is a **high-speed**, synchronous communication protocol using:
- MOSI
- MISO
- SCK
- CS

### Characteristics
| Feature | Description |
|------|------------|
| Devices | Few |
| Pins | 4+ |
| Speed | High |
| Use case | Displays, flash memory |

### SPI in Smart Home Systems
- TFT displays
- External memory modules

📌 **Interview Line**  
> SPI is used when high-speed data transfer is required.

---

## 🔹 Protocol Selection Logic

| Component | Protocol |
|--------|----------|
| Simple sensor | GPIO |
| Analog sensor | ADC |
| Multiple sensors | I2C |
| Display | I2C / SPI |
| Debugging | UART |

📌 This selection logic is the foundation of **protocol detection and data routing**.

---

## 🔹 Self-Evaluation Checklist

- [ ] I understand why protocols are needed
- [ ] I can explain UART, I2C, and SPI
- [ ] I know when to use each protocol
- [ ] I can explain protocol choice in interviews

---

## 🧠 Key Takeaway
> Communication protocols enable structured, reliable, and scalable data exchange in embedded systems.

---

## 🚀 Next Step
**Day 07:** Displays, UI output, and visualization in embedded systems.
