# Fuzzy-Logic-Control-of-a-Robotic-Manipulator

**Computational Intelligence Course Project**  

Design and implementation of a fuzzy inference–based controller for autonomous motion, target tracking, and obstacle avoidance of a robotic manipulator within the Webots simulator using Python.

---

## 📌 Project Overview

This project explores the application of **Fuzzy Logic Control (FLC)** for advanced robotic manipulation tasks.  

The manipulator is required to reach designated targets, adapt to dynamic environments, and avoid collisions. Unlike classical model-based approaches, control is achieved through **linguistic rule evaluation and fuzzy inference**, enabling flexible and robust decision-making under uncertainty.

The system is developed in **Python** and evaluated in the Webots simulator, which provides high-fidelity physics and realistic sensor feedback.

---

## 🎯 Objectives

- Develop fuzzy membership functions for perceptual variables.  
- Construct linguistic rule-based decision systems for control.  
- Translate fuzzy outputs into actionable joint commands.  
- Quantitatively evaluate tracking accuracy and obstacle avoidance performance.  
- Extend control to dynamic, constrained, and cluttered environments.  

---

## 🧠 Skills & Concepts Demonstrated

- Fuzzy inference system design  
- Membership function tuning  
- Rule base formulation  
- Defuzzification strategies  
- Sensor-driven autonomous control  
- Robotic kinematics and motion planning  
- Simulation-based experimental validation  

---

## 📥 Inputs & Outputs

### Inputs from simulated sensors
- Joint angles  
- Joint velocities  
- Distance and relative orientation to target  
- Proximity to static or moving obstacles  

### Controller outputs
- Joint velocity and position commands  
- Adaptive motion updates respecting constraints  

---

## 🟢 Phase 1 — Fixed Target Control

**Objective:** Achieve accurate positioning of the manipulator’s end-effector toward a **stationary target**.  

**Approach:**  
- Implement a basic fuzzy controller using linguistic rules to map positional and angular errors into joint movements.  
- Evaluate performance under simple static conditions.  
- Establish baseline metrics for accuracy and stability.  

---

## 🟡 Phase 2 — Dynamic Target Tracking with Obstacle Avoidance

**Objective:** Enable the manipulator to **track moving targets** while maintaining safe distances from static obstacles.  

**Approach:**  
- Extend the fuzzy inference system to incorporate proximity sensing.  
- Introduce rules for collision avoidance while preserving goal-directed motion.  
- Test controller performance in scenarios with moving targets and fixed obstacles.  

---

## 🔴 Phase 3 — Advanced Control in Dynamic and Constrained Environments

**Objective:** Operate in complex, realistic environments involving **moving obstacles, dynamic targets, and joint constraints**.  

**Approach:**  
- Enhance the fuzzy rule base to account for joint limits, velocity constraints, and workspace boundaries.  
- Integrate multi-objective reasoning to balance tracking, obstacle avoidance, and kinematic feasibility.  
- Validate robustness and adaptability in dynamic, cluttered scenarios.  

---

## ⚙️ Fuzzy Inference Procedure

1. **Fuzzification:** Convert sensor readings into fuzzy sets.  
2. **Rule Evaluation:** Assess applicable linguistic rules.  
3. **Aggregation:** Combine fuzzy actions from multiple rules.  
4. **Defuzzification:** Translate fuzzy outputs into precise actuator commands.  
5. **Execution:** Apply the computed commands to the manipulator joints.  

---

## 🌍 Simulation Environment

Experiments are conducted in the **Webots simulator**, which provides:  

- Accurate physical modeling of the manipulator.  
- Realistic interaction with dynamic targets and obstacles.  
- Continuous feedback for closed-loop control validation.  

This environment allows systematic evaluation of fuzzy control strategies under reproducible conditions while safely testing scenarios that would be challenging on real hardware.

---

## 🛠 Technologies Used

- **Python** – Implementation of fuzzy control logic.  
- **Webots** – Simulator providing physics and sensory feedback.  
- **Fuzzy Logic Methodologies** – Membership functions, rule bases, defuzzification.  
- **Robotic Kinematics** – Multi-joint manipulator modeling and control.  
