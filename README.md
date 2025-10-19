# STM32-Based Wireless Sensor Communication System

## Transmitter Unit
<img src="https://github.com/user-attachments/assets/c853c86e-0aac-4d26-a05f-9c6ded325c01" alt="Transmitter_Unit" width="250">

## Receiver Unit
<img src="https://github.com/user-attachments/assets/fc87a098-cec9-4c04-bf27-daf66ecdc136" alt="Receiver_Unit" width="250">

## Overview
- This project is a wireless sensor communication system built around the **STM32F411VE** microcontroller.
- The system consists of two main units: a **Transmission Unit (PTX)** and a **Receiver Unit (PRX)** that communicate wirelessly using the **NRF24L01 transceiver module**.
- The PTX gathers real-time data from a **MAX30102 Heart Rate/SpO2 sensor** and a **NEO-6M GPS module**. This data is then transmitted to the PRX.
- As a fail-safe, all sensor data is simultaneously logged to an **SD card** on the transmitter side.
- The PRX receives the data and displays it on a **graphical LCD display**.
- Additionally, this system also features bi-directional communication, allowing a user to send commands back to the PTX to remotely enable or disable sensors using push buttons.

## Hardware Components

### Transmitter Unit (PTX)
* **MCU:** STM32F411VE Development Board
* **Transceiver:** NRF24L01 Modules 
* **Health Sensor:** MAX30102 Heart Rate & SpO2 Module 
* **GPS:** NEO-6M GPS Module 
* **Storage:** Micro SD Card Module 

### Receiver Unit (PRX)
* **Display:** 2-inch Graphical LCD (ST7789V)

## Software
- STM32CubeIDE (Code in Bare Metal)

## Usage
1.  **Open the projects:** The repository contains two projects in Code folder: `Transmitter_Unit` and `Receiver_Unit`. Open them in STM32CubeIDE.
2.  **Build the code:** Right-click on each project and select "Build Project".
3.  **Flash the firmware:**
    * Connect the ST-Link to the **Transmitter Unit** board and flash the transmitter firmware.
    * Connect the ST-Link to the **Receiver Unit** board and flash the receiver firmware.

## Project Contributors:
- Nalin Saxena (nasa7792)
- Abhirath Koushik (abhirathkoushik-cub)
