#📡 ESP32 Water Tank Level Monitoring System (Blynk IoT)

This project is an IoT based water tank level monitoring system built using ESP32 and an Ultrasonic Sensor (HC-SR04).
The system measures the water level in a tank and sends the data to the Blynk IoT mobile app, where it is displayed using a Gauge widget.

This allows users to monitor the tank level remotely from their smartphone.

📺 Full Project Explanation Video:
Explanation of the project is available on my YouTube channel.
👉  video link.

🧠 Project Idea

In many homes and buildings, people cannot easily check the water level in overhead tanks.
This project solves that problem by using an ultrasonic sensor to measure the distance between the sensor and water surface.

The ESP32 processes this distance and sends the tank level percentage to the Blynk IoT app, where it is displayed visually.

⚙️ Components Used

-> ESP32 Development Board

-> Ultrasonic Sensor (HC-SR04)

-> Jumper Wires

-> Breadboard

-> Power Supply

-> Smartphone with Blynk IoT App

🔌 Circuit Connections
Ultrasonic Sensor	ESP32
VCC	5V
GND	GND
TRIG	GPIO 5
ECHO	GPIO 18


📱 Blynk IoT Setup

Create a Blynk account

Create a new Template

Add a Datastream

Virtual Pin: V0

Data Type: Integer

Range: 0 – 100

Add a Gauge widget

Assign it to V0

The gauge will display the tank level percentage.

💻 How It Works

The ultrasonic sensor measures the distance between the sensor and water surface.

ESP32 calculates the distance using sound waves.

The distance is converted into tank water level percentage.

ESP32 sends this value to the Blynk Cloud.

The Blynk mobile app displays the level using a Gauge.
