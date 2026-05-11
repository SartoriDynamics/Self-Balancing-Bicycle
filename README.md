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
- Low-cost physical structure.  
- Experimental platform for robotics and control.

---

## ⚙️ How It Works

1. The MPU-6050 measures the bicycle inclination and angular motion.  
2. The ESP32 processes sensor data and computes the control action.  
3. The servo motor adjusts the torque to stabilize the bicycle.  
4. Experimental data can be collected for analysis and controller validation.

---

## 📂 Repository Structure

- **Arduino IDE Configuration.txt** → ESP32 development board IDE configuration guide.
- **Component List.txt** → All project components.
- **SBB 3D printing files/** → 3D printable CAD models for physical parts.
- **Arduino codes/** → ESP32 firmware and experiment code:
  - **Balance/**: Main LQR balancing code (`LQR.ino`).
  - **Experiments/**: Test sketches for controller and hardware:
    - `LQR_experiment.ino`: Experimental LQR control and data collection.
    - `test_components.ino`: Individual component testing.
  - **Xbox/**: Joystick (Xbox) remote control (`xbox.ino`).
- **Python codes/** → Notebooks and scripts for analysis:
  - `Balance_LQR_Controller_Design.ipynb`: LQR controller design and simulation.
  - `Velocity_PI_Controller_Design.ipynb`: Velocity PI controller design.
  - `Save_Data_During.ipynb`: Real-time data acquisition.
  - `Save_Data_After.ipynb`: Post-experiment data processing.

---

## 📸 Images

<table>
  <tr>
    <td align="center" width="50%" border="1" cellpadding="12">
      <img src="/SBB images/bia.png" alt="Assembled self-balancing bicycle prototype" width="100%"/>
    </td>
    <td align="center" width="50%" border="1" cellpadding="12">
      <img src="/SBB images/esquematico.png" alt="ESP32 wiring and electronics diagram" width="100%"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <em>Assembled self-balancing bicycle prototype.</em>
    </td>
    <td align="center">
      <em>ESP32 wiring and electronics diagram.</em>
    </td>
  </tr>
</table>

---

## 🎥 Video

<table>
  <tr>
    <td align="center" style="border: 1px solid #d0d7de; padding: 12px;">
      <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube"/><br><br>
      <a href="https://www.youtube.com/watch?v=5PImU6t4usI" target="_blank">
        <img src="https://img.youtube.com/vi/5PImU6t4usI/maxresdefault.jpg"
             alt="Self-Balancing Bicycle demonstration video"
             width="700"/>
      </a>
      <br><br>
      <em>Click the thumbnail to watch the demonstration video.</em>
    </td>
  </tr>
</table>
