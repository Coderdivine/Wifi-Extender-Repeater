---

# WiFi Extender/Repeater

Welcome to the WiFi Extender/Repeater project! This project utilizes an ESP32 to create a WiFi extender that can repeat an existing WiFi signal, extending its range. The project is developed using the Arduino IDE.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Configuration](#configuration)
- [Usage](#usage)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The WiFi Extender/Repeater project is designed to help you extend the range of your WiFi network using an ESP32 microcontroller. This can be particularly useful in large homes or areas with weak WiFi signals.

## Features

- **Extend WiFi Range**: Amplifies and extends the range of an existing WiFi network.
- **Easy Setup**: Simple configuration using the Arduino IDE.
- **Open Source**: Completely open source and customizable.

## Hardware Requirements

To build this project, you will need:

- An ESP32 development board
- USB cable for programming the ESP32
- A computer with the Arduino IDE installed
- Breadboard and jumper wires (optional for initial testing)nstalled in the Arduino IDE (Instructions [here](https://github.com/espressif/arduino-esp32))

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Coderdivine/Wifi-Extender-Repeater.git
   cd Wifi-Extender-Repeater
   ```
## Configuration

1. **Edit Configuration File**

   Open the `Wifi-Extender-Repeater.ino` file in the Arduino IDE and update the following lines with your network credentials:

   ```cpp
   const char* ssid = "Your_SSID";           // Replace with your WiFi SSID
   const char* password = "Your_PASSWORD";   // Replace with your WiFi password
   const char* ext_ssid = "Extender_SSID";   // SSID for the extended network
   const char* ext_password = "Extender_PASSWORD"; // Password for the extended network
   ```

2. **Upload the Code**

   Connect your ESP32 board to your computer and upload the code using the Arduino IDE.

## Usage

1. **Power the ESP32**

   Once the code is uploaded, power the ESP32 using a USB cable or an external power source.

2. **Connect to the Extended Network**

   Your ESP32 should now be acting as a WiFi extender. Connect to the `Extender_SSID` network using the password you configured.

## Troubleshooting

- **Cannot Connect to the ESP32**: Ensure your credentials are correct and the ESP32 is within range of your main WiFi network.
- **Weak Signal**: Place the ESP32 in a location where it can receive a strong signal from your main router and still cover the desired extension area.
- **Reboot Issues**: If the ESP32 keeps rebooting, check for power supply issues or incorrect configurations in the code.

## Contributing

We welcome contributions! Please fork this repository, create a new branch, and submit a pull request with your changes.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
