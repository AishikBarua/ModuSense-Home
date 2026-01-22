# Day-10: ESP32 Setup & First Firmware Upload (Arduino IDE)

## Objective
The goal of Day-10 was to set up the ESP32 development environment using **Arduino IDE**, successfully upload the first firmware, and verify serial communication. This day establishes the foundation for all future hardware and IoT development.

---

## Development Environment

- **IDE:** Arduino IDE 2.x
- **Board Package:** ESP32 by Espressif Systems
- **ESP32 Board:** ESP32 Dev Module
- **Operating System:** Windows
- **Upload Tool:** esptool v5.1.0
- **Baud Rate:** 115200

---

## ESP32 Board Configuration

The following configuration was used in Arduino IDE:

| Setting | Value |
|------|------|
| Board | ESP32 Dev Module |
| Port | COM5 |
| Upload Speed | 115200 |
| CPU Frequency | 240MHz (WiFi/BT) |
| Flash Frequency | 40MHz |
| Flash Mode | DIO |
| Flash Size | 4MB |
| Partition Scheme | Default |

---

## First Test Program (Hello ESP32)

```cpp
void setup() {
  Serial.begin(115200);
  delay(1000);
  Serial.println("ESP32 Upload OK");
}

void loop() {

Program Explanation

Serial.begin(115200) initializes UART communication.

delay(1000) ensures serial port stability after reset.

Serial.println() confirms successful firmware execution.

loop() is intentionally empty for this test.

Firmware Upload Result
Compilation Output
Sketch uses 281487 bytes (21%) of program storage space.
Global variables use 20848 bytes (6%) of dynamic memory.

Flashing Output
Writing at 0x00010000...
Hash of data verified.
Leaving...
Hard resetting via RTS pin...


This confirms that the firmware was written correctly to flash memory, verified, and the ESP32 was reset to execute the new program.

Serial Monitor Verification

Baud Rate: 115200

Output:
ESP32 Upload OK


This confirms:

ESP32 booted successfully

setup() function executed

Serial communication is working properly

Issues Faced & Solutions
Issue: Serial Write Timeout / COM Port Busy

Cause:

COM port locked by another process

Serial Monitor open during upload

Windows USB driver conflict

Solution:

Closed Serial Monitor before upload

Reconnected ESP32 USB cable

Restarted Arduino IDE / PC

Held BOOT button during upload when required

Key Learnings

ESP32 programs are stored in external flash memory.

Manual BOOT mode may be required for flashing.

Baud rate must match between code and Serial Monitor.

Serial Monitor is essential for debugging embedded systems.

Stable hardware setup is critical before sensor integration.
  // Empty loop
}
