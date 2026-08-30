# 04: Virtual Obstacle-Avoiding Robot & A* Path Planning

A Python-based robotics simulation project featuring reactive obstacle avoidance and optimal global pathfinding on a 2D grid environment.

## Project Overview

This repository section contains two core computational robotics modules:
1. **Reactive Obstacle Avoidance:** A finite state decision loop simulating real-time ultrasonic sensor distance readings to dynamically stop, turn, or move forward.
2. **Global Path Planning (A* Search Algorithm):** An implementation of the $A^*$ search algorithm with Manhattan distance heuristics to calculate optimal paths around static grid obstacles.

## Technical Details & Modules

### 1. Obstacle Avoidance Simulation
* Uses randomized continuous distance readings to simulate sensor feedback.
* Executes discrete state transitions (`Move`, `Turn`, `Stop`) depending on real-time distance thresholds.

### 2. A* Pathfinding Algorithm
* **Environment:** Binary matrix representation ($0 = \text{Free Space}$, $1 = \text{Obstacle}$).
* **Heuristic:** Manhattan distance $h(n) = |x_1 - x_2| + |y_1 - y_2|$.
* **Visualization:** Uses `matplotlib` to render the grid map, start/goal positions, and the calculated optimal trajectories.

## Setup & Dependencies

Ensure you have Python installed along with the required scientific computing libraries:

```bash
pip install numpy matplotlib
