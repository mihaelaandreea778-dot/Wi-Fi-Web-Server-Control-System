# Wi-Fi-Web-Server-Control-System


Overview

This project implements a local web server using an ESP32 microcontroller configured as an Access Point (AP). It allows users to control hardware components (LEDs/GPIOs) remotely through a web browser interface.
Features

Standalone Access Point: 
  -  Creates its own Wi-Fi network (SSID: "Echipa_GM") for direct connection.
  -  Interactive Web Interface: Hosted HTML page with dynamic CSS-styled buttons for real-time control.
  -  Dual Channel Control: Independent management of GPIO 26 and GPIO 2 states.
  -  Live Feedback: Displays the current ON/OFF status of the outputs directly on the web page.

Technologies Used

  -  ESP32
  -  mbedded C / Arduino
  -  Wi-Fi Library (Asynchronous Server)
  -  HTML/CSS
  -  GPIO Control

How It Works

The ESP32 initializes as an Access Point and starts a web server on port 80. When a client connects to the IP address, the server parses HTTP GET requests. Depending on the request, the microcontroller toggles the digital state of the pins and updates the HTML interface to reflect the changes.

Project Contribution

As part of this laboratory assignment, my contribution focused on:

  -  Web Server Implementation: Configuring the ESP32 to handle incoming HTTP client requests.
  -  GPIO State Management: Developing the logic to parse commands and toggle hardware pins (26 and 2).
  -  UI/UX Design: Creating the HTML structure and CSS styling for the control buttons and status display.
