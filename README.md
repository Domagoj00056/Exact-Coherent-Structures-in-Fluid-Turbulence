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

## Abstract

We consider the incompressible Navier–Stokes equations body-forced by $\sin(4y)\hat{x}$ on the torus $(x,y)\in[0,2\pi]^2$, with the aim of extracting unstable recurrent flows from high-dissipation regions. Each recurrent flow describes a closed cycle within the state space and, when considered collectively, may provide a framework for describing long-time turbulent dynamics and statistics. In particular, unstable periodic orbits (UPOs) and relative periodic orbits (RPOs) represent recurrent behaviour within the flow, capturing recurring patterns of evolution within the turbulent dynamics. Near-recurrent episodes are identified from DNS using the modified recurrence function $R_K$, and subsequently converged to exact invariant solutions using the Newton–GMRES–Hookstep method. High-dissipation regions, corresponding to extreme bursting events, contain fewer close recurrences, making them more difficult to identify using the recurrence approach. A DNS trajectory of duration $10^4$ was analysed, producing 445 initial guesses, of which 14 converged to eight unique invariant solutions.


---

## Main Results

A DNS trajectory of approximately $10^4$ time units was analysed to generate initial guesses for invariant solutions.

From **445 initial guesses**, **14 converged solutions** were obtained, corresponding to **8 unique invariant solutions**.

These included:

- periodic orbits (POs),
- relative periodic orbits (RPOs),
- a travelling wave,
- and an equilibrium solution.

A particular focus was placed on solutions extending into the high-dissipation region of the turbulent dynamics.

Two of the recovered relative periodic orbits, **R3 and R4**, have

$$
\bar D = 0.1905
$$

and

$$
\bar D = 0.1928,
$$

respectively.

These solutions extend substantially into the high-dissipation region and were not matched to corresponding invariant solutions in the literature surveyed for the dissertation.

The periodic orbit P1 closely matches the previously reported \(P_2\) solution of Chandler & Kerswell (2013), while the travelling wave TW1 corresponds closely to a solution identified by Farazmand (2016). These comparisons provide useful validation of the numerical approach. In contrast, R3 and R4 extend into the high-dissipation region of the turbulent dynamics and may represent previously unreported relative periodic orbits.

## Method

The computational workflow can be summarised as:

1. Perform DNS of two-dimensional Kolmogorov flow and monitor the dissipation.
2. Target high-dissipation events and identify near recurrences using the modified recurrence function $R_K$.
3. Refine near-recurrent states into exact invariant solutions using Newton–GMRES–Hookstep.
4. Classify and analyse the converged solutions 

---

## Dissertation

The complete MSc dissertation is available here:

**[Download the dissertation](https://github.com/Domagoj00056/Exact-Coherent-Structures-in-Fluid-Turbulence/blob/main/DISS%20STA.pdf)**

---



## Related Work

This project builds on previous work on recurrent and invariant solutions in turbulent Kolmogorov flow, including:

- Chandler & Kerswell (2013), *Invariant recurrent solutions embedded in a turbulent 2D Kolmogorov flow*.
- Farazmand (2016), work on the computation of invariant solutions using adjoint-based methods.
- Redfern, Lazer & Lucas (2024), work investigating dynamically relevant recurrent flows and high-dissipation events.

---

## Acknowledgements

I would like to thank **Dr Dan Lucas** for his supervision and guidance throughout the project, and the **School of Mathematics at the University of St Andrews** for the opportunity to work on this project.


