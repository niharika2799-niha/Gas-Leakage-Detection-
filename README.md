Gas Leakage Detection and Automatic Off System
Overview
The Gas Leakage Detection and Automatic Off System is a safety-focused embedded solution designed to detect hazardous gas leaks using an MQ2 sensor and automatically activate safety mechanisms. When a leak is detected, the system alerts the surroundings using a buzzer, turns off electrical appliances through a relay module, and closes the gas regulator using a servo motor. Built using **Arduino Nano**, this project aims to prevent accidents in residential, commercial, and industrial environments.

Features
* **Real-Time Gas Detection** using MQ2 sensor
* **Automatic Regulator Shutoff** using servo motor
* **Immediate Audible Alert** through buzzer activation
* **Electrical Appliance Shutdown** via relay module
* **Fast Response to LPG, Methane, CO leaks**
* **Low-cost, reliable hardware components**

Installation
1. Clone the Repository
bash
git clone https://github.com/yourusername/gas-leakage-detection-system.git
cd gas-leakage-detection-system

2. Install Arduino IDE
Download from: [https://www.arduino.cc/en/software](https://www.arduino.cc/en/software)

3. Install Required Libraries
In Arduino IDE, install:
Servo.h
```
4. Upload Code to Arduino Nano
1. Connect Arduino Nano using USB
2. Open `.ino` file
3. Select:
   * Board: **Arduino Nano**
   * Processor: **ATmega328P (Old Bootloader)**
4. Click **Upload**

Configuration
Hardware Connections

| Component    | Arduino Pin |
| ------------ | ----------- |
| MQ2 Sensor   | D2          |
| Buzzer       | D3          |
| Relay Module | D4          |
| Servo Motor  | D5          |

Adjustable Parameters (in code)
You can modify:
* Servo rotation angle
* Threshold gas detection level
* Buzzer or relay behavior

Usage
After uploading the code and powering the Arduino Nano:
1. **MQ2 detects gas leakage**
2. If gas level crosses threshold:
   * Buzzer activates
   * Relay turns OFF electrical appliances
   * Servo motor rotates to close regulator
3. If gas level returns to normal:
   * Buzzer stops
   * Relay restores appliances
   * Servo resets to original position

Run the System
Just power the Arduino using:
* USB
* 5V adapter
* External battery

Project Structure
gas-leakage-detection-system/
├── code/
│   └── gas_detection.ino        # Main Arduino program
├── hardware/
│   ├── circuit-diagram.png      # Optional schematic
│   ├── block-diagram.png
├── documentation/
│   └── project-report.pdf       # Complete report
├── README.md                    # Documentation

Components Used
* Arduino Nano
* MQ2 Gas Sensor
* Relay Module
* Servo Motor
* Buzzer
* Connecting wires
* Power supply


sion**, **advanced README**, or **GitHub badges**, I can generate them too.
