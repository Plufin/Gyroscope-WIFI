# MPU6050 and ESP-NOW Data Transmission with TFT Display

In collaboration with [Protomosh](https://github.com/Protomosh)

This project demonstrates a simple implementation of data transmission using the MPU6050 accelerometer sensor and ESP-NOW protocol, with real-time visualization on a TFT display. The code is written for an ESP32 device.
Representation for LEDs see code [here](https://github.com/Plufin/Motion-controlled-RGB-ring)

## Components Used

- MPU6050 accelerometer sensor
- ESP32 board
- TFT display

## Libraries Required

- Adafruit_MPU6050: Library for interfacing with the MPU6050 sensor.
- TFT_eSPI: Library for controlling the TFT display.
- ESP-NOW: Library for communication between ESP32 devices.


## Project Overview

This project combines the functionalities of the MPU6050 sensor and ESP-NOW communication to send accelerometer and gyroscope data wirelessly. The data is then displayed in real-time on a TFT display.

### MPU6050 Configuration

- The code initializes the MPU6050 sensor, sets its range and filter bandwidth, and displays the configuration details.

### ESP-NOW Setup

- ESP-NOW is initialized, and a peer is registered for data transmission.

### TFT Display

- The TFT display is configured using the TFT_eSPI library.
- Accelerometer and gyroscope data are read from the MPU6050 sensor and displayed on the TFT screen.
- The displayed data includes speed (acceleration in the X-axis), steering (gyroscope rotation in the Z-axis), and a randomly generated mode.

### Data Transmission

- The collected data is sent via ESP-NOW to a receiving ESP32 device.
