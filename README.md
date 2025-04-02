# smart-agriculture-iot-system
IoT-based smart greenhouse system using ESP32, Blynk, sensors, pump, UVA light, and LCD.
# 🌱 Smart Agricultural Monitoring System (IoT-Based Greenhouse)

This project is a smart greenhouse system designed using IoT technologies to monitor and control environmental conditions such as soil moisture, humidity, temperature, and light. It features automatic and manual irrigation control, UVA lighting, and live sensor data display via both a mobile app and an LCD screen.

---

## 📌 Project Overview

- **Microcontroller**: ESP32 (Wemos D1 R32)
- **Platform**: Blynk IoT
- **Connectivity**: WiFi
- **Sensors Used**:
  - Soil Moisture Sensor
  - DHT11 (Temperature & Humidity)
  - Rain Sensor
  - TEMT6000 (Light Sensor)
- **Actuators**:
  - Water Pump (controlled via Relay)
  - UVA Light
- **Display**:
  - 20x4 LCD with I2C module

---

## 🎯 Objectives

- Monitor real-time environmental data (soil moisture, humidity, temperature, light).
- Enable remote control of irrigation and UVA lighting through a mobile app.
- Automate water pump operation based on soil moisture thresholds.
- Provide local visual feedback using an LCD screen.

---

## 🔧 System Architecture
Sensors → ESP32 → Blynk Cloud → Mobile App ↓ LCD Display ↓ Water Pump / UVA Light


---

## 📱 Blynk Mobile App Features

- Displays:
  - 🌡️ Temperature (`V0`)
  - 💧 Humidity (`V1`)
  - 🌿 Soil Moisture (`V2`)
  - 🌧️ Rain Sensor (`V4`)
  - ☀️ Light Intensity (`V3`)
- Controls:
  - 🧪 Water Pump ON/OFF (`V6`)
  - 🔆 UVA Light ON/OFF

---

## 💻 Code & Libraries

Make sure the following libraries are installed in your Arduino IDE:

- `Blynk` (New Blynk library)
- `WiFi.h` (comes with ESP32)
- `DHT` by Adafruit
- `LiquidCrystal_I2C` by Frank de Brabander
- `Wire.h` (for I2C LCD)

> You can find the full code in the `code/` directory.



## 🧠 Future Improvements

- Add a real-time clock (RTC) module for time-based operations.
- Add automatic mode with user-defined thresholds through the app.
- Expand to cloud-based data logging and notifications.

![System Overview](images/system_preview.png)


## 🌿 System Overview
![Smart Greenhouse Preview](./system_preview.png)



