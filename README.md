# ERGOS
### Embodied Reinforcement Gait Operating System

---

## 🧠 Overview
The ERGOS (Embodied Reinforcement Gait Operating System) project is a low-cost, open-source platform designed for advanced dynamic humanoid robotics research. It serves as a ROS2-based control environment that integrates high-efficiency servo hardware with Reinforcement Learning (RL) techniques. The primary goal of ERGOS is to develop and optimize highly dynamic, stable gait patterns for bipedal systems, demonstrating sophisticated movement capabilities on an economical, self-contained hardware platform. Here is a photo of ERGOS's current design:

---

<div style="text-align: center;"><img src="https://github.com/Bryanh002/AI-Robot/blob/main/Documentation/images/Robot_Image_1.PNG" /></div>

---

## ⚙️ Features (Planned and In Progress)
- **Dynamic Walking with Reinforcement Learning**
  - RL-based control for adaptive locomotion
  - Simulation-first training approach before deployment on hardware
- **Smart Serial Servo Control**
  - Dual-servo setup using Feetech STS3235 and STS3250 actuators  
  - Pulleys with 2:1 gear ratios at select joints for torque optimization
- **Custom Electronics**
  - PCB with ESP32-S3 microcontroller for servo communication and power management
  - Jetson Orin Nano as the main compute module running the AI systems
- **Environmental Awareness (Future)**
  - Integration of a vision system for obstacle perception and terrain recognition
- **Speech and Interaction (Future)**
  - Onboard LLM to process voice commands and control robot behavior through natural language

---

## 🧩 System Architecture (In Development)
| Component | Function |
|------------|-----------|
| **Jetson Orin Nano** | Runs reinforcement learning models and manages high-level control |
| **ESP32-S3 PCB** | Interfaces with servos, manages serial bus communication and power |
| **Smart Servos (Feetech STS3235 & STS3250)** | Actuators for joints, supporting position feedback and serial daisy-chaining |
| **Pulleys (2:1 ratio)** | Increases effective torque at key leg joints |
| **Simulation Environment** | Used for RL model training prior to real-world deployment |

> CAD design (SolidWorks) and PCB layout (Altium Designer) are currently in active development.

---

## 🧪 Development Phases
1. **Phase 1 — Hardware Integration**  
   Finalize CAD design and PCB for servo control and power distribution.

2. **Phase 2 — Reinforcement Learning Simulation**  
   Develop simulation environment for dynamic walking using RL.  
   *(Likely frameworks: PyTorch, custom physics simulation, or Isaac Gym)*

3. **Phase 3 — Real-World Testing**  
   Transfer trained model to the Jetson Orin Nano for live walking experiments.

4. **Phase 4 — Vision and Speech Integration**  
   Add camera input for object detection and LLM for high-level control.

---

## 🧠 Technical Summary
- **Programming Language:** Python (planned)
- **Frameworks:** TBD (PyTorch or TensorFlow for RL; ROS2 possible integration)
- **Hardware:** Jetson Orin Nano, ESP32-S3, Feetech STS3235/STS3250 smart servos
- **Design Tools:** SolidWorks (mechanical), Altium Designer (PCB)

---

## 🚀 Getting Started
*(To be updated as the project matures)*

**Planned sections:**
1. Installation requirements (JetPack SDK, Python environment, dependencies)
2. Simulation setup (RL environment)
3. Model training and deployment instructions
4. Hardware configuration and servo connection mapping

---

## 📈 Future Work
- Implement visual SLAM and object detection pipeline  
- Add voice recognition and LLM-based decision-making  
- Optimize energy consumption and walking stability  
- Publish simulation and training environments for community use  

---

## 📜 License
This project is open source and released under the **MIT License**.  
See the [LICENSE](LICENSE) file for more information.

---

## 👤 Author
**Bryan Heddle**  
Mechatronics & AI Systems Engineering Student — *Western University*  

---

## 💡 Acknowledgments
Special thanks to the open-source robotics community for tools, documentation, and inspiration contributing to this project’s foundation.

---


