# Embedded-projects
All the projects that we have performed were posted here with codes and documentation, so whenever anyone require help can take help from this and also question us issues that you are facing.We surely try to answer you.

This document provides a step-by-step guide on setting up communication between two ESP32 boards using the Controller Area Network (CAN) protocol with SN65HVD230 transceiver modules. The communication is implemented using the CAN library in the Arduino IDE.
1. Wiring Connections
Connect the components as follows:
ESP32 to SN65HVD230 (for both sender and receiver)

ESP32 Pin |  SN65HVD230 Pin
----------|----------------
3.3V	| VCC
GND	| GND
GPIO5  |	TXD
GPIO4  | 	RXD



SN65HVD230 to SN65HVD230 Connections

SN65HVD230 (Sender)  |    SN65HVD230 (Receiver)
---------------------|-------------------------
CANH  |  CANH
CANL  |  CANL   
GND   |  GND

    

2. Installing the CAN Library

(1.)Open Arduino IDE.

(2.)Go to Sketch -> Include Library -> Manage Libraries.

(3.)Search for "CAN" and install the Arduino-CAN library that supports ESP32 version 1.0.6.

-->If the communication not works than you can try loopback test for both the ESP32 boards one by one.The loopback test code is attached here and connections are given below.

ESP32 Pin      SN65HVD230 Pin
3.3V     -->    VCC
GND      -->    GND
GPIO4    -->    TXD
GPIO5    -->    RXD

