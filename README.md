Name:SANDEEP S
Company:CODETECH IT SOLUTIONS
ID:CT06DG25
domain:EMBEDDED SYSTEM
Duration:June 10th toJuly 25th

Project Title:
Bluetooth-Controlled Home Automation System
 Objective:
To design and implement a Bluetooth-based system that allows the user to wirelessly switch home electrical appliances ON and OFF using a smartphone and an Arduino microcontroller.

 Project Concept:
This home automation system leverages Bluetooth communication to receive control commands from a mobile phone and uses an Arduino to interpret those commands and trigger relays, which control the connected electrical devices (like a fan, bulb, or TV).

🛠️ Hardware Components:
Component	Description
Arduino UNO/Nano	Main controller that processes commands
HC-05 Bluetooth Module	Enables wireless communication with phone
Relay Module (5V)	Acts as a switch to control AC appliances
Smartphone	Used to send control signals via Bluetooth
Power Supply (5V)	Powers the Arduino and modules
Resistors (1kΩ and 2kΩ)	For voltage level shifting on HC-05 RX
AC appliances	Lamps, fans, etc., to be controlled
Jumper wires, breadboard	For prototyping connections

 Working Principle:
The smartphone connects to the HC-05 Bluetooth module.

The user sends commands (1, 0, etc.) via a Bluetooth terminal app.

The HC-05 receives these signals and passes them to the Arduino via UART.

The Arduino reads the command and turns ON/OFF the relay module accordingly.

The relay switches the connected appliance ON or OFF based on the command.

🔌 Circuit Diagram (Text Description):
HC-05 VCC → Arduino 5V

HC-05 GND → Arduino GND

HC-05 TX → Arduino RX (Pin 0)

HC-05 RX ← Arduino TX (Pin 1) via a 1kΩ/2kΩ voltage divider

Relay IN → Arduino Pin 8

Relay VCC → Arduino 5V

Relay GND → Arduino GND

Relay COM/NO connected to appliance AC wire

If you want an image of this schematic, I can generate one—just ask.

 Software Requirements:
Arduino IDE – for uploading code to Arduino.

Bluetooth Terminal App (Android) – to send commands (e.g., "1" for ON, "0" for OFF).

 Mobile App Setup:
Download Bluetooth Terminal HC-05 or Arduino Bluetooth Controller.

Pair your phone with HC-05 (password: 1234 or 0000).

Connect in the app and send:

1 → Turns ON the device

0 → Turns OFF the device

 Advantages:
Wireless control without the internet

Cost-effective solution for smart homes

Simple and expandable to multiple devices

Easy to use and build

 Applications:
Control lights, fans, or TVs

Elderly or disabled support system

Office and industrial automation (basic)

