Smart Rainwater Harvesting System
Overview
The Smart Rainwater Harvesting System (SRHS) is designed to automate the collection and filtration of rainwater using Internet of Things (IoT) technologies. Utilizing a Raspberry Pi as the central controller, the system employs various sensors to measure rainfall, water pH levels, and tank water levels. It automatically redirects water flow based on water quality and maintains optimal tank levels. This system is ideal for sustainable water management in residential or commercial buildings.

Features
Rain Detection: Automatically detects the presence of rain to start the water collection process.
pH Measurement: Measures the pH level of the collected water to determine its quality.
Water Level Monitoring: Keeps track of water levels in storage tanks using ultrasonic sensors.
Automatic Water Routing: Uses a servo motor to direct water flow based on pH levels.
Web Server Integration: Sends data to a web server for remote monitoring and control.
Hardware Requirements
Raspberry Pi (Model 3B or newer recommended)
pH sensor with ADC (Analog-to-Digital Converter)
Ultrasonic sensor for water level measurement
Servo motor for controlling water flow
Relay module for controlling the water dispenser
Rainfall detection sensor
Miscellaneous: Breadboard, jumper wires, power supply, etc.
Software Requirements
Raspberry Pi OS or any compatible Linux distribution
Python 3.6 or newer
GPIO Zero library for Raspberry Pi GPIO access
Requests library for HTTP requests
Installation
Setup Raspberry Pi: Install Raspberry Pi OS and ensure it's up to date.

sql
Copy code
sudo apt update
sudo apt upgrade
Install Python Libraries:

Copy code
pip3 install gpiozero requests
Hardware Setup: Connect all sensors and actuators to the Raspberry Pi according to the GPIO pin assignments defined in the code.

Clone Repository:

bash
Copy code
git clone <repository-url>
cd <repository-directory>
Configuration: Adjust the default configurations in the script to match your hardware setup, such as GPIO pin numbers and sensor thresholds.

Usage
To start the system, run the main script:

Copy code
python3 rainwater_harvesting_controller.py
The system will automatically begin monitoring for rain and collecting data. Check the rainwater_harvesting.log file for logs and operational details.

Contributing
Contributions to the SRHS project are welcome! Please fork the repository, make your changes, and submit a pull request.

License
This project is licensed under Anirudh. M et al., - see the LICENSE file/ Research paper for more details.
https://www.ijitee.org/wp-content/uploads/papers/v11i2/B96301211221.pdf