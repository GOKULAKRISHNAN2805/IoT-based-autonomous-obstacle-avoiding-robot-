# 🤖 IoT-Based Obstacle Avoiding Robot with ESP32-CAM Monitoring

An intelligent IoT-based autonomous robotic system designed for obstacle detection, autonomous navigation, real-time wireless control, and live video monitoring using ESP8266, ESP32-CAM, ultrasonic sensors, servo motors, and DC motor drivers.

---

# 📌 Project Overview

This project presents a smart IoT-enabled obstacle avoiding robot capable of autonomous navigation while providing real-time live video streaming through ESP32-CAM.

The robot uses ultrasonic sensing and servo-based directional scanning to detect nearby obstacles and make intelligent navigation decisions automatically.

A custom responsive web dashboard allows users to:

- Control the robot wirelessly
- Monitor live distance data
- Switch between manual and autonomous modes
- Adjust motor speed in real-time
- View live ESP32-CAM video stream

The project combines:

- Embedded Systems
- Robotics
- IoT Communication
- Real-Time Monitoring
- Web-Based Control
- Autonomous Navigation
- Wireless Automation

---

# 🚀 Features

- ✅ Autonomous obstacle avoidance
- ✅ Manual robot control through web dashboard
- ✅ ESP32-CAM live video streaming
- ✅ WiFi-based wireless communication
- ✅ Real-time distance monitoring
- ✅ Servo-based environment scanning
- ✅ PWM motor speed control
- ✅ Auto / Manual mode switching
- ✅ Responsive web interface
- ✅ Embedded C++ programming
- ✅ Differential drive robot navigation
- ✅ Real-time web server control

---

# 🛠 Hardware Components

| Component | Quantity | Purpose |
|---|---|---|
| ESP8266 NodeMCU | 1 | Main robot controller |
| ESP32-CAM | 1 | Live video streaming |
| HC-SR04 Ultrasonic Sensor | 1 | Obstacle detection |
| Servo Motor | 1 | Sensor direction scanning |
| L298N Motor Driver | 1 | Motor control |
| DC Geared Motors | 2 | Robot movement |
| Robot Chassis | 1 | Mechanical body |
| Wheels | 2 | Mobility |
| Battery Pack | 1 | Power supply |
| Jumper Wires | Multiple | Hardware connections |

---

# 💻 Software Requirements

- Arduino IDE
- ESP8266 Board Package
- ESP32 Board Package
- Embedded C++ Programming
- WiFi Libraries
- ESP8266WebServer Library
- Servo Library

---

# 📂 Project Structure

```bash
IoT-Obstacle-Avoiding-Robot/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── code/
│   ├── esp8266_robot_controller.ino
│   ├── esp32_cam_stream.ino
│   └── libraries.txt
│
├── images/
│   ├── robot-front.png
│   ├── robot-top.png
│   ├── testing-environment.png
│   ├── esp32-stream.png
│   └── circuit-diagram.png
│
└── docs/
    └── Project_Report.pdf
```

---

# ⚙️ System Architecture

The proposed system consists of:

- Sensor Module
- Processing Unit
- Motor Control Unit
- Wireless Communication Module
- Real-Time Monitoring Module
- Web-Based Dashboard

---

# 🧠 Working Principle

The robot operates using a continuous sensing and decision-making process.

## 1️⃣ Obstacle Detection

The HC-SR04 ultrasonic sensor continuously measures the distance between the robot and nearby obstacles.

The servo motor rotates the sensor to scan:
- Left side
- Right side
- Front direction

---

## 2️⃣ Data Processing

ESP8266 processes sensor data and compares obstacle distances with predefined threshold values.

---

## 3️⃣ Decision Making

Based on obstacle conditions:

- Clear path → Move forward
- Obstacle detected → Stop
- Left side clear → Turn left
- Right side clear → Turn right
- All sides blocked → Reverse and re-evaluate

---

## 4️⃣ Motor Control

The L298N motor driver controls:
- Forward movement
- Reverse movement
- Left turning
- Right turning
- Speed control using PWM

---

## 5️⃣ Real-Time Monitoring

ESP32-CAM streams live video over WiFi using an embedded web server.

Users can remotely monitor the robot environment through any browser.

---

# 🌐 IoT Communication

The project uses WiFi communication for:
- Wireless robot control
- Live sensor monitoring
- Real-time video streaming
- Dashboard communication

---

# 📡 Communication Protocols

| Protocol | Purpose |
|---|---|
| TCP/IP | Network communication |
| HTTP | Web dashboard communication |
| WiFi | Wireless connectivity |

---

# 🔌 Pin Configuration

## ESP8266 Connections

| Component | ESP8266 Pin |
|---|---|
| IN1 | D1 |
| IN2 | D2 |
| IN3 | D3 |
| IN4 | D4 |
| TRIG | D5 |
| ECHO | D6 |
| Servo Signal | D7 |

---

# ⚠ Important Hardware Note

The HC-SR04 ultrasonic sensor Echo pin outputs 5V.

ESP8266 GPIO pins support only 3.3V.

A voltage divider or logic level converter must be used between:

```text
HC-SR04 Echo → ESP8266 D6
```

to prevent damage to the ESP8266.

---



---

# 💻 Source Code

The project contains two major embedded programs.

| File | Description |
|---|---|
| esp8266_robot_controller.ino | Main robot control system |
| esp32_cam_stream.ino | ESP32-CAM video streaming |

---

# ⚙️ Features Implemented in Code

- WiFi Web Server
- Real-Time Robot Control
- Autonomous Obstacle Avoidance
- Servo-Based Direction Scanning
- PWM Speed Control
- Live Distance Monitoring
- JSON Data Communication
- Responsive Web Dashboard
- ESP32-CAM Streaming
- Auto / Manual Mode Switching

---

# 🛠 Setup Instructions

## Step 1 — Install Arduino IDE

Download and install Arduino IDE.

---

## Step 2 — Install Required Board Packages

Install:
- ESP8266 Board Package
- ESP32 Board Package

---

## Step 3 — Install Required Libraries

Install:

```text
ESP8266WiFi
ESP8266WebServer
Servo
WiFi
esp_camera
```

---

## Step 4 — Connect Hardware Components

Connect:
- ESP8266
- ESP32-CAM
- Ultrasonic Sensor
- Servo Motor
- L298N Motor Driver
- DC Motors
- Battery Pack

---

## Step 5 — Upload ESP32-CAM Code

Upload:
```text
esp32_cam_stream.ino
```

Copy the generated IP address from Serial Monitor.

---

## Step 6 — Update ESP8266 Controller Code

Update:

```cpp
#define CAM_IP "http://YOUR_ESP32_CAM_IP/"
```

Also update WiFi credentials:

```cpp
const char* ssid = "YOUR_WIFI_NAME";
const char* password = "YOUR_WIFI_PASSWORD";
```

---

## Step 7 — Upload ESP8266 Code

Upload:

```text
esp8266_robot_controller.ino
```

---

## Step 8 — Open Web Dashboard

Open ESP8266 IP address in browser.

The dashboard provides:
- Robot control
- Speed adjustment
- Mode switching
- Distance monitoring
- Live camera feed

---

# 📷 Real-Time Monitoring Dashboard

The responsive web dashboard includes:

- Live ESP32-CAM stream
- Manual direction controls
- Auto mode switching
- Real-time sensor data
- PWM speed adjustment
- Wireless operation

---

# 📊 Applications

- Smart Surveillance Robots
- Industrial Monitoring
- Autonomous Navigation
- Security Systems
- IoT Robotics
- Smart Inspection Systems
- Warehouse Automation
- Remote Monitoring Robots

---

# ✅ Advantages

- Wireless robot control
- Autonomous navigation
- Real-time monitoring
- Embedded + IoT integration
- Low-cost implementation
- Portable design
- Responsive dashboard UI
- Real-time communication
- Live video streaming

---

# ⚠ Limitations

- WiFi range limitations
- Battery backup depends on load
- ESP32-CAM video quality depends on network speed
- Limited processing power for advanced AI

---

# 🔮 Future Improvements

Future enhancements can include:

- AI object detection
- Face recognition
- Voice control
- Mobile app integration
- Cloud dashboard
- GPS tracking
- SLAM mapping
- Computer vision
- Machine learning navigation
- Autonomous path planning

---

# 🧪 Technologies Used

## Hardware

- ESP8266 NodeMCU
- ESP32-CAM
- HC-SR04 Ultrasonic Sensor
- Servo Motor
- L298N Motor Driver
- DC Motors

---

## Software

- Arduino IDE
- Embedded C++
- HTML/CSS/JavaScript
- WiFi Communication
- HTTP Protocol
- PWM Motor Control

---

# 📈 Project Outcomes

The developed system successfully:

- Detects obstacles accurately
- Performs autonomous navigation
- Streams live video wirelessly
- Enables web-based robot control
- Demonstrates IoT and embedded integration
- Provides real-time monitoring capabilities

---

# 👨‍💻 Author

## Gokula Krishnan R

Electronics and Communication Engineer  
IoT & Embedded Developer  
Automation Enthusiast

📧 Email: gokulakrishnanramasamy65@gmail.com

🌐 GitHub: https://github.com/GOKULAKRISHNAN2805

---

# 📄 License

This project is licensed under the MIT License.

---

# ⭐ Support

If you found this project useful, give it a ⭐ on GitHub.

---

# 🙌 Acknowledgement

This project was developed as part of an IoT and Embedded Systems learning initiative focused on robotics, automation, wireless communication, and real-time monitoring systems.
