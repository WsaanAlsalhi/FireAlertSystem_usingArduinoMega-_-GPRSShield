# Fire Alert System using Arduino Mega and GPRS Shield

## Overview
This project uses an **Arduino Mega** with a **GPRS Shield (SIM900/SIM800)** to send **SMS alerts** when a fire is detected. The system can be integrated with a fire sensor (like a smoke or flame sensor) to automatically notify a predefined phone number.

---

## Features
- Sends SMS alerts: `"Warning: Fire detected!"`.
- Compatible with **Arduino Mega**.
- Uses **Serial1** for reliable communication with the GPRS Shield.
- Works with any GSM-enabled SIM card with SMS credit.

---

## Hardware Required
- Arduino Mega 2560
- GPRS Shield (SIM900 or SIM800)
- Fire or smoke sensor (optional for automatic detection)
- Jumper wires
- Power source (USB or external 5V/2A recommended for GPRS Shield)
- SIM card with SMS capability and sufficient balance

---

## Circuit Connections
| Arduino Mega Pin | GPRS Shield Pin |
|-----------------|----------------|
| 18 (TX1)        | RX             |
| 19 (RX1)        | TX             |
| GND             | GND            |

> Make sure the SIM card is active and not PIN-protected.

---

## Software Setup
1. Open Arduino IDE.
2. Upload the `FireAlert.ino` code.
3. Modify the phone number in the code:
   ```cpp
   String phoneNumber = "+96891234567"; // Replace with your number
