# Fuzzy-Logic-Control-of-a-Robotic-Manipulator


Computational Intelligence Course Project 

Design and implementation of a fuzzy inference–based controller for autonomous motion, target tracking, and obstacle avoidance of a robotic arm in the Webots simulator using Python.

---

## 📌 Project Overview

This project investigates the application of **Fuzzy Logic Control (FLC)** to robotic manipulation tasks.

A multi-joint manipulator must reach targets, adapt to environmental changes, and avoid collisions.  
Instead of classical model-based control, decision making is performed through **linguistic rules and fuzzy inference**.

The implementation is developed in **Python** and tested inside a physics-based robotic simulation.

---

## 🎯 Objectives

- Design fuzzy membership functions for perception variables.
- Develop rule-based decision systems.
- Convert fuzzy outputs into executable motor commands.
- Evaluate tracking accuracy and safety.
- Extend the controller toward dynamic and constrained environments.

---

## 🧠 Skills & Concepts Demonstrated

- Fuzzy inference systems (Mamdani / Sugeno)
- Membership function design
- Rule base construction
- Defuzzification methods
- Autonomous robotics
- Sensor-based control
- Simulation-driven validation

---

---

# 🟢 Phase 1 — Static Target Reaching

## Goal
Move the manipulator end-effector toward a **fixed point** in space.

## Inputs (examples)
- Joint angles  
- Joint velocities  
- Distance to target  

## Fuzzy Design

Typical linguistic variables:

- Distance → *near*, *medium*, *far*
- Joint speed → *slow*, *normal*, *fast*

## Outputs
- Motion commands  
- Velocity adjustments  

## Evaluation
- Accuracy of reaching the target  
- Smoothness of motion  
- Stability of the controller  

---

---

# 🟡 Phase 2 — Target Tracking with Obstacle Avoidance

## Goal
Enhance the controller to:

- follow the target  
- detect obstacles  
- avoid collisions  

## Additional Inputs
- Distance to nearest obstacle  
- Relative motion information  

## Example Rules
- If obstacle is **very close** → reduce speed.
- If obstacle is **close** and target is far → change direction.
- If obstacle is **far** and target is near → increase speed.

## Expected Behavior
The robot should reach the goal while maintaining safe clearance.

---

---

# 🔴 Phase 3 — Dynamic & Constrained Environment

## Goal
Operate in a more realistic scenario including:

- moving obstacles  
- actuator limits  
- speed constraints  
- workspace boundaries  

## Controller Requirements
The system must **prioritize multiple objectives simultaneously**:

- follow moving targets  
- avoid collisions  
- respect joint limits  
- maintain smooth trajectories  

## Advanced Rule Design
Rules may adapt priorities dynamically depending on the situation.

---

---

## ⚙️ Fuzzy Inference Procedure

1. Fuzzification of sensory inputs.
2. Rule evaluation.
3. Aggregation of outputs.
4. Defuzzification (e.g., centroid method).
5. Apply commands to joints.

---

## 🛠 Technologies Used

- Python  
- Webots  
- Fuzzy logic principles  
- Robotic kinematics  

---


