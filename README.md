# 🌡️ Smart Classroom Temperature Monitoring System

## 📌 Project Overview

This project implements a **Smart Classroom Temperature Monitoring System** using IoT technology. The system continuously monitors the classroom temperature and automatically sends a **WhatsApp alert** to the concerned authority when the temperature exceeds the predefined threshold of **23°C**.

The solution is designed to be **cost-effective, automated, and easy to deploy**, making it suitable for educational environments.

The project is implemented using **MicroPython** and tested using the **Wokwi simulation environment**, eliminating the need for physical hardware during development.

---

## 🎯 Problem Statement

In many classrooms, air conditioning systems may operate irregularly, causing discomfort to students. There is often no automated system to continuously monitor classroom temperature and notify the responsible authority when the temperature becomes too high.

This project addresses the issue by providing an **automatic temperature monitoring and alert system** using IoT technology and WhatsApp notifications.

---

## ⚙️ Features

* 🌡️ Continuous classroom temperature monitoring
* 🚨 Threshold-based alert system at **23°C**
* 📱 Automatic WhatsApp notifications using an API
* 📡 WiFi-based communication
* ⏱️ **15-minute cooldown** to prevent repeated alerts
* 💻 Simulation-based implementation using Wokwi
* 🔧 No physical hardware required during development

---

## 🧰 Technologies Used

| Technology       | Purpose                                     |
| ---------------- | ------------------------------------------- |
| **MicroPython**  | Programming the ESP32                       |
| **ESP32**        | IoT controller (simulated)                  |
| **DHT22**        | Temperature and humidity sensor (simulated) |
| **WhatsApp API** | Sending temperature alerts                  |
| **Wokwi**        | IoT simulation and testing                  |
| **GitHub**       | Source code and project management          |

---

## 🧩 How the System Works

The system follows a simple continuous monitoring process:

1. The **ESP32** connects to a WiFi network.
2. The **DHT22 sensor** reads the classroom temperature and humidity.
3. The temperature value is compared with the predefined threshold of **23°C**.
4. If the temperature exceeds **23°C**, the system sends a **WhatsApp alert** to the registered phone number through an API.
5. After sending the alert, the system waits for **15 minutes** before sending another alert.
6. The temperature monitoring process continues continuously.

### 🔄 System Flow

```text
        ┌─────────────────┐
        │     ESP32       │
        │  Connect to WiFi│
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │  DHT22 Sensor   │
        │ Read Temperature │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │ Temperature >   │
        │      23°C ?      │
        └───────┬─────────┘
            Yes │       No
                │        │
                ▼        │
       ┌────────────────┐ │
       │ Send WhatsApp  │ │
       │     Alert      │ │
       └───────┬────────┘ │
               │          │
               ▼          │
       ┌────────────────┐ │
       │ 15-Minute      │ │
       │ Cooldown       │ │
       └───────┬────────┘ │
               │          │
               └────┬─────┘
                    │
                    ▼
             Continue Monitoring
```

---

## 🧪 Simulation

The project is developed and tested using **Wokwi**, an online electronics simulator.

The simulation allows the ESP32 and DHT22 sensor to be tested without requiring physical components.

### Simulation Components

* ESP32
* DHT22 Temperature & Humidity Sensor
* WiFi connection
* MicroPython program
* WhatsApp API integration

---

## 📱 WhatsApp Alert

When the classroom temperature rises above the predefined threshold, the system automatically sends a WhatsApp notification.

### Example Alert

```text
⚠️ Classroom Temperature Alert!

Temperature has exceeded the safe threshold of 23°C.

Please check the classroom cooling system.
```

A **15-minute cooldown mechanism** is implemented to prevent the system from sending repeated notifications continuously.

---

## 🚀 Future Scope

The project can be further improved by adding:

* 📊 Real-time temperature monitoring dashboard
* 📈 Temperature history and data logging
* 🌡️ Multiple classroom monitoring
* ❄️ Automatic AC/fan control
* ☁️ Cloud-based data storage
* 📧 Email and SMS notifications
* 📱 Mobile application integration
* 🔔 Multiple notification channels

---

## 👩‍💻 Authors

### NANDANA SAJEEV

GitHub: [@nandanasvsajeev-spec](https://github.com/nandanasvsajeev-spec)

### MIYANDA MARY JANUSH

GitHub: [@miyandamary](https://github.com/miyandamary)

### S.M GOPIKA

GitHub: [@smgopika2-design](https://github.com/smgopika2-design)

### ANNA GOMEZ.S

GitHub: [@kmary2575-beep](https://github.com/kmary2575-beep)

---

## 📄 Project Information

**Project Type:** IoT / Embedded Systems
**Programming Language:** MicroPython
**Platform:** ESP32
**Simulation:** Wokwi
**Sensor:** DHT22
**Communication:** WiFi + WhatsApp API

---

## ⭐ Acknowledgement

This project was developed as a collaborative academic project to demonstrate the use of **IoT, MicroPython, sensors, WiFi communication, and automated notifications** in a smart classroom environment.
