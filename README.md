A wearable smart heating solution designed to monitor ambient and internal temperatures and dynamically regulate warmth using heating foils — controlled by a LilyPad microcontroller and temperature sensors.

## Project Overview

This project focuses on enhancing comfort in cold environments through a **Smart Heating Jacket**. It integrates:

- **DHT sensors** to measure both *internal* (inside the jacket) and *external* (ambient) temperatures.
- **Heating foil** to distribute controlled heat inside the jacket.
- **LilyPad microcontroller**, a wearable Arduino-compatible board ideal for textile integration.

## Features

- Textile-friendly with wearable electronics (LilyPad)
- Dual-temperature sensing (inside and outside)
- Automatic heat control based on temperature difference
- Energy-efficient regulation
- Modular code for easy expansion

## How It Works

1. The DHT sensors continuously monitor the temperature inside the jacket and the ambient temperature outside.
2. If the internal temperature is significantly lower than the target threshold (or in comparison with the outside), the LilyPad activates the **heating foil**.
3. The heat is distributed through the foil embedded in the jacket lining, raising the internal temperature gradually.
4. The system ensures that the heating stops when optimal comfort is achieved.

## Hardware Components

| Component           | Quantity | Description                              |
|--------------------|----------|------------------------------------------|
| LilyPad Arduino    | 1        | Wearable microcontroller board           |
| DHT11/DHT22 Sensor | 2        | One for internal, one for external temp  |
| Heating Foil       | 1        | Thin foil for warmth distribution        |
| Power Source       | 1        | LiPo battery or equivalent               |
| Connecting Wires   | -        | For sensor and foil connections          |

## Repository Structure
📦 Smart-Heating-Jacket/
API.ino               # Handles temperature reading and heating logic
LilyPad_2sensors.ino  # Integrates LilyPad control and sensors
README.md             # Project documentation

## Getting Started

### Prerequisites

- Arduino IDE
- Libraries:
  - `DHT` sensor library (`DHT.h`)

### Uploading the Code

1. Open either `.ino` file in Arduino IDE.
2. Connect your LilyPad Arduino to your computer.
3. Select the correct board and port under **Tools**.
4. Upload the sketch.

### Wiring Guide

- **DHT Sensors**: Connect VCC to 3.3V, GND to GND, and signal to digital pins.
- **Heating Foil**: Connect via MOSFET or relay to control with digital output pin.
- Ensure adequate insulation and safety precautions.



