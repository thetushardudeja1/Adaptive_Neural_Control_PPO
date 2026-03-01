# Adaptive Neural Control of Nonlinear Robotic Systems via Proximal Policy Optimization

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-GPU-orange.svg)
![Stable-Baselines3](https://img.shields.io/badge/RL-PPO-green.svg)
![MuJoCo](https://img.shields.io/badge/Simulator-MuJoCo-red.svg)
![Status](https://img.shields.io/badge/Project-Active-success)
![License](https://img.shields.io/badge/License-Academic--Only-lightgrey)

---

## Overview

This project investigates whether **Proximal Policy Optimization (PPO)**  
can act as an adaptive neural controller for nonlinear robotic systems.

We compare:

- Classical model-based control (PD controller)
- Reinforcement learning-based neural control (PPO)

The study is conducted on a **2-DOF robotic manipulator** simulated in MuJoCo.

The primary research objective is to evaluate:

- Stability
- Control effort
- Robustness to perturbations
- Adaptation capability

---

## Research Motivation

Traditional PID/PD controllers require:

- Manual gain tuning
- Accurate system modeling
- Fixed control structure

This project explores whether a learned neural policy can:

- Replace classical controllers
- Adapt to nonlinear dynamics
- Maintain stability under uncertainty
- Reduce manual tuning effort

---

## System Description

The robotic manipulator follows nonlinear dynamics of the form:

M(q) q̈ + C(q, q̇) q̇ + G(q) = τ

Where:

- q → Joint positions
- q̇ → Joint velocities
- τ → Applied torque

Control objective:

Stabilize the manipulator around the upright configuration.

---

## Project Structure

```text
Adaptive_Neural_Control_PPO/
│
├── env/            → MuJoCo robot models
├── controllers/    → Classical PD controller implementation
├── training/       → PPO training scripts
├── experiments/    → Evaluation experiments
├── notebooks/      → Research notebooks
├── models/         → Saved trained policies
├── plots/          → Generated figures
├── results/        → Logged performance metrics
└── paper/          → Draft manuscript
```

---

## Technology Stack

- Python 3.10+
- MuJoCo physics simulator
- PyTorch (GPU accelerated)
- Stable-Baselines3 (PPO implementation)
- Gymnasium interface

---

## Experimental Workflow

1. System modeling and verification
2. Classical PD stabilization baseline
3. PPO-based adaptive control training
4. Performance metric evaluation
5. Robustness analysis
6. Comparative study

---

## Current Progress

- [x] 2-DOF robotic manipulator model
- [x] PD baseline stabilization
- [x] PPO stabilization training
- [ ] Robustness evaluation
- [ ] Comparative analysis
- [ ] Manuscript preparation

---

## Academic Notice

All rights reserved.

This repository is part of an academic research project.

No permission is granted to reproduce, distribute, or use
any portion of this work without explicit written permission
from the author.

---

## Author

Tushar Dudeja  
Control Systems Project  
2025–26