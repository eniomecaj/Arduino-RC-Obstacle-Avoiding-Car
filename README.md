# Arduino RC Obstacle-Avoiding Car

This is an Arduino-powered obstacle-avoiding robot car designed as a personal engineering project to develop and showcase hands-on skills in electronics, programming, and embedded system design. It uses an ultrasonic sensor to detect objects and autonomously navigate around them using a motor driver and two DC motors.

## Features

- Autonomous obstacle avoidance using an HC-SR04 ultrasonic distance sensor  
- Motor control via L298N H-Bridge driver  
- Powered by Arduino Uno (or compatible)  
- Adjustable detection range via code  
- Expandable with features like Bluetooth, line-following, or app control

## Bill of Materials

| Component              | Quantity | Notes                                    |
|------------------------|----------|------------------------------------------|
| Arduino Uno            | 1        | Or compatible microcontroller             |
| L298N Motor Driver     | 1        | Controls 2 DC motors                      |
| HC-SR04 Ultrasonic Sensor | 1     | For obstacle detection                    |
| DC Motors (with wheels)| 2        | Gear motors preferred                     |
| Chassis Base           | 1        | Can be custom or off-the-shelf            |
| 18650 or 9V Battery    | 1        | + battery holder                          |
| Jumper Wires           | Several  | Male-to-male and male-to-female           |
| Breadboard or PCB      | Optional | For tidy wiring or prototyping            |

## Circuit Diagram

📸 *[Insert Fritzing-style diagram or schematic image here]*

## Wiring Overview

- **HC-SR04**  
  - VCC → 5V  
  - GND → GND  
  - Trig → D9  
  - Echo → D10  

- **L298N**  
  - IN1 → D2  
  - IN2 → D3  
  - IN3 → D4  
  - IN4 → D5  
  - ENA / ENB → 5V (or use PWM pins for speed control)

- **Motors**  
  - Left motor → OUT1 & OUT2  
  - Right motor → OUT3 & OUT4

- **Power**  
  - External battery to L298N motor power input  
  - 5V from Arduino to L298N logic power

## Arduino Code


