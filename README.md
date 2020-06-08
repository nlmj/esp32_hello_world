<!-- # Hello World Example

Starts a FreeRTOS task to print "Hello World"

See the README.md file in the upper level 'examples' directory for more information about examples. -->
# Hello World

My first ESP32 program. This project uses the sample Hello World from esp-idf examples. 

## Motivation
Installing and setting up esp-idf environment for future development. Install [esp-idf](https://docs.espressif.com/projects/esp-idf/en/stable/get-started/) following espressif documentation.

## Tools
macOS Cataline Version 10.15.5 \
ESP-IDF v4.2-dev-1660-g7d7521367 

## Problems and Solutions

Mac couldn't detect the port connecting to ESP32. Lacking driver
Solution: Install [CP210x VCP Driver](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers). [Github discussion](https://github.com/espressif/arduino-esp32/issues/1084).

Mac couldn't detect the port connecting to ESP32 even after installing the driver. Faulty Cable.
Solution: Replace cable. I used a USB Type C to Type A converter to a USB Type A to Micro USB.

