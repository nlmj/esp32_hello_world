<!-- # Hello World Example

Starts a FreeRTOS task to print "Hello World"

See the README.md file in the upper level 'examples' directory for more information about examples. -->
# Hello World

My first ESP32 program. This project uses the sample Hello World from esp-idf examples. \
Directory: ~/esp/hello_world \
To build and flash: idf.py build && idf.py -p /dev/tty.SLAB_USBtoUART flash


## Motivation
Installing and setting up esp-idf environment for future development. Install [esp-idf](https://docs.espressif.com/projects/esp-idf/en/stable/get-started/) following espressif documentation.

## Tools

macOS Cataline Version 10.15.5 \
ESP-IDF v4.2-dev-1660-g7d7521367 \
ESP32 WROOM\
Adafruit HUZZAH32 Feather

## Problems and Solutions

Mac couldn't detect the port connecting to ESP32. Lacking drivers. [Github discussion](https://github.com/espressif/arduino-esp32/issues/1084).\
Solution: Install [CP210x VCP Driver](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers). 

Mac couldn't detect the port connecting to ESP32 even after installing the driver. Faulty Cable.\
Solution: Replace cable. I used a USB Type C to Type A converter to a USB Type A to Micro USB.

idf.py doesn't work after closing terminal after setup.
Solution: macOS Catalina uses zsh terminal. \
Create .zshrc in ~/ directory:
```
$ touch ~/.zhrc
```
Include these lines inside ~/.zhrc:
```
export IDF_PATH=~/esp/esp-idf
export PATH="$IDF_PATH/tools:$PATH"
```
