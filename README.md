# Bayesian Multi-Agent UAV Simulation for 5G Signal Optimization

This repository implements a Multi-Agent Reinforcement Learning (MARL) simulation using PyMARL, where **10 UAVs** collaborate to optimize **5G signal coverage** using **Bayesian Optimization**, **Gaussian Processes**, **Monte Carlo Dropout**, and **advanced acquisition strategies** (Thompson Sampling, Entropy Search, UCB).

## 🚁 Project Overview

- **Environment**: Custom `UAVEnv` simulates UAV behavior and 5G signal propagation in a continuous 2D map.
- **Learning Framework**: PyMARL with QMIX (or others you configure).
- **Optimization Techniques**:
  - Gaussian Process-based modeling of 5G signal field.
  - Bayesian Optimization for path planning.
  - Uncertainty quantification using Monte Carlo Dropout.
  - Acquisition functions: UCB, Thompson Sampling, and Entropy Search.
- **Visual Outputs**:
  - UAV Trajectories
  - Signal Heatmaps

---

## 🗂️ Directory Structure

```bash
pymarl/
├── src/
│   ├── envs/
│   │   └── UAVEnv.py           # Custom environment for UAV signal optimization
│   ├── config/
│   │   ├── envs/
│   │   │   └── uav.yaml        # Environment configuration
│   │   └── algs/
│   │       └── qmix_uav.yaml   # Algorithm config (e.g. QMIX for MARL)
│   └── main.py                 # Launch training and testing
