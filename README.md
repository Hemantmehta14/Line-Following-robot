# ESP32 Line Following Robot

## Overview

This project is an autonomous Line Following Robot built using the ESP32 microcontroller, IR sensor array, and dual motor driver modules. The robot detects a predefined path and continuously adjusts motor speeds to stay aligned with the line, demonstrating real-time sensor processing, embedded control systems, and robotic navigation.

---

## Features

* Autonomous line tracking
* ESP32-based control system
* Real-time IR sensor processing
* Differential motor speed control
* Compact and low-cost design
* Rechargeable battery-powered operation
* Suitable for robotics competitions and educational projects

---

## Hardware Components

| Component                                      | Quantity    |
| ---------------------------------------------- | ----------- |
| ESP32 Development Board                        | 1           |
| IR Sensor Array Module                         | 1           |
| Motor Driver Module (L298N / MX1508 / Similar) | 2           |
| DC Gear Motors                                 | 4           |
| Robot Chassis                                  | 1           |
| Wheels                                         | 4           |
| Rechargeable Li-ion Batteries                  | 2           |
| Battery Holder                                 | 1           |
| Buck Converter (LM2596)                        | 1           |
| Perfboard / Prototype PCB                      | 1           |
| Connecting Wires                               | As Required |
| Power Switch                                   | 1           |

---

## Working Principle

1. The IR sensor array continuously monitors the surface beneath the robot.
2. A dark line absorbs infrared light while the surrounding surface reflects it.
3. Sensor readings are processed by the ESP32.
4. Based on the detected line position, the ESP32 adjusts motor speeds.
5. The robot moves left, right, or straight to remain centered on the path.
6. This feedback loop enables autonomous navigation.

---

## System Architecture

```text
IR Sensor Array
        |
        v
      ESP32
        |
        v
  Motor Driver Modules
        |
        v
      DC Motors
        |
        v
 Robot Movement Control
```

---

## Pin Connections

### IR Sensor Array

| Sensor Output | ESP32 Pin |
| ------------- | --------- |
| S1            | GPIO 32   |
| S2            | GPIO 33   |
| S3            | GPIO 25   |
| S4            | GPIO 26   |
| S5            | GPIO 27   |

### Motor Driver

| Driver Pin | ESP32 Pin |
| ---------- | --------- |
| IN1        | GPIO 18   |
| IN2        | GPIO 19   |
| IN3        | GPIO 21   |
| IN4        | GPIO 22   |

> Modify according to your actual wiring.

---

## Software Requirements

* Arduino IDE
* ESP32 Board Package
* Embedded C/C++
* USB Driver for ESP32

---

## Applications

* Robotics Competitions
* Autonomous Navigation Systems
* Educational Robotics
* Embedded Systems Learning
* Path Tracking Research

---

## Future Improvements

* PID Control Implementation
* Obstacle Avoidance
* Bluetooth Control
* Wi-Fi Monitoring
* Machine Vision Integration
* Maze Solving Capability

---

## Project Outcomes

* Successfully implemented autonomous path tracking.
* Achieved real-time line detection using IR sensors.
* Developed motor control algorithms using ESP32.
* Demonstrated practical applications of embedded systems and robotics.

---

## Technologies Used

* ESP32
* Arduino IDE
* Embedded C++
* IR Sensors
* Motor Drivers
* Autonomous Robotics

---

## Author

**Hemant Mehta**

Embedded Systems | IoT | Robotics | PCB Design
