# Car Black Box System 🚗

## 📌 Project Overview

The Car Black Box (CBB) is a microcontroller-based embedded system designed to continuously monitor and log critical driving events for post-incident analysis. Inspired by black boxes used in aviation, this system is tailored for automotive environments to track anomalies such as over-speeding, sudden braking, or system faults.

The project uses a PIC16F877A microcontroller with peripherals like potentiometers as analog input sources, and stores event data into EEPROM for non-volatile logging.

## 🚦 Key Features

- Real-time monitoring of driving conditions
- Detection and logging of events like over-speeding
- Event logging in EEPROM with timestamps
- Peripheral interaction using ADC (speed simulation via potentiometer)
- Efficient interrupt-based system design
- Extendable for GPS, crash sensor, or communication modules

## 🧠 Pre-requisites

To work on or understand this project, knowledge in the following areas is essential:

- PIC microcontroller programming (PIC16F877A)
- Microcontroller schematics and interfacing
- Peripheral handling using ADC (potentiometer)
- Interrupt Service Routines (ISR)
- Familiarity with MPLAB X IDE and XC8 compiler

## 🔧 Tools & Technologies

- **Microcontroller:** PIC16F877A
- **Software:** MPLAB X IDE, XC8 Compiler
- **Communication:** UART (for debug output)
- **Storage:** EEPROM (internal)
- **Peripherals:** Potentiometer (speed simulation), LEDs

## 🧰 File Structure

- `main.c` — Main application logic and event loop
- `adc.c / adc.h` — ADC initialization and reading functions
- `eeprom.c / eeprom.h` — EEPROM read/write operations
- `uart.c / uart.h` — UART communication for debug output
- `config.h` — Configuration bits and system settings

## ⚙️ How It Works

1. ADC reads potentiometer value to simulate vehicle speed
2. System continuously monitors the speed value
3. If speed crosses threshold — event is logged into EEPROM
4. UART outputs the logged data for debugging
5. Data persists in EEPROM even after power off

## ⚙️ How to Compile & Run

1. Open project in **MPLAB X IDE**
2. Select **XC8 compiler**
3. Build the project
4. Flash to PIC16F877A board
5. Monitor output via UART terminal

## What I Learned

- EEPROM interfacing and non-volatile data storage
- ADC configuration and analog signal reading
- Interrupt-based embedded system design
- UART communication for debugging
- Real-world automotive embedded system concepts

## Author

**Miryala Vamshi**  
Embedded Systems Engineer  
📧 vamshimiryala2@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/vamshi-miryala-a7b71a347)
