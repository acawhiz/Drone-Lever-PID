# Drone Lever PID

🚀 A hybrid PID-controlled lever system using DE10-Nano FPGA, BDCM, and real-time C# visualization.

This project controls a physical **lever** that is lifted by a **brushless DC motor (BDCM)** and **propeller**, with closed-loop feedback using a **PID controller**. The project is implemented on an **Intel DE10-Nano FPGA board**, and includes a C# interface for real-time PID parameter display and tuning.

---

## ⚙️ Features

- 🧠 **PID Control**  
  - Switchable between **FPGA-implemented PID** and **C#-based PID**
  - Tunable parameters: P, I, D gains, update rate, output limits

- 🛰 **Sensor Integration**  
  - Uses the **ADXL345** accelerometer to detect lever angle/tilt
  - Samples vibration/noise data for filtering and control

- 🌀 **Filtering**  
  - Implements an **exponential moving average filter** to reduce motor vibration impact on sensor readings

- 💻 **C# Interface**  
  - Live plotting and parameter updates
  - Option to simulate PID in software or defer control to the FPGA

---

## 📦 Components

| Component         | Description                        |
|------------------|------------------------------------|
| DE10-Nano         | FPGA platform with ARM Cortex-A9   |
| BDCM + Propeller | Provides lift for the lever         |
| ADXL345          | 3-axis accelerometer (I2C/SPI)      |
| C# GUI           | Real-time PID display & control     |

---

## 🔍 Focus Areas

- ✅ FPGA Design (Verilog/SystemVerilog)
- ✅ Embedded Systems
- ✅ Real-Time PID Control
- ✅ Sensor Filtering (Exponential Filter)
- ✅ C# GUI and Serial Communication
- ✅ Hardware/Software Co-Design
- ✅ Signal Processing and Vibration Management

---

## 🚧 Development Status

- ✅ Working prototype on hardware
- ✅ C# interface with PID tuning and monitoring
- ✅ PID selectable via software toggle
- 🛠 Improving filtering and response time
- 🧪 Testing with different payloads and vibration patterns

---

## 📸 Demo & Images

> Coming Soon — images and video of the lever in action will be added here.

---

## 📅 Roadmap

- [ ] Add support for saving PID presets
- [ ] Integrate FFT-based vibration analysis
- [ ] Improve C# visualization performance
- [ ] Upload hardware schematics and filter design

---

> ⭐ Star this project to follow development and get notified of updates!
