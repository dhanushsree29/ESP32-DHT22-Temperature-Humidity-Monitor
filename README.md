# ESP32-DHT22-Temperature-Humidity-Monitor

IoT temperature and humidity monitoring using an ESP32 and DHT22 sensor.

## About the Project

This project is a simple IoT-based temperature and humidity monitoring system using an ESP32 development board and a DHT22 sensor.

The DHT22 sensor measures the surrounding temperature and relative humidity. The ESP32 processes the sensor readings and displays them on the Arduino IDE Serial Monitor.

## Components Used

- ESP32 Development Board
- DHT22 Temperature and Humidity Sensor
- Breadboard
- Jumper Wires
- USB Cable
- Computer with Arduino IDE

## Hardware Connection

The DHT22 sensor data pin is connected to:

- DHT22 DATA → ESP32 GPIO 26
- DHT22 VCC → ESP32 3.3V
- DHT22 GND → ESP32 GND

> Note: Check the pin labels on your particular DHT22 module before making the connections.

## Software Requirements

- Arduino IDE
- ESP32 Board Support Package
- DHT Sensor Library

## How It Works

1. The ESP32 initializes the DHT22 sensor.
2. The sensor measures temperature and humidity.
3. The ESP32 reads the sensor values every 2 seconds.
4. The readings are displayed on the Serial Monitor.
5. If the sensor cannot provide a valid reading, an error message is displayed.

## Arduino Code

The Arduino source code is available in:

`ESP32_DHT22.ino`

The program uses the DHT library and reads the DHT22 sensor connected to GPIO 26.

## Example Output

```text
IoT Temperature & Humidity Monitoring

Temperature: 28.50 °C
Humidity: 65.20 %
----------------------

Temperature: 28.70 °C
Humidity: 64.80 %
----------------------

Temperature: 29.00 °C
Humidity: 64.10 %
----------------------
