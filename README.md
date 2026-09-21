# ES-EXP-7
# EXP — INTERFACING A 16×2 LCD WITH ARDUINO USING AN I2C MODULE FOR SENSOR DATA DISPLAY

## Aim

To interface a **16×2 LCD display with Arduino using an I2C module** and display sensor data on the LCD.

## Objectives

- To understand the operation of a 16×2 LCD.
- To interface the LCD with Arduino using an I2C module.
- To reduce the number of GPIO pins required for LCD communication.
- To read sensor data using Arduino.
- To display the sensor readings on the LCD.

## Hardware / Software Tools Required

### Hardware

- Arduino UNO
- 16×2 LCD Display
- I2C LCD Module (PCF8574-based)
- DHT11 Temperature and Humidity Sensor
- Breadboard
- Jumper wires
- USB cable

### Software

- Arduino IDE
- Arduino C/C++ programming language
- LiquidCrystal_I2C library
- DHT sensor library

## Components

### 16×2 LCD
### I2C Module
### Circuit Connections
### I2C Communication
### Working Principle

1. The DHT11 sensor measures temperature and humidity.
2. Arduino reads the sensor values through the digital data pin.
3. The Arduino processes the received sensor data.
4. The processed values are sent to the LCD through the I2C interface.
5. The LCD displays the temperature on one line.
6. The humidity is displayed on the second line.
7. The readings are periodically updated.

## Arduino Program
```
#include <LiquidCrystal.h>

// LCD pins: RS, EN, D4, D5, D6, D7
LiquidCrystal lcd(7, 6, 5, 4, 3, 2);

void setup() {
  lcd.begin(16, 2);

  lcd.setCursor(0, 0);
  lcd.print("EMBEDDED");
}

void loop() {
  
}
```
##Observation

<img width="1600" height="719" alt="image" src="https://github.com/user-attachments/assets/950b687e-0a85-4f1e-8237-11237ee8e459" />
<img width="899" height="1599" alt="image" src="https://github.com/user-attachments/assets/58a39160-40f4-4de7-8aeb-8c969b614e21" />


##Result

Thus, the **16×2 LCD was successfully interfaced with Arduino UNO using an I2C module**, and the temperature and humidity values obtained from the DHT11 sensor were successfully displayed on the LCD. The experiment demonstrates the use of **I2C communication for efficient sensor-data display** in embedded and IoT applications.
