# Rapid-Exploring Random Tree (RRT) Implementation

This repository contains a Python implementation of a Rapidly-exploring Random Tree (RRT)-style planner, along with a helper script related to grasp inverse kinematics.

> **Files**
- `adarrt.py` — RRT-based planner implementation (adaptive / goal-biased / variant-style RRT, depending on how you configured it).
- `soda_grasp_ik.py` — utilities for computing IK for a “soda can grasp” style task (robot/manipulator grasp pose / joint solution helper).

---

## What is RRT?

Rapidly-exploring Random Trees (RRT) are sampling-based motion planning algorithms that efficiently explore high-dimensional spaces to find a collision-free path from a start state to a goal state. They are widely used in robotics because they are:
- **Probabilistically complete** (given enough samples, they will find a solution if one exists),
- Practical in **high-dimensional configuration spaces** (e.g., robot arms),
- Easy to extend with heuristics like goal-biasing, adaptive step sizes, or constraint checks.

---

## Project Structure

```text
.
├── adarrt.py
└── soda_grasp_ik.py
