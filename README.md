# Autonomous-robot-using-Arduino-and-ultrasonic-sensor

# Obstacle Avoidance Robot Code 

## Overview

This Arduino code is designed for an obstacle avoidance robot using an ultrasonic sensor. The robot has two sets of motors for the left and right wheels. It uses the NewPing library to interface with the ultrasonic sensor and detect obstacles. The code instructs the robot to move forward and perform an obstacle avoidance maneuver when an obstacle is detected.

## Pin Configuration

- **MLa (Left Motor 1st Pin):** Connects to the positive terminal of the left motor.
- **MLb (Left Motor 2nd Pin):** Connects to the negative terminal of the left motor.
- **MRa (Right Motor 1st Pin):** Connects to the positive terminal of the right motor.
- **MRb (Right Motor 2nd Pin):** Connects to the negative terminal of the right motor.
- **TRIGGER_PIN (Ultrasonic Sensor Trigger Pin):** Connects to the trigger pin on the ultrasonic sensor.
- **ECHO_PIN (Ultrasonic Sensor Echo Pin):** Connects to the echo pin on the ultrasonic sensor.

## Setup

1. Connect the motors and ultrasonic sensor to the specified pins on your Arduino board.
2. Install the NewPing library in the Arduino IDE.
3. Upload the provided code to your Arduino using the Arduino IDE.

## Functionality

The robot operates based on the following conditions:

- **Edge Detection:** If an obstacle is detected within a specified distance, the robot stops, performs an avoidance maneuver, and continues moving forward.



# Line Follower Robot Code 

## Overview

This Arduino code is designed for a line follower robot using infrared (IR) sensors. The robot has two sets of motors for the left and right wheels, and it uses IR sensors to detect the presence or absence of a line. The code instructs the robot to follow the line based on the sensor inputs.

## Pin Configuration

- **MLa (Left Motor 1st Pin):** Connects to the positive terminal of the left motor.
- **MLb (Left Motor 2nd Pin):** Connects to the negative terminal of the left motor.
- **MRa (Right Motor 1st Pin):** Connects to the positive terminal of the right motor.
- **MRb (Right Motor 2nd Pin):** Connects to the negative terminal of the right motor.
- **IR_Left (IR Sensor on the Left):** Connects to the digital output pin of the left IR sensor.
- **IR_Right (IR Sensor on the Right):** Connects to the digital output pin of the right IR sensor.

## Setup

1. Connect the motors and IR sensors to the specified pins on your Arduino board.
2. Upload the provided code to your Arduino using the Arduino IDE.

## Functionality

The robot operates based on the following conditions:

- **Stop:** If both IR sensors detect a line (HIGH), the robot stops.
- **Left Turn:** If the left IR sensor does not detect a line (LOW) while the right IR sensor detects a line (HIGH), the robot turns left.
- **Right Turn:** If the left IR sensor detects a line (HIGH) while the right IR sensor does not detect a line (LOW), the robot turns right.
- **Forward:** If both IR sensors do not detect a line (LOW), the robot moves forward.

