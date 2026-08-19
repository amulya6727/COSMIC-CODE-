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

## 🎥 Demonstration of the Solution
At L1, the satellite moves away from the equilibrium region, demonstrating its unstable nature. Similarly, at L2, the satellite does not remain near the equilibrium point. L3 also shows unstable behaviour under a small disturbance. At L4, however, the satellite remains within a bounded region around the point. This demonstrates the stable behaviour of L4 for the chosen mass ratio. L5 shows similar bounded behaviour.
In my visualization, red represents the unstable points L1, L2 and L3, while green represents the stable or bounded points L4 and L5. The yellow satellite and cyan trajectory make the motion easier to observe.


## 🧠 Assumptions
My simulation makes some simplifying assumptions.
# Assumption 1 — Circular orbits
    I assumed the two primary bodies follow approximately circular orbits around their common centre of mass.
    That's why I used the Circular Restricted Three-Body Problem.
# Assumption 2 — Negligible satellite mass
    I assumed the satellite has negligible mass compared with the two primary bodies, so its gravitational effect on them is     ignored.
# Assumption 3 — Idealized system
    I treated the system as an ideal two-body system and do not include effects such as other planets, solar perturbations,      atmospheric drag or radiation pressure.
# Assumption 4 — Numerical simulation
    The satellite trajectories are obtained numerically, so the results depend on the integration time, initial conditions       and numerical tolerances.


## ⚠️ Limitations

Because of these assumptions, my simulation is not intended to be an exact prediction of a real spacecraft trajectory. Instead, it is a physics-based model for understanding Lagrange-point dynamics and how system parameters influence them.
    

## 🔄 Parameter Modification

The simulator allows the user to change:

```text
M₁ = Mass of Planet 1
M₂ = Mass of Planet 2
D  = Distance between the planets



