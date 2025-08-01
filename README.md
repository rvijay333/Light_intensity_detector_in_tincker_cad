# 💡 Light Intensity Detector (Tinkercad + Arduino)

An interactive project to detect ambient light using a photoresistor (LDR) and an Arduino Uno. The brighter the environment, the brighter the LED—perfect for learning about analog sensors and microcontroller basics!

---

![Project Demo](images/demo.gif) 

---

## 🚀 Features

- Real-time detection of light intensity with photoresistor
- Smooth LED brightness control using analog output
- Ready to simulate in [Tinkercad](https://www.tinkercad.com/)
- Beginner-friendly code, well-commented

## 🗂️ Table of Contents

- [Project Overview](#-project-overview)
- [Circuit Diagram](#-circuit-diagram)
- [How It Works](#-how-it-works)
- [Getting Started](#-getting-started)
    - [Requirements](#requirements)
    - [Running in Tinkercad](#running-in-tinkercad)
    - [Running on Hardware](#running-on-hardware)
- [Example Code](#-example-code)
- [Demo](#-demo)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📖 Project Overview

This project uses an LDR (photoresistor) to sense changes in ambient light. The detected value controls the brightness of an LED connected to an Arduino Uno. You’ll learn how to use analogRead/analogWrite and understand the basics of analog sensors.

---

## 🖼️ Circuit Diagram

![Circuit Diagram](images/circuit.png)  <!-- Replace with your own schematic image -->

**Components:**
- Arduino Uno
- LDR (photoresistor)
- LED
- 220Ω resistor (for LED)
- 10kΩ resistor (for LDR voltage divider)
- Breadboard & wires

---

## ⚙️ How It Works

1. The LDR and 10kΩ resistor form a voltage divider; their junction connects to Arduino's A0 analog pin.
2. The Arduino reads light intensity on A0 (0–1023).
3. The value is scaled and sent to an LED via `analogWrite()` for smooth brightness adjustment.

---

## 🛠️ Getting Started

### Requirements

- [Tinkercad account](https://www.tinkercad.com/)
- Arduino Uno (real or simulated)
- The listed components above

### Running in Tinkercad

1. Go to the [Tinkercad Project Link](https://www.tinkercad.com/...) <!-- Add your project link here -->
2. Start the simulation and interact with the photoresistor.
3. Watch the LED brightness change as light intensity varies.

### Running on Hardware

1. Build the circuit as shown.
2. Upload the code from this repo (`/code/LightIntensityDetector.ino`) to your Arduino using Arduino IDE.
3. Test the circuit by changing the light falling on the LDR.

---

## 💻 Example Code

> **File:** `LightIntensityDetector.ino`

