Project: Web Server Implementation on ESP32 Board.
College: JNN College of Engineering, Shimoga (VTU).

This repository contains the firmware code and implementation architecture for an asynchronous IoT web server built as part of an academic mini-project. The goal was to establish a standalone local network node capable of monitoring environmental telemetry parameters in real time.

Technical Details:
- Microcontroller: ESP32 NodeMCU development board (built-in Wi-Fi station mode)
- Sensor interface: DHT22 Digital Temperature and Humidity Sensor
- Development environment: Arduino IDE (C/C++ firmware configuration)
- Communication layer: HTTP local network routing
- Key libraries: ESPAsyncWebServer and WiFi.h libraries (enabling non-blocking request cycles)

System Architecture:
The firmware initializes the ESP32 Wi-Fi module to hook into a designated local access gateway. Once an automated local IP address is established via DHCP, the controller boots a background server listening on TCP port 80. The interface processes incoming HTTP GET requests asynchronously, parsing active environmental values directly into a responsive client browser view without interrupting core hardware execution loops.

I have uploaded our group's official project synopsis presentation slides as reference documentation in this repository.
