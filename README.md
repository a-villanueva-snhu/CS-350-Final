# Smart Thermostat Prototype (CS350)

## Overview

This project is a prototype smart thermostat developed as the final project for an Embedded Systems course. 
The goal was to design and implement the low-level functionality of a connected thermostat using a Raspberry Pi and various hardware peripherals. 
The system reads ambient temperature from an AHT20 sensor, allows the user to adjust a target temperature using GPIO buttons, 
indicates heating or cooling status with LEDs, displays system information on an LCD, and simulates cloud communication through UART output.

The thermostat is implemented as a finite state machine with three operating modes: **OFF**, **HEAT**, and **COOL**. 
This project demonstrates embedded software development, hardware interfacing, and system architecture analysis.

## Technologies Used

* Raspberry Pi 5
* Python 3
* GPIOZero / lgpio
* I²C (AHT20 Temperature Sensor)
* UART Serial Communication
* 1602 LCD Display
* GPIO LEDs and Push Buttons

---

## Reflection

### Project Summary

This project solved the problem of creating a functional smart thermostat prototype capable of monitoring room temperature, 
accepting user input, controlling heating and cooling indicators, and simulating communication with a cloud server. 
The project also included evaluating hardware architectures for a future production version with integrated Wi-Fi connectivity.

### What I Did Well

One of the strongest aspects of this project was organizing the thermostat as a finite state machine. 
Separating the OFF, HEAT, and COOL operating modes simplified the control logic and made the software easier to understand and extend. 
I also successfully integrated multiple hardware interfaces, including GPIO, I²C, UART, and the LCD display, into a single application.

<img width="605" height="711" alt="cs 350 final state machine drawio" src="https://github.com/user-attachments/assets/213335da-b0b6-4887-b511-f88fe1479ca6" />


### Where I Could Improve

Given more time, I would improve the software by separating hardware drivers, state logic, and user interface code into independent modules. 
I would also add more robust error handling for sensor failures and expand the cloud simulation to use an actual network protocol such as MQTT or HTTP instead of UART.

### Tools and Resources

This project introduced me to several embedded development tools and libraries, including GPIOZero, lgpio, Adafruit's CircuitPython sensor libraries, 
and Raspberry Pi hardware documentation. These resources will continue to be valuable for future embedded and IoT projects.

### Transferable Skills

This project strengthened my understanding of finite state machine design, embedded software architecture, 
peripheral communication protocols (GPIO, I²C, and UART), hardware/software integration, and evaluating hardware platforms 
based on technical and business requirements. These skills directly apply to embedded systems, robotics, IoT devices, and other software engineering projects.

### Maintainability, Readability, and Adaptability

The project was designed using clear state definitions, descriptive variable names, modular functions, and 
comments explaining key functionality. Using a finite state machine made the control logic predictable and easy to modify. 
The hardware interfaces were implemented using standard libraries, making it easier to adapt the software to different sensors or future hardware platforms.
