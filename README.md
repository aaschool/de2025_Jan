This project focuses on developing an autonomous suitcase system that utilizes robotic technology, machine vision, and sensing capabilities to enhance the travel experience. The suitcase is designed to autonomously follow its user while safely navigating through dynamic environments, such as airports or public spaces.
At the heart of this system is the Obstacle Detection & Reaction System, which I chose as the core section for the development. This system represents a critical safety feature that ensures the suitcase can detect and respond to physical obstacles in real-time.
It is designed to stop the suitcase whenever an obstacle is detected, preventing collisions and creating a safe interaction between the suitcase and its environment.
By prioritizing obstacle detection and response, this subsystem ensures that the suitcase's autonomous features operate safely and effectively within its broader robotic architecture.


Objective of Assignment7 Code:

This code is designed to create a simple obstacle detection and motor control system for an autonomous suitcase. The goal is to ensure the suitcase can:
Keep the motors running when there are no obstacles.
Stop safely when an obstacle is detected within a threshold distance (30 cm).
Indicate obstacle detection visually using an LED.

Key Components Used:

HC-SR04 Ultrasonic Sensor:
Used for measuring the distance to obstacles in front of the suitcase.
It outputs a pulse (TRIG) and listens for the echo (ECHO) to calculate distance.

L298N Motor Driver Module:
Controls two DC motors (left and right) for moving the suitcase forward.
It allows for PWM speed control and direction control (IN1/IN2, IN3/IN4).

Two DC Motors:
One motor on the left wheel and one on the right wheel to propel the suitcase.
Both motors are set to move forward simultaneously in this code.

LED Indicator:
Acts as a visual alert for obstacle detection.
Turns ON when an obstacle is too close, OFF when path is clear.

Arduino Board (e.g., Uno or Nano):
The main controller managing sensor inputs and motor/LED outputs.

Aims of this code:
Continuously reads data from the ultrasonic sensor.
Stops the motors if an obstacle is within 30 cm, preventing a collision.
Keeps the motors running if no obstacle is detected.
Activates an LED warning when stopped due to an obstacle.
