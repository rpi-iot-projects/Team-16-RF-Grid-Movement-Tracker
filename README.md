
# RF Grid Movement Tracker

A touchless 2D movement tracking and drawing pad prototype using RF technology.

## Table of Contents

- [Overview](#overview)  
- [Hardware Components](#hardware-components)  
- [Software and Dependencies](#software-and-dependencies)  
- [Usage](#usage)  
- [Results and Demonstration](#results-and-demonstration)  

## Overview

This project demonstrates a touchless 2D movement tracking system using RFID technology. The goal is to track motion across a grid of RFID tags and display it live on a web interface. It offers an alternative to traditional input methods like pressure or touch, providing a cost-effective and efficient solution that can be used for applications such as digital drawing pads, accessibility devices, and movement controllers.

Key features:
- Real-time 2D position tracking
- MQTT communication for fast data transmission
- Live web visualization via Node-RED and custom HTML/CSS/JS
- Touchless interaction using RFID technology

## Hardware Components

- 1 × RFID Reader (RC522)
- 12 × Passive RFID Tags (mounted on a clipboard in a grid formation)
- 1 × Raspberry Pi Model 3B (system controller and data transmitter)
- Several Jumper Wires (connection between RFID reader and Raspberry Pi GPIO pins)
- 1 × Clipboard with Grid Layout (physical platform for RFID tags)
- 1 × External Monitor (for Raspberry Pi terminal interface)
- 1 × Laptop (Node-RED Host & Web Display)
- 1 × Keyboard (for Raspberry Pi)
- 1 × Mouse (for Raspberry Pi)

## Software and Dependencies

- **Programming Languages:** Python 3, HTML, JS, CSS
- **Libraries and Tools:**
  - Raspberry Pi Terminal
  - Node-RED (with MQTT broker)
  - Mosquitto MQTT Broker
  - Custom HTML, CSS, and JavaScript for the web visualization
  - WebSocket Communication (via Node-RED node)
  - Web browser for live interface display

## Usage

1. Connect the RFID Reader (RC522) to the Raspberry Pi via jumper wires.
2. Arrange and secure 12 passive RFID tags onto a clipboard in a grid layout.
3. Run the attached custom Python script on the Raspberry Pi to read RFID tag data.
4. Send the RFID data via MQTT to the Node-RED server running on a laptop.
5. Node-RED processes incoming messages and updates the custom web interface using WebSocket communication.
6. View live position updates and create drawings based on RFID tag movements directly in a web browser.

## Results and Demonstration

The final prototype successfully tracked position changes across the RFID tag grid and displayed them live on a custom web page. Although there were initial challenges during the live demo, the team resolved technical issues and produced a working integrated system afterward. The drawing pad allows users to interact in a touchless manner and visually trace movements on the grid.

Demonstration videos of the final prototype and testing are available here:  
[Google Drive Link](https://drive.google.com/drive/folders/1sSi9nSDxqp_Yd4aQeGOnyo5cW3OfIJ2k?usp=sharing)
