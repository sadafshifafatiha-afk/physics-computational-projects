# 03: DC Motor Speed Control via PID Simulation

A discrete-time Python implementation and simulation of a DC motor speed control system using a Proportional-Integral-Derivative (PID) controller.

## Project Overview

This project simulates dynamic feedback speed control for a DC motor under a discrete-time framework. The PID controller continuously calculates an error value as the difference between a desired target speed (setpoint) and a measured motor speed, applying corrections based on proportional, integral, and derivative terms.

## Key Features

* **Discrete-Time Control Loop:** Implements standard discrete numerical updates for PID feedback logic.
* **Tunable Gains:** Allows easy adjustment of Proportional ($K_p$), Integral ($K_i$), and Derivative ($K_d$) parameters to analyze step response, overshoot, and settling time.
* **Data Visualization:** Generates plots comparing the actual system response curve against the target setpoint using `matplotlib`.

## Technical Summary & Parameters

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Setpoint** | `50.0` | Target rotational speed unit |
| **$K_p$** | `0.80` | Proportional gain (error correction) |
| **$K_i$** | `0.20` | Integral gain (accumulated error offset) |
| **$K_d$** | `0.05` | Derivative gain (rate of change damping) |
| **Time Span** | `0 - 10 s` | Simulation duration |





