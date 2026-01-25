# ESP32 Sensors & Communication Protocols  
**Day 21 – Day 22**

This phase focuses on understanding how ESP32 interacts with the physical world using sensors and communication protocols.  
The goal was to build **clear mental models**, not just connect wires.

---

## 🔹 Day 21: Sensor Fundamentals (ESP32 Perspective)

### What I Learned

A sensor does **not** send temperature, gas, or motion directly to ESP32.  
A sensor converts a **physical quantity into an electrical signal** (voltage or logic level), which ESP32 then processes.

ESP32 only understands:
- Voltage levels (via ADC)
- Digital logic (HIGH / LOW)

---

### Types of Sensors

#### 1️⃣ Analog Sensors
- Output a **continuous range of voltages**
- ESP32 reads them using **ADC (Analog-to-Digital Converter)**

**Examples:**
- Gas sensors (MQ series)
- Temperature sensors (LM35)
- Light sensors (LDR)

**Concept to remember (must memorize):**
0V → ADC value 0
3.3V → ADC value 4095 (ESP32)
