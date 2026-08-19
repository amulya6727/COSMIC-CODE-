# COSMIC-CODE
# 🌌 Earth–Moon Lagrange Point Satellite Dynamics

## 🚀 Project Overview

This project demonstrates the motion and stability of a satellite placed near the five Lagrange points of the Earth–Moon system.

The project uses numerical simulation and visualization to study how a satellite behaves near:

- L1
- L2
- L3
- L4
- L5

It also allows the system parameters to be modified, including the masses of the two primary bodies and the distance between them, to observe how the Lagrange-point locations change.

---

## 🎯 Problem Statement

Demonstrate how a satellite behaves when placed near the five Lagrange points of a two-body system.

The system should also allow the user to modify:

- Mass of Planet 1 (M₁)
- Mass of Planet 2 (M₂)
- Distance between the two planets (D)

and observe how these changes affect:

- The mass ratio μ
- The locations of L1–L5
- Satellite trajectories
- Stability of the Lagrange points

---

## 🌍 Lagrange Points

Lagrange points are locations in a two-body system where the gravitational forces and orbital motion create special dynamical conditions.

The five points are:

### L1
Located between the two primary bodies.

Generally unstable.

### L2
Located beyond the smaller primary body.

Generally unstable.

### L3
Located opposite the smaller primary body.

Generally unstable.

### L4
Forms an equilateral triangle with the two primary bodies.

Stable for sufficiently small mass ratios.

### L5
The counterpart of L4 on the opposite side.

Stable for sufficiently small mass ratios.

---

## 🧮 Physics Model

The simulation uses the Circular Restricted Three-Body Problem (CR3BP).

The mass ratio is calculated as:

μ = M₂ / (M₁ + M₂)

The positions of the Lagrange points are calculated numerically for L1, L2 and L3, while L4 and L5 are obtained from their analytical coordinates.

The satellite equations of motion are numerically integrated to obtain its trajectory.

---

## 🔬 Simulation Workflow

The project follows these steps:

1. Define the masses M₁ and M₂.
2. Define the distance D between the primary bodies.
3. Calculate the mass ratio μ.
4. Calculate the five Lagrange points.
5. Place a satellite near each Lagrange point.
6. Introduce a small disturbance to the satellite.
7. Numerically calculate the satellite trajectory.
8. Compare the resulting behaviour.
9. Modify M₁, M₂ and D.
10. Recalculate the system.
11. Observe how the planets and Lagrange points change.
12. Compare the stability of the five points.

---

## 💻 Technologies Used

- Python
- NumPy
- SciPy
- REBOUND
- Manim
- Google Colab

---

## 📊 Results

The simulation demonstrates that:

| Lagrange Point | Behaviour |
|---|---|
| L1 | Unstable |
| L2 | Unstable |
| L3 | Unstable |
| L4 | Stable / Bounded |
| L5 | Stable / Bounded |

A small disturbance near the unstable points can cause the satellite to move away from the Lagrange point.

For L4 and L5, the satellite can remain in a bounded region around the equilibrium point for the simulated conditions.

---

## 🔄 Parameter Modification

The simulator allows the user to change:

```text
M₁ = Mass of Planet 1
M₂ = Mass of Planet 2
D  = Distance between the planets
