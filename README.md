<div align="center">
    <h1 id="Header">PiCar-Control-System-Performance</h1>
</div>

## Overview

```
Note: This was my final project for my Engineering Design class I took at WashU with a team of 2.
```

The PiCar is a robotic platform powered by a Raspberry Pi, which serves as its primary control unit. This project integrates multiple sensors and actuators to achieve precise control and autonomous movement. The system employs PID control to meet the objectives of Control, Movement, and Movement with Control, ensuring optimal performance in speed, direction, and distance tracking.

<div align="center">
    <img src="PiCar-figure-1.png" alt="screenshot" width="400px" height="300px">
    <img src="PiCar-figure-2.png" alt="screenshot" width="400px" height="300px">
</div>

## Key features Include
* A Raspberry Pi-based control system
* Ultrasonic sensor for obstacle detection (the "eyes")
* Camera for object recognition and tracking (the "mouth")
* DC motor for rear-wheel drive
* Three servomotors for steering, head movement, and tilt
* Analog-to-Digital Converter (ADC) for data acquisition
* Advanced power management via a PWM HAT

## Technologies/Tools Used
* Hardware: Raspberry Pi, Ultrasonic Sensor, Camera, DC Motor, Servomotors, ADC, PWM HAT
* Software: Python, PID Control Algorithm
* Development Tools: Raspberry Pi GPIO, FFT Analysis Tools
* Sensors: Ultrasonic sensor, Photoresistor, LEDs
* Power Management: Battery system with LED indicators and PWM HAT integration

## Functionality and Results
* Control
  * Designed and implemented a PID control system to regulate the motor speed in a no-load environment.
  * Achieved steady velocity at 5 RPS with a steady-state error of 0.071 and an overshoot of -24.8%.
  * Analyzed the system's performance using velocity-time plots and FFT for steady-state verification.
 
* Movement
  * Developed a program to drive the PiCar toward a blue object positioned at least 10 feet away.
  * Used an ultrasonic sensor for distance tracking and speed adjustment.
  * Implemented a camera-angle-tracking algorithm for precise steering via servos.

* Movement with Control
  * Combined PID control and camera tracking for enhanced precision.
  * Maintained a constant speed of 5 RPS while tracking and pathing to the target object.
  * Addressed dynamic system challenges, achieving a steady-state error of 0.188 and overshoot of 29.0%.

* Conclusion
  * This project successfully demonstrated the importance of fine-tuning PID coefficients:
  * Kp balances stability and responsiveness.
  * Ki addresses steady-state errors while maintaining stability.
  * Kd dampens oscillations and reduces noise.

If you would like to know more about our "PiCar-System-Control-Performance" project, checkout:
```
Final_Report_ESE205.pdf
```
