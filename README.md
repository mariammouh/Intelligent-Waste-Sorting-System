# ♻️ SortBin – Intelligent Waste Sorting System

## Overview

**SortBin** is an intelligent waste-sorting system developed as part of the **Enactus International Competition 2026**. The project combines **Artificial Intelligence**, **Computer Vision**, **IoT**, and **Embedded Systems** to automate waste classification and improve recycling efficiency.

The system identifies waste items using a camera and a Deep Learning model, then automatically directs each item to the appropriate compartment through a motorized sorting mechanism.

---

## Problem Statement

Manual waste sorting is:

* Time-consuming
* Costly
* Error-prone
* Potentially hazardous for workers

SortBin aims to automate this process using AI-driven classification and embedded hardware, reducing human intervention while increasing sorting accuracy.

---

## Features

* 📷 Real-time image acquisition using a Pi Camera
* 🧠 Waste classification using a Deep Learning model (ResNet)
* 🤖 Automated sorting mechanism
* 🔄 Real-time decision making on edge devices
* ♻️ Support for multiple waste categories
* 📡 IoT and embedded system integration

---

## System Architecture

```text
Waste Item
     │
     ▼
Pi Camera V2
     │
     ▼
ResNet Classification Model
(Raspberry Pi)
     │
     ▼
Category Prediction
     │
     ▼
Arduino Mega
     │
     ▼
Stepper Motor Control
     │
     ▼
Waste Directed to Correct Bin
```

---

## Hardware Components

| Component                | Role                      |
| ------------------------ | ------------------------- |
| Raspberry Pi             | Main processing unit      |
| Pi Camera V2             | Image acquisition         |
| Arduino Mega             | Motor control             |
| 28BYJ-48 Stepper Motor   | Rotating sorting platform |
| ULN2003 Driver           | Stepper motor driver      |
| Multi-compartment Bin    | Waste collection          |
| Touch Display (Optional) | Local monitoring          |

---

## Software Stack

### Artificial Intelligence

* Python
* TensorFlow / TensorFlow Lite
* ResNet Architecture
* NumPy

### Computer Vision

* OpenCV

### Embedded Systems

* Raspberry Pi OS
* Arduino IDE

### Remote Access

* SSH
* VNC Viewer

---

## Waste Categories

Current prototype supports:

* Plastic
* Cardboard / Paper
* Others

Future versions may include:

* Glass
* Metal
* Organic Waste
* Electronic Waste

---

## AI Model

The waste classification module is based on a **ResNet (Residual Neural Network)** architecture trained on labeled waste images.

### Model Workflow

1. Capture image using Pi Camera V2
2. Preprocess image
3. Run inference on Raspberry Pi
4. Predict waste category
5. Send command to Arduino
6. Rotate sorting platform toward the correct compartment

---

## Project Objectives

* Improve recycling efficiency
* Reduce manual sorting errors
* Protect workers from hazardous waste exposure
* Promote sustainable waste management
* Demonstrate practical AI and IoT integration

---

## Results

✅ Functional prototype developed

✅ Real-time waste classification

✅ Automated waste redirection

✅ Successful integration of AI, Computer Vision, IoT, and Embedded Systems

---

## Team

Developed during the **Enactus 2026 Competition** by:

* Basma El Kadri
* Ghita Benlahcen
* Mariam Mouh
* Najat Aderdour
* Wijdane Abouzaid

---

## Future Improvements

* Expand supported waste categories
* Improve model accuracy with larger datasets
* Add cloud-based analytics dashboard
* Implement fill-level monitoring sensors
* Deploy OTA updates for remote maintenance

---

## License

This project was developed for educational, research, and innovation purposes within the Enactus program.
