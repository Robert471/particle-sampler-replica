# 🌱 Humidity & Smoke Sensor Monitoring - ElectroPerú

This project was developed for **ElectroPerú** and consists of a distributed monitoring system using **ESP32 boards** to measure **humidity and smoke levels**.  
A total of **65 devices** were installed across the facility, transmitting data via **MQTT** to a **Raspberry Pi** server running Python for real-time visualization.

---

## 📁 Project Structure

The repository is organized as follows:

* **`backend/`**: Python scripts for MQTT broker, data reception, and visualization.
* **`firmware/`**: ESP32 embedded code for sensor acquisition and MQTT communication.
* **`docs/`**: Technical documentation, schematics, and deployment notes.
* **`image/`**: Photographic records of PCB, programming, testing, and installation.

---

## 🛠️ Hardware and Connections

### PCB Connection
Printed circuit board (PCB) designed for interfacing the humidity and smoke sensors with the ESP32 module.

![PCB Connection](image/pcb_connection.jpg)

---

## 🚀 Development and Deployment

### Programming Phase
Firmware development and debugging on ESP32 boards.  
![Programming](image/programming.png)

### Testing Phase
Validation of MQTT communication and sensor accuracy before deployment.  
![Testing](image/testing.jpg)

### Installation
On-site installation and supervision of 65 devices across ElectroPerú facilities.  
![Engineer](image/enginner.jpg)

---

## 📊 Monitored Parameters

The system measures and transmits the following variables:

- **Humidity levels**  
- **Smoke detection**  
- **Device health and connectivity status**

---

## 📋 Requirements and Setup

### Firmware (ESP32)
1. Open the `firmware/` folder in PlatformIO or Arduino IDE.
2. Configure Wi-Fi credentials and MQTT broker address.
3. Compile and flash the ESP32 boards.

### Backend (Raspberry Pi)
1. Navigate to the `backend/` folder.
2. Install dependencies:
   ```bash
   pip install paho-mqtt matplotlib flask
