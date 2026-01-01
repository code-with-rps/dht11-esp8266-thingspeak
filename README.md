# IoT-Based Temperature & Humidity Monitoring System 🌡️📊

An **end-to-end IoT-based temperature and humidity monitoring system** using a **DHT11 sensor** and **ESP8266 (NodeMCU)**, with real-time data visualization on the **ThingSpeak cloud platform**.

---

## 🚀 Features
- Real-time temperature and humidity monitoring
- Wi-Fi enabled data transmission (2.4 GHz)
- Cloud integration using ThingSpeak
- Live graphical data visualization
- Serial monitoring for debugging and status updates

---

## 🧰 Hardware Used
- ESP8266 NodeMCU
- DHT11 Temperature & Humidity Sensor
- Jumper wires
- USB cable

---

## 💻 Software & Tools
- Arduino IDE
- ESP8266WiFi Library
- Adafruit DHT Sensor Library
- Adafruit Unified Sensor Library
- ThingSpeak Cloud Platform

---

## 🔌 Circuit Connections

| DHT11 Pin | ESP8266 NodeMCU |
|----------|----------------|
| VCC | 3.3V |
| DATA | D4 (GPIO2) |
| GND | GND |

---

## ☁️ ThingSpeak Configuration
- **Field 1** → Temperature (°C)
- **Field 2** → Humidity (%)
- **Minimum update interval** → 15 seconds

---

## 📊 Output
Live temperature and humidity data visualized on the ThingSpeak dashboard.

---


## 📁 Project Structure
```text
dht11-esp8266-thingspeak/
├── code/
│   └── dht11_esp8266_thingspeak.ino
├── images/
│   └── thingspeak_output.png
├── README.md
└── LICENSE


---

## 🔧 Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/code-with-rps/dht11-esp8266-thingspeak.git
Open the Arduino file:

bash
Copy code
code/dht11_esp8266_thingspeak.ino
Install the required libraries from Arduino Library Manager:

ESP8266WiFi

Adafruit DHT Sensor Library

Adafruit Unified Sensor

Update the following placeholders in the code:

cpp
Copy code
const char* ssid = "YOUR_WIFI_NAME";
const char* password = "YOUR_WIFI_PASSWORD";
String apiKey = "YOUR_THINGSPEAK_API_KEY";
Select the board and port:

Board: NodeMCU 1.0 (ESP-12E Module)

Port: COMxx

Upload the code to the ESP8266.

▶️ How It Works
The DHT11 sensor measures temperature and humidity.

ESP8266 connects to a 2.4 GHz Wi-Fi network.

Sensor data is sent to ThingSpeak using HTTP requests.

Data is displayed as live graphs on the ThingSpeak dashboard.

🧠 Learning Outcomes
Sensor interfacing with ESP8266

Wi-Fi networking and HTTP communication

Cloud-based IoT data visualization

Serial communication and debugging

Understanding end-to-end IoT system architecture

🔐 Security Note
Wi-Fi credentials and ThingSpeak API keys are not included in this repository.
Users must add their own credentials before uploading the code.

📌 Future Improvements
Email or alert notifications on threshold breach

OLED display integration

Relay-based automation (fan/light control)

Data analytics and CSV export from ThingSpeak

👤 Author
Rudrapratap Singh

📜 License
This project is licensed under the MIT License.
