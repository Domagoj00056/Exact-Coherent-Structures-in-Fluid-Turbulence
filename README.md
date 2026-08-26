# Exact Coherent Structures in Fluid Turbulence

**MSc Mathematics Dissertation — University of St Andrews, 2026**

**Author:** Domagoj  
**Supervisor:** Dr Dan Lucas

---

## Overview

This project investigates **exact coherent structures in turbulent flow** from a dynamical-systems perspective.

The study considers two-dimensional **Kolmogorov flow** at Reynolds number $Re = 40$ and focuses on identifying recurrent and invariant solutions embedded within the turbulent dynamics.

In particular, the project investigates whether invariant solutions can be identified in the **high-dissipation, low-probability regions** of the turbulent trajectory, where close recurrences are comparatively rare.

The approach combines recurrence analysis with the **Newton–GMRES–Hookstep** method to refine near-recurrent flow fields into exact invariant solutions.

---

## Main Results

A DNS trajectory of approximately \(10^4\) time units was analysed to generate initial guesses for invariant solutions.

From **445 initial guesses**, **14 converged solutions** were obtained, corresponding to **8 unique invariant solutions**.

These included:

- periodic orbits (POs),
- relative periodic orbits (RPOs),
- a travelling wave,
- and an equilibrium solution.

A particular focus was placed on solutions extending into the high-dissipation region of the turbulent dynamics.

Two of the recovered relative periodic orbits, **R3 and R4**, reach

\[
D/D_{\mathrm{lam}} = 0.1905
\]

and

\[
D/D_{\mathrm{lam}} = 0.1928,
\]

respectively.

These solutions extend substantially into the high-dissipation region and were not matched to corresponding invariant solutions in the literature surveyed for the dissertation.

The periodic orbit **P1** closely matches the previously reported \(P_2\) solution of Chandler & Kerswell (2013), providing a useful comparison with earlier work.

---

## Visualisation

The \(I-D\) plane shows the energy input and dissipation of the flow, with the DNS probability density shown in the background.

The invariant solutions are then plotted as trajectories through this plane.

The accompanying vorticity visualisations show the corresponding evolution of the physical flow field.

### Periodic orbit in the typical turbulent region

This animation shows a periodic orbit located predominantly in the high-probability region of the DNS.

### High-dissipation recurrent solution

This animation shows a relative periodic orbit recovered by targeting the low-probability, high-dissipation region of the turbulent dynamics.

---

## Method

The computational workflow can be summarised as:

1. Perform direct numerical simulation (DNS) of Kolmogorov flow.
2. Monitor the dissipation and identify high-dissipation events.
3. Search for approximate recurrences within the DNS trajectory.
4. Use the recurrent flow fields as initial guesses.
5. Refine the guesses using Newton–GMRES–Hookstep.
6. Identify converged invariant solutions.
7. Remove duplicates and classify the resulting solutions.
8. Analyse their location within the turbulent \(I-D\) distribution.

---

## Dissertation

The complete MSc dissertation is available here:

**[Download the dissertation](Dissertation.pdf)**

---

## Code

The main computational work was carried out in Python.

The repository contains the relevant notebooks and Python scripts used for:

- DNS analysis,
- recurrence detection,
- invariant-solution searches,
- vorticity reconstruction,
- dissipation/input calculations,
- and visualisation.

---

## Related Work

This project builds on previous work on recurrent and invariant solutions in turbulent Kolmogorov flow, including:

- Chandler & Kerswell (2013), *Invariant recurrent solutions embedded in a turbulent 2D Kolmogorov flow*.
- Farazmand (2016), work on the computation of invariant solutions using adjoint-based methods.
- Redfern, Lazer & Lucas (2024), work investigating dynamically relevant recurrent flows and high-dissipation events.

---

## Acknowledgements

I would like to thank **Dr Dan Lucas** for his supervision and guidance throughout the project, and the **School of Mathematics at the University of St Andrews** for the opportunity to work on this project.

---

## Repository Structure

```text
.
├── Dissertation.pdf
├── README.md
├── code/
│   ├── Kflow-NGh.ipynb
│   ├── functions.py
│   └── parameters.py
├── figures/
└── animations/
