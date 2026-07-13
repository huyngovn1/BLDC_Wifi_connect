# BLDC Motor Controller with ESP32 WiFi

A BLDC motor control and monitoring system developed using the ESP32 WiFi module.

The project combines a three-phase BLDC power stage, gate-driver circuits, an OLED display, and wireless communication. The ESP32 provides WiFi connectivity for remote monitoring, configuration, and motor-control commands.

## Project Overview

The system is designed to control a three-phase brushless DC motor while providing wireless communication through the ESP32.

The ESP32 processes control commands, manages the user interface, displays operating information on the OLED screen, and communicates with external devices through WiFi.

## Hardware Design

<p align="center">
  <img src="https://github.com/user-attachments/assets/d7c5ee4f-0e9b-4a86-bd6e-cb7c18bac1d7" width="600" alt="BLDC WiFi controller hardware">
</p>

<p align="center">
  <i>BLDC motor controller hardware with ESP32 WiFi connectivity.</i>
</p>

## System and PCB Overview

<p align="center">
  <img src="https://github.com/user-attachments/assets/cd053c2d-ae37-4418-abe0-8bd91e36eeee" width="900" alt="BLDC WiFi controller PCB and system overview">
</p>

<p align="center">
  <i>PCB layout and system design of the BLDC WiFi controller.</i>
</p>

## Main Features

- Three-phase BLDC motor control
- ESP32 WiFi connectivity
- Wireless motor-control commands
- Remote system monitoring
- Motor speed control
- OLED status display
- MOSFET gate-driver circuit
- Dedicated power-supply section
- Configurable operating parameters
- PCB and schematic design included

## Main Hardware

The project uses the following main components:

- ESP-WROOM-32 module
- Three-phase MOSFET power stage
- IR2101S MOSFET gate drivers
- LM393 comparator circuit
- 1.3-inch I2C OLED display
- Schottky diodes
- Buck-converter power supply
- Switches and configuration inputs
- BLDC motor connection interface
- Supporting resistors and capacitors

## ESP32 WiFi Communication

The ESP32 provides wireless communication between the motor controller and an external device.

The WiFi system can be used to:

- Connect the controller to a wireless network
- Receive motor-control commands
- Update operating parameters
- Send motor status information
- Display connection status
- Support remote monitoring and control

The communication interface can be expanded using a web server, mobile application, or another WiFi-based control system.

## OLED Display

The OLED screen provides local operating information such as:

- WiFi connection status
- Motor operating state
- Speed or throttle value
- Control mode
- System notifications
- Fault information

## Firmware

The firmware is developed for the ESP32 using C or C++.

The main firmware functions include:

- ESP32 peripheral initialization
- WiFi initialization and connection
- Wireless command reception
- Motor-control command processing
- PWM signal generation
- OLED display control
- System-status monitoring
- Communication timeout handling
- Fault detection
- Main control loop

## Working Principle

1. The system is powered through the main power input.
2. The power-supply circuit provides suitable voltages for the control electronics.
3. The ESP32 initializes WiFi, the OLED display, and the motor-control interface.
4. An external device connects to the controller through WiFi.
5. Motor-control commands are transmitted to the ESP32.
6. The ESP32 processes the commands and generates the required control signals.
7. The gate-driver circuits control the three-phase MOSFET power stage.
8. The operating status is displayed locally and can be transmitted wirelessly.

## Repository Contents

This repository contains:

- Altium schematic files
- PCB layout files
- ESP32 hardware libraries
- Component footprints
- 3D component models
- Manufacturing output files
- Supporting project documents
- README documentation

## Development Tools

- Altium Designer
- Arduino IDE or ESP-IDF
- ESP32 development tools
- C and C++ programming languages
- WiFi-enabled computer or mobile device

## Applications

This project can be used for:

- WiFi-controlled BLDC motors
- Remote motor-monitoring systems
- Smart electric vehicles
- Robotic systems
- Industrial motor controllers
- IoT motor-control applications
- Embedded-system education

## Project Status

The project currently includes the hardware design, PCB layout, component libraries, and WiFi control architecture.

Further development may include:

- Mobile application control
- Web-based control interface
- Real-time speed feedback
- Current and voltage monitoring
- Temperature protection
- Data logging
- MQTT or cloud connectivity

## Safety Notice

This project contains a high-current three-phase power stage.

During testing:

- Use a current-limited power supply.
- Check for short circuits before applying power.
- Test at low voltage first.
- Monitor MOSFET and motor temperature.
- Disconnect the motor before modifying the circuit.
- Use suitable fuses and protective equipment.

## Author

Developed by [huyngovn1](https://github.com/huyngovn1)
