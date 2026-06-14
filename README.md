# 📡 433MHz ASK RF Receiver Module

![Status](https://img.shields.io/badge/status-open--hardware-blue)
![Frequency](https://img.shields.io/badge/frequency-433MHz-green)
![Modulation](https://img.shields.io/badge/modulation-ASK-orange)
![Hardware](https://img.shields.io/badge/hardware-PCB-purple)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## 🚀 Overview

**433MHz ASK RF Receiver Module** is a compact open-hardware wireless receiver PCB designed for receiving **433MHz Amplitude Shift Keying signals** in embedded systems, IoT projects, RF learning setups, remote-control decoding experiments, and custom wireless communication applications.

The design includes an antenna input stage, RF tuning section, transistor-based RF front-end, diode-based signal detection, filtering network, and LM358-based analog signal conditioning to provide a usable output signal for microcontrollers, decoder circuits, oscilloscopes, or logic analyzers.

---

## ✨ Key Features

- 📡 433MHz RF signal reception
- 📶 ASK modulation support
- 🧲 Antenna input matching and RF tuning
- ⚡ Diode-based signal detection stage
- 🔺 LM358-based signal amplification and conditioning
- 🧹 RC filtering for noise reduction
- 🔌 Simple VCC, GND, and DATA output interface
- 🧩 Compact custom PCB layout
- 🛠️ Open-hardware design
- 🧪 Suitable for RF testing, learning, and prototyping

---

## 🧠 Technical Description

This module is designed to receive wireless signals in the **433MHz ISM frequency band** using **ASK modulation**.

The incoming RF signal is captured by the antenna and passed through a tuned RF input network. The signal is then processed through the RF front-end stage, detected using diode-based rectification, filtered using resistor-capacitor networks, and conditioned using LM358 operational amplifier stages.

The final output can be connected to a microcontroller GPIO pin, oscilloscope, logic analyzer, decoder circuit, or embedded system for further processing.

---

## 🧱 System Block Diagram

```text
Antenna
   ↓
RF Input Matching / Tuning
   ↓
RF Front-End Stage
   ↓
ASK Signal Detection
   ↓
Noise Filtering
   ↓
LM358 Signal Conditioning
   ↓
DATA Output
   ↓
Microcontroller / Decoder / Logic Analyzer
```

---

## 🔌 Pinout

| Pin | Name | Description |
|---|---|---|
| 1 | VCC | Power input |
| 2 | DATA | Receiver output signal |
| 3 | GND | Ground |

---

## 🧩 Main Components

| Component | Function |
|---|---|
| Antenna | Captures 433MHz RF signals |
| Inductors | RF tuning and filtering |
| Capacitors | Coupling, filtering, and decoupling |
| Diodes | Signal detection |
| Transistor | RF front-end signal handling |
| LM358 | Amplification and analog signal conditioning |
| Resistors | Biasing, gain setting, and filtering |
| Header Pins | External power and signal interface |

---

## ⚙️ Hardware Design Sections

### 1. Antenna Input Section

The antenna input receives the 433MHz RF signal.  
A properly tuned antenna improves sensitivity, stability, and range.

### 2. RF Tuning Section

The LC components are used to tune and filter the received RF signal.  
This section helps improve selectivity around the 433MHz frequency range.

### 3. RF Front-End Section

The transistor stage helps process the weak RF input signal before detection.

### 4. ASK Signal Detection Section

The diode stage detects amplitude changes in the received RF signal and converts them into a lower-frequency signal component.

### 5. Filtering Section

RC filters smooth the detected signal and reduce unwanted RF noise.

### 6. LM358 Signal Conditioning Section

The LM358 operational amplifier stages amplify and condition the detected signal so it can be used by external digital or analog circuits.

### 7. Output Section

The output pin provides the recovered receiver signal for further processing.

---

## 🖼️ Project Preview

### Schematic
<img width="1203" height="570" alt="image" src="https://github.com/user-attachments/assets/dba9f76a-4c4d-456e-9909-b6e5f7a4cc1a" />

![Schematic](images/schematic.png)

### PCB Layer
<img width="1126" height="740" alt="image" src="https://github.com/user-attachments/assets/d7e1af72-39ec-4dfe-a8f1-dbd3286d03a5" />

![PCB Layer](images/pcb-top.png)



### 3D PCB Render

<img width="1042" height="748" alt="image" src="https://github.com/user-attachments/assets/051b80e4-f895-4ddf-b932-8b2c0d344b57" />
<img width="730" height="724" alt="image" src="https://github.com/user-attachments/assets/e5f72484-3110-4a07-93c1-7b5899c61e6a" />
<img width="775" height="706" alt="image" src="https://github.com/user-attachments/assets/5c67a9b5-4720-477f-bd98-79b4226ea370" />
<img width="1171" height="754" alt="image" src="https://github.com/user-attachments/assets/f80d6f3b-259b-4c64-813d-25b2ea75359e" />
<img width="994" height="693" alt="image" src="https://github.com/user-attachments/assets/e442adae-970d-46cf-986b-0c2f329196f2" />


![3D Render](images/3d-render.png)

---

## 📡 Antenna Notes

For better range and sensitivity, use a properly sized antenna.

A common quarter-wave antenna length for 433MHz is approximately:

```text
17.3 cm
```

A simple wire antenna can be used for testing, but performance depends on placement, wire quality, ground reference, and surrounding interference.

---

## ⚠️ Important Notes

This module is intended for:

- Educational use
- RF learning
- Prototype development
- Experimental wireless communication
- Embedded hardware testing

---

## 👨‍💻 Author

Designed by **Fernando S.M.H.G**

Open-hardware RF receiver project for embedded systems, electronics learning, and wireless communication experiments.

---

## 📜 License

This project is released under the **MIT License**.

You are free to use, modify, improve, and share this project with proper attribution.

---

## ⭐ Support

If this project helps you, consider giving the repository a star.

```text
Made for RF learning, embedded systems, and open-hardware development.
```
