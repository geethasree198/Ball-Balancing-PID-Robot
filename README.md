# Ball Balancing PID Controlled Robot

An Arduino-based one-dimensional ball balancing robot that uses an HC-SR04 ultrasonic sensor for position measurement, a servo motor as the actuator, and a PID controller for closed-loop stabilization.

## 📌 Project Overview

This project demonstrates the practical implementation of a closed-loop PID control system for stabilizing a ball at a desired position on a movable platform.

The HC-SR04 ultrasonic sensor continuously measures the position of the ball. The Arduino UNO processes this measurement, calculates the error between the actual position and the desired setpoint, and applies a Proportional-Integral-Derivative (PID) control algorithm.

The resulting control signal is sent to a servo motor, which tilts the platform and moves the ball back toward the desired position.

## 🎯 Objectives

- Design and implement a one-dimensional ball balancing system.
- Measure ball position using an HC-SR04 ultrasonic sensor.
- Implement a PID controller using Arduino UNO.
- Control the platform angle using a servo motor.
- Maintain the ball near a desired setpoint.
- Test the system's response to external disturbances.

## 🛠️ Hardware

- Arduino UNO
- HC-SR04 Ultrasonic Sensor
- Servo Motor
- Ball balancing platform

## 💻 Software

- Arduino IDE
- Embedded C / Arduino C++
- PID Control Algorithm

## 🧠 Control Algorithm

The system uses a Proportional-Integral-Derivative (PID) controller.

### Proportional (P)

The proportional term generates a corrective response based on the current error between the desired and measured ball position.

### Integral (I)

The integral term accumulates the error over time and helps reduce steady-state error.

### Derivative (D)

The derivative term responds to the rate of change of the error and helps reduce overshoot and oscillations.

## ⚙️ System Workflow

1. The HC-SR04 ultrasonic sensor measures the ball's position.
2. Arduino UNO receives the distance measurement.
3. The current position is compared with the desired setpoint.
4. The position error is calculated.
5. The PID controller calculates the required correction.
6. The servo motor adjusts the platform angle.
7. The ball moves toward the desired position.
8. The process continuously repeats as a closed-loop system.

## 📊 Experimental Results

The physical prototype was successfully tested for:

- Setpoint tracking
- Disturbance rejection
- Stability
- Overshoot and oscillation

The prototype demonstrated stable balancing and was able to return the ball toward the setpoint after small and medium disturbances.

## 🔧 PID Implementation

The Arduino implementation calculates:

- Position error
- Integral of the error
- Derivative of the error
- PID control output

The servo position is then adjusted according to the calculated PID output.

## 🔮 Future Scope

- Extend the system to two-dimensional ball-and-plate balancing.
- Implement automatic PID parameter tuning.
- Integrate camera-based computer vision for more accurate position detection.
- Explore advanced control strategies.

## 📄 Project Report

The complete project report is available in:

`Project_Report/Ball_Balancing_PID_Robot.pdf`

## 👥 Project Members

- Geetha Sree
- Sadurthram Manivel
- Jerom Jason A

## 🏫 Institution

Vellore Institute of Technology  
School of Electronics Engineering (SENSE)
