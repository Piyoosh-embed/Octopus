# Octopus
This is my first project using an embedded system.
**Project Overview**
Octopus is a specialized PCB card designed for diagnostic and monitoring purposes in Variable Message Sign (VMS) displays. It provides real-time status updates for VMS units consisting of 10, 12, or 14 rows, each built using a matrix of 150, 180, or 210 LED P10 modules (32x16). In addition to VMS diagnostics, the Octopus PCB card offers comprehensive environmental monitoring by tracking temperature, humidity, door status, shock detection, and light intensity. The current temperature is displayed directly on the card using a 7-segment display. Moreover, the card is capable of controlling an AC exhaust fan, ensuring efficient thermal management of the system.

**Features**
1. VMS Diagnostic Capability: Monitors and reports the status of Variable Message Sign displays.
2. Environmental Monitoring: Tracks temperature, humidity, light intensity, door status, and shock detection for comprehensive system monitoring.
3. Temperature Display: Displays real-time temperature readings via a 7-segment display integrated on the PCB.
4. AC Exhaust Fan Control: Automates the operation of an AC exhaust fan for efficient thermal management based on environmental conditions.
5. Multi-row Status Reporting: Provides detailed status updates for up to 14-row VMS displays, ensuring optimal system performance.
6. Data Communication via IP: Shares diagnostic and environmental data over IP using a specific port, enabling seamless integration with web applications for remote monitoring.
7. Supports TCP/IP and UDP Protocols: Offers flexible data transmission through both TCP/IP and UDP protocols, providing reliable and real-time communication to external systems.
8. Versatile Monitoring Options: Enables monitoring of physical and environmental parameters to ensure safe and stable operations in dynamic environments.
**Hardware Components**
1. ATmega2560: The core microcontroller responsible for processing inputs from sensors and managing communication protocols.
2. Sensors:
   . Temperature and Humidity Sensor: Monitors environmental conditions to provide real-time data for temperature and humidity levels.
   . Door Status Sensor: Detects whether doors are open or closed, ensuring secure system operations.
   . Shock Sensor: Monitors physical shocks or vibrations for added safety and damage prevention.
   . Light Intensity Sensor: Measures ambient light levels to adjust display settings or trigger alerts.
3. Other Components:
   . Ethernet Module (W5100): Facilitates network communication, enabling the PCB to share data via IP over TCP/IP and UDP protocols.
   . 7-Segment Display (TM1637): Displays real-time temperature and status updates directly on the PCB.
   . Real-Time Clock (RTC DS3231): Provides accurate timekeeping for time-stamped logging and scheduled operations.
   . GPS Module: Captures location data, useful for tracking or geographically specific operations.

**Software Setup**
1. Development Environment:
   . The software for the Octopus PCB is developed using the Arduino Framework within the Arduino IDE tool, providing an accessible and flexible environment for embedded programming.
2. Libraries Used: Several core libraries from the Arduino IDE repository are used for sensor interfacing, communication, and display control. These include-
   Ethernet, TM1637Display, DHT, RTClib
   External GitHub Repository Libraries: Additional specialized libraries are sourced from GitHub repositories to extend functionality, such as- Libraries for the GPS Module for location tracking, Libraries to enhance networking capabilities and TCP/IP, UDP communication.

**Configuration**
Adjust the system settings (sensor thresholds) in the configuration file. Set up communication parameters.
   

