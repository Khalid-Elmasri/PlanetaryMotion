# Planetary Motion Simulator

A computational physics project that models planetary and exoplanetary motion using Keplerian orbital mechanics, numerical methods, and scientific visualization.

![Python](https://img.shields.iohon-3.11-blue)
![NumPy](https://img.shields.iomPy-Scientific%20Computing-orange)
![Matplotlib](https:///badge/Matplotlib-Visualization-green)
![Physics](https://img.shdge/Domain-Orbital%20Mechanics-purple)

---

## Overview

This project simulates the motion of planets orbiting a central star using classical orbital mechanics.

The simulation solves Kepler's Equation numerically using the Newton-Raphson method, computes orbital trajectories, and generates visualizations and animations of planetary motion. The project also investigates the behaviour of close-orbiting exoplanets known as *Hot Jupiters*, where short orbital periods introduce additional numerical challenges.

The aim of this project is to combine mathematical modelling, numerical analysis, and scientific programming to reproduce realistic orbital dynamics.

---

## Key Features

- Numerical solution of Kepler's Equation
- Newton-Raphson root-finding implementation
- Elliptical orbit generation
- Earth-Sun system simulation
- Orbit trajectory visualisation
- Animated orbital motion
- Hot Jupiter exoplanet case study
- Numerical stability investigation
- Scientific plotting and analysis

---

## Scientific Background

Planetary motion is governed by Newtonian gravitation and Kepler's Laws.

For elliptical orbits, Kepler's Equation relates mean anomaly and eccentric anomaly:

\[
M = E - e\sin(E)
\]

where

- \(M\) = Mean Anomaly
- \(E\) = Eccentric Anomaly
- \(e\) = Orbital Eccentricity

Since this equation has no general analytical solution, numerical methods are required.

This project solves the equation iteratively using the Newton-Raphson method.

---

## Earth-Sun Simulation

The Earth-Sun system is used as a benchmark case.

### Parameters

| Parameter | Value |
|------------|---------|
| Semi-Major Axis | 1 AU |
| Eccentricity | 0.0167 |
| Orbital Period | 365.25 days |

### Example Output

<p align="center">
  <img src="results/earth_orbit.The simulation reproduces the expected nearly-circular elliptical orbit, with the Sun located at one focus of the orbit.

---

## Orbit Animation

Animated visualisations track the position of Earth throughout one complete orbital period.

orbit_animation.gif

---

## Exoplanet Case Study: Hot Jupiter

To test the robustness of the model, a close-orbiting gas giant exoplanet was simulated.

### System Parameters

| Parameter | Value |
|------------|------------|
| Star Mass | 1.11 M☉ |
| Planet Mass | 0.46 MJ |
| Semi-Major Axis | 7.83 × 10⁹ m |
| Orbital Period | ≈ 4.23 days |

Because the orbital period is significantly shorter than Earth's, numerical integration requires smaller time steps to maintain stability and accuracy.

### Example Output

<p align="center">
  <img src="results/hot_jit.png
</p>

The system was evolved across hundreds of orbital periods to investigate long-term stability.

---

## Numerical Stability Analysis

Numerical simulations depend strongly on the chosen integration time step.

This project investigates:

- Stability over long simulations
- Positional drift
- Computational cost
- Time-step sensitivity

Example analysis:

<p align="center">
  <img src="results/stability_analysis
This helps identify suitable numerical parameters for reliable orbital simulations.

---

## Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- Scientific Computing
- Numerical Methods

---

## Skills Demonstrated

This project demonstrates:

### Programming

- Object-oriented design
- Scientific Python development
- Data visualisation

### Mathematics

- Numerical root finding
- Trigonometry
- Differential equations

### Physics

- Orbital mechanics
- Newtonian gravity
- Keplerian motion

### Data Analysis

- Model validation
- Stability analysis
- Computational experimentation

---

## Future Improvements

Potential extensions include:

- N-body gravitational simulations
- Multi-planet systems
- Solar System model
- Energy conservation diagnostics
- Relativistic corrections
- GPU acceleration
- Interactive visualisation dashboard

---

## Installation

```bash
git clone https://github.com/yourusername/planetary-motion-simulator.git

cd planetary-motion-simulator

pip install -r requirements.txt
```

---

## Running the Project

```bash
jupyter notebook
```

or

```bash
python src/orbit.py
```
