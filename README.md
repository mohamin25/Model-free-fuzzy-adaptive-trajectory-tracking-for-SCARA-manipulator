# Model-Free Fuzzy Adaptive Trajectory Tracking Control using Dynamic Surface Control (DSC)

This repository contains the **Simulink** implementation of the robust control strategy proposed in the following research paper, applied to a SCARA-type manipulator.

## 📄 Paper Reference

The simulation is based on the following publication:

**Title:** A model-free fuzzy adaptive trajectory tracking control algorithm based on dynamic surface control
**Authors:** Tong, M., Lin, W., Huo, X., Jin, Z., & Miao, C.
**Journal:** *International Journal of Advanced Robotic Systems*, 17(1), 2020.
**DOI:** `10.1177/1729881419894417`

---

## ✨ Project Overview

The goal of this project is to implement and simulate an advanced, model-free control algorithm for highly accurate trajectory tracking of a robot manipulator.

### Key Features Implemented:

* **Model-Free Control:** The controller design avoids the need for an exact mathematical model of the robot dynamics, making it robust against uncertainties.
* **Fuzzy Adaptive Logic:** A **Fuzzy Logic System** is incorporated to approximate the unknown dynamics, with parameters adjusted online using a **Lyapunov self-adaptation law** to ensure tracking stability and performance.
* **Dynamic Surface Control (DSC):** The DSC technique is employed to simplify the backstepping design process by using first-order filters, effectively mitigating the "explosion of complexity" issue.
* **Application:** The control algorithm is validated on the complete dynamics of a **Selective Compliance Assembly Robot Arm (SCARA)** manipulator.

---



---

## 📧 Contact and Contribution

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page]([Your Repository URL]/issues) if you have any questions.
