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

## 🛠️ Requirements and Setup

To run the simulation, you will need the following software and toolboxes:

### Software Prerequisites

* **MATLAB** (R2018b or newer is recommended)
* **Simulink**

### Required Toolboxes

* **Fuzzy Logic Toolbox** (Essential for the implementation of the Fuzzy Logic System)

### Repository Structure (Suggested)

| File Name | Description |
| :--- | :--- |
| `fuzzy_adaptive_dsc.slx` | The main Simulink model file containing the controller and robot dynamics. |
| `scara_parameters.m` | A MATLAB script to define the physical parameters of the SCARA robot. |
| `control_gains.m` | A MATLAB script to initialize controller gains, trajectory definition, and fuzzy system parameters. |
| `results/` | Directory for storing output plots and data (e.g., tracking error, joint velocities). |

---

## 🚀 Running the Simulation

Follow these steps to open and execute the Simulink model:

1.  **Clone the Repository:**
    ```bash
    git clone [Your Repository URL]
    ```
2.  **Open MATLAB:** Navigate to the cloned repository directory in the MATLAB command window.
3.  **Initialize Parameters:** Run the necessary initialization scripts (e.g., `control_gains.m`) to set up the workspace variables.
    ```matlab
    control_gains;
    ```
4.  **Open the Model:** Load the Simulink file.
    ```matlab
    open('fuzzy_adaptive_dsc.slx')
    ```
5.  **Run Simulation:** Set the desired simulation time and click the "Run" button in the Simulink environment.
6.  **Analyze Results:** View the performance plots on the scopes within the model, which typically show the desired vs. actual trajectory and the tracking error.

---

## 📈 Expected Outcomes

The model-free fuzzy adaptive DSC is expected to demonstrate superior performance characteristics compared to non-adaptive or model-based controllers:

* **High Tracking Accuracy:** Minimized steady-state tracking error.
* **Robustness:** Stable performance even in the presence of unknown robot parameters or external disturbances.
* **Boundedness:** All signals in the closed-loop system (control input, states, and adaptive parameters) remain bounded.

---

## 📧 Contact and Contribution

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page]([Your Repository URL]/issues) if you have any questions.
