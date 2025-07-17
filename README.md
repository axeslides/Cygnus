# Cygnus
Looking into how control systems like audrino and it's working in tandum with other modules to better understand they're functions 
Laptop Cooling System using Arduino

Project Overview

This project implements a compact temperature-controlled cooling system for laptops or electronic devices using an Arduino UNO, DHT sensors, relay modules, and external fans. The primary objective is to maintain a cooler environment beneath the laptop by dynamically controlling two external fans based on temperature readings.

Features

Real-time temperature monitoring using two sensors (DHT11 and DHT22)

Automatic control of two external fans via relay modules

Adjustable activation logic based on ambient and localized temperature differences

Visual feedback via Arduino's built-in LED to indicate fan activity

Modular design for future expansion (e.g., Peltier cooling modules)


Hardware Used

Arduino UNO (or compatible board)

DHT11 sensor (for ambient temperature measurement)

DHT22 sensor (for triggering temperature measurement)

2-Channel Relay Module

Two 12V DC Fans

Power source (Laptop USB port, Lenovo ThinkCentre USB, or external adapter)

Connecting wires and breadboard


How It Works

DHT11 sensor records ambient room temperature.

DHT22 sensor records the immediate temperature under the laptop.

When the under-laptop temperature exceeds a certain threshold above the ambient, one or both fans activate:

Fan 1 turns on at +4°C above ambient

Fan 2 turns on at +7°C above ambient


LED indicator blinks faster or slower based on fan activation.

System automatically adapts to varying ambient room temperatures.

Optional: future updates may include PWM control and Peltier modules.


Setup Instructions

1. Wire the sensors and relays according to the provided circuit diagram.


2. Upload the Arduino code from the /code directory to your Arduino board.


3. Power the Arduino and fans via a reliable 12V source.


4. Monitor serial output for debugging and temperature readings.


5. Place the cooling system under your laptop and observe dynamic fan control.

