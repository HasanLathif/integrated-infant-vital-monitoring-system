# Integrated Non-Adhesive Pediatric Vital Sign Monitoring System

**Tags:** `[Ongoing]`, `Thesis`, `IoT`, `Hardware`, `Sensor Fusion`, `ESP32`, `Wearable`

> **Status: [Ongoing]** This is my active undergraduate thesis focusing on the development of a non-invasive, split-node wearable system for pediatric monitoring.

---

<img width="426" height="1041" alt="Image" src="https://github.com/user-attachments/assets/c98146cd-6000-4b97-b21a-b9ffca814d44" />

## 1. The Problem

Continuous monitoring of pediatric vital signs (Respiratory Rate and SpO2) is critical for early detection of emergencies, particularly for pediatrics in the interstage phase. However, traditional adhesive electrodes can damage fragile pediatric skin, and wired connections limit mobility and comfort. Current solutions often lack effective motion artifact suppression, leading to false alarms.

## 2. My Solution

This study proposes a **Smart Wearable System** utilizing a **Split-Node design** to optimize sensor data recording and transmission without adhesive contact.

The system consists of two main components:
1.  **Master Node (Chest Strap):** Uses dry electrodes to record diaphragm electrical activity (dEMG) for Respiratory Rate (RR) monitoring. It integrates an **IMU (Accelerometer + Gyroscope)** to detect motion and filter artifacts.
2.  **Slave Node (Smart Socks):** Uses a **MAX30102** photometric biosensor to measure SpO2 at the foot/ankle, a location with stable perfusion.

The nodes communicate via **ESP-NOW** for low-latency data synchronization and transmit processed data via **Bluetooth Low Energy (BLE)** to a central monitor.

## 3. My Role & Key Contributions

I am the **Sole Researcher and Developer** for this project.

* **System Design:** Conceptualized the split-node architecture to separate respiration and pulse monitoring for better ergonomics.
* **Hardware Engineering:** Integrating the ESP32 microcontroller with dEMG dry electrodes, MAX30102 sensors, and IMU units.
* **Signal Processing:** Developing a **Sensor Fusion** algorithm (DSP) that uses IMU data as a reference signal to actively suppress motion artifacts from the vital sign readings.
* **Wireless Protocol Implementation:** Implementing ESP-NOW for node-to-node communication and BLE for power-efficient data transmission.

## 4. Technology Stack

* **Hardware:** `ESP32` (Master & Slave Nodes), `MAX30102` (SpO2), `Dry Electrodes` (dEMG), `IMU` (MPU6050/similar)
* **Communication Protocols:** `ESP-NOW`, `Bluetooth Low Energy (BLE)`
* **Signal Processing:** `Digital Signal Processing (DSP)`, `Sensor Fusion`, `Motion Artifact Suppression`
* **Programming:** `C/C++` (Arduino/PlatformIO), `Python` (for data analysis/prototyping)

## 5. Proof of Progress

* **In Progress** 

## 6. Project Status

**Status: [Ongoing]**
*This project is currently in the active development and prototyping phase.*
