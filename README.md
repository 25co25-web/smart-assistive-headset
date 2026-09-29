# 🎧 Smart Assistive Headset

An ESP32-based smart assistive headset that uses ultrasonic sensors to detect nearby obstacles and provides real-time distance feedback through Bluetooth audio.

## 🚀 Overview

The Smart Assistive Headset is a low-cost prototype designed to help users become aware of nearby obstacles without constantly looking around.

The headset uses ultrasonic sensors to measure the distance of objects. The ESP32 processes the sensor readings and communicates the information to a mobile device over Bluetooth. The mobile application can then provide spoken feedback through a Bluetooth headset or speaker.

## ✨ Features

* 📏 Real-time obstacle distance detection
* 🎧 Audio-based distance feedback
* 📡 Bluetooth communication using ESP32
* 📱 Mobile-phone integration
* ⚡ Fast response to nearby obstacles
* 💰 Low-cost hardware
* 🔧 Easy to modify and extend

## 🛠️ Hardware

* ESP32 / NodeMCU-32S
* HC-SR04 Ultrasonic Sensors
* 1kΩ resistor
* 2kΩ resistor
* Bluetooth-enabled smartphone
* Bluetooth headset / speaker
* Jumper wires
* Breadboard

## 🔌 Sensor Setup

The prototype can use multiple ultrasonic sensors for different directions:

| Direction | Trigger |    Echo |
| --------- | ------: | ------: |
| Left      |  GPIO 5 | GPIO 18 |
| Center    | GPIO 16 |  GPIO 4 |
| Right     | GPIO 17 | GPIO 19 |

> **Note:** The HC-SR04 Echo signal should be reduced to a safe voltage level before connecting it to an ESP32 GPIO. A resistor voltage divider is used for this purpose.

## 🔄 How It Works

```text
Ultrasonic Sensors
        ↓
      ESP32
        ↓
Distance Processing
        ↓
    Bluetooth
        ↓
   Mobile Phone
        ↓
   Audio Feedback
        ↓
 Bluetooth Headset
```

1. The ultrasonic sensors send sound pulses.
2. The sensors receive the reflected signal from nearby objects.
3. The ESP32 calculates the approximate distance.
4. The distance information is sent to the mobile device through Bluetooth.
5. The mobile application converts the information into spoken feedback.
6. The feedback is played through the headset.

## 📱 Software

The project can use:

* Arduino IDE
* ESP32 Arduino Core
* MIT App Inventor
* Bluetooth communication
* Android Text-to-Speech


## 🎯 Future Improvements

* Add vibration feedback
* Improve directional detection
* Add rechargeable battery support
* Make the headset more compact
* Improve outdoor detection
* Add configurable distance thresholds
* Develop a dedicated Android application

## ⚠️ Project Status

**Prototype / Educational Project**

This project is currently a prototype developed for learning, experimentation, and demonstrating embedded systems, Bluetooth communication, and assistive technology concepts.

## 👨‍💻 Contributors

- Jonathan De Sa — @jonathandesa
- Rahul — @rahul123

⭐ If you find this project useful, consider giving the repository a star!
