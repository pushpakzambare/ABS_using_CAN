# **Automatic Braking System using CAN Protocol 🚗⚙️**

## **Project Overview**
This project implements an **Automatic Braking System (ABS)** using the **Controller Area Network (CAN) protocol** for communication. It is designed to enhance vehicle safety by automatically detecting obstacles and applying the brakes when necessary.

The system consists of:
- **HC-SR04 Ultrasonic Sensor** 🛑 for distance measurement.
- **STM32F407 Microcontroller** 🖥️ for processing sensor data and controlling braking.
- **MCP2551 CAN Transceiver** 🔄 for transmitting data between modules.
- **L298N Motor Driver** 🏎️ for controlling the braking mechanism.
- **Buzzer** 🔊 to alert the driver in case of obstacles.

## **How It Works**
1. The **HC-SR04 ultrasonic sensor** continuously monitors the distance to objects in front of the vehicle.
2. The **STM32F407 microcontroller** processes the sensor data and determines whether a collision is imminent.
3. If an obstacle is detected within a predefined distance:
   - A braking command is sent over the **CAN bus** to another microcontroller.
   - The second microcontroller activates the **L298N motor driver**, which slows down or stops the vehicle.
   - A **buzzer** sounds an alert.
4. The system continuously updates and transmits data over the CAN network for reliable real-time communication.

## **Hardware Requirements**
- STM32F407 Discovery Board (x2)
- HC-SR04 Ultrasonic Sensor
- MCP2551 CAN Transceiver (x2)
- L298N Motor Driver
- DC Motor
- USB to TTL UART Serial Converter (CP2102)
- Resistors (1KΩ, 120Ω)

## **Software Requirements**
- **STM32CubeIDE** (for firmware development)
- **Embedded C Programming** (for microcontroller logic)
- **CAN Protocol Implementation** (for data transmission)

## **Advantages ✅**
- **Improves vehicle safety** by automatically braking in critical situations.
- **Reduces driver fatigue** by assisting with braking.
- **Enhances fuel efficiency** through optimized braking.
- **Uses reliable CAN protocol** for real-time communication.
- **Potentially lowers insurance costs** for vehicles equipped with ABS.

## **Future Enhancements 🚀**
- **Integration with AI** for advanced obstacle detection.
- **Vehicle-to-Vehicle (V2V) communication** for better traffic safety.
- **Smarter braking mechanisms** with adaptive speed control.

