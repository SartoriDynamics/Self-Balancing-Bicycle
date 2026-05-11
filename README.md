# Self-Balancing Bicycle

A low-cost self-balancing bicycle platform developed for control research and education at UFMG.

This project is released under the MIT License.  
Copyright (c) 2024 GTI - UFMG

---

## Hardware

- 1× ESP-WROOM-32 30-pin development board
- 2× Nidec 24H DC motors
- 2× Set Tire wheels (88516 + 88517)
- 1× 2GT-280 belt (6 mm width)
- 1× SG90 metal gear servo motor
- 1× Adjustable DC-DC voltage regulator (12 V to 5 V)
- 1× GY-521 MPU-6050 module
- 1× 12 V battery holder for 3×18650 lithium-ion batteries

---

## 🛠️ Features

- Real-time balance control using ESP32.  
- MPU-6050 inertial sensing for tilt estimation.  
- Steering actuation using a servo motor.  
- Low-cost mechanical structure for control experiments.  
- Experimental platform for robotics and control education.

---

## ⚙️ How It Works

1. The MPU-6050 measures the bicycle inclination and angular motion.  
2. The ESP32 processes sensor data and computes the control action.  
3. The servo motor adjusts the steering angle to stabilize the bicycle.  
4. The DC motors provide propulsion during balancing experiments.  
5. Experimental data can be collected for analysis and controller validation.

---

## 📂 Repository Structure

- **Arduino codes/** → ESP32 firmware and control algorithms.
- **Python codes/** → Data analysis and visualization scripts.
- **SBB images/** → Project images and schematics.
  - `bia.png` → Assembled self-balancing bicycle prototype.
  - `esquematico.png` → Wiring and electronics diagram.

---

## 📸 Images

<p align="center">
  <img src="/SBB images/bia.png" alt="Assembled self-balancing bicycle prototype" width="500"/><br>
  <sub>Assembled self-balancing bicycle prototype.</sub>
</p>

<p align="center">
  <img src="/SBB images/esquematico.png" alt="ESP32 wiring and electronics diagram" width="500"/><br>
  <sub>ESP32 wiring and electronics diagram.</sub>
</p>

---

## 🎥 Video

<p align="center">
  <a href="https://www.youtube.com/watch?v=5PImU6t4usI">
    <img src="https://img.youtube.com/vi/5PImU6t4usI/maxresdefault.jpg" 
         alt="Self-Balancing Bicycle demonstration video" 
         width="600"/>
  </a>
  <br>
  <sub>Click the image to watch the demonstration video.</sub>
</p>
