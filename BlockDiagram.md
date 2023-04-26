---
title: Block Diagram
---

# 8.0 Block Diagram
## 8.1 Current Block Diagram

![Figure 8A: Block Diagram.](/photos/Figure8B.png "Figure 8A: Block Diagram.")

## 8.2 Block Diagram Overview
The team has divided the project into several subsystems, each responsible for a specific task to achieve the overall project requirements. The ESP32 is responsible for communication between the microcontroller and the internet. The PIC19(L)F67K40 is the microcontroller that manages the overall system logic, receives input from the sensors, and sends commands to the motor controller. The TC74A4 is a temperature serial sensor responsible for measuring the temperature, while the AS7343L-DLGM is a light serial sensor that measures light intensity. The motor controller is a serial actuator responsible for controlling the motor's speed and direction. All the major components used in the project are surface mount and operate at a system logic-level voltage of 3.3V. To meet the project requirements, the system uses at least two serial sensors and one serial actuator, using SPI and I2C for communication. The system also uses UART for communicating with the ESP32 and has at least one example of SPI or I2C or both. Finally, to achieve board-to-web duplex communication over WiFi, the ESP32 is responsible for communicating with the internet and exchanging data between the board and the web interface. Together, all these subsystems work in tandem to ensure the project requirements are met, and the system functions as intended.

[click here to return to index](/index)
