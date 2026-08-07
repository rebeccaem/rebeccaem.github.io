---
layout: page
title: Research
permalink: /research/
---

Broadly, my group works on three connected threads: discovering and exploiting **sparse structure** in high-dimensional, non-Gaussian systems, understanding **dynamical systems** through analytic (rather than purely numerical) methods, and **calibrating, validating, and quantifying uncertainty** in computational models of complex, multi-physics phenomena. Below is a rough map of the main directions, with a few representative papers linked under each &mdash; the [full publication list](/publications/) has everything.

### Sparse structure in non-Gaussian systems

Many high-dimensional systems &mdash; even strongly non-Gaussian ones &mdash; reveal simple conditional-independence structure once you look in the right coordinates. We develop algorithms, largely built on measure transport, to recover this structure directly from data, and use it to interpret and safely decouple large multi-physics codes.

- [Learning non-Gaussian graphical models via Hessian scores and triangular transport](https://www.jmlr.org/papers/v25/21-0022.html), *JMLR* 2024
- [Learning local neighborhoods of non-Gaussian graphical models](https://ojs.aaai.org/index.php/AAAI/article/view/34059), *AAAI* 2025
- [Exact mean and covariance formulas after diagonal transformations of a multivariate normal](https://www.sciencedirect.com/science/article/abs/pii/S0047259X25000843?via%3Dihub), *JMVA* 2025
- [Diagonal nonlinear transformations preserve structure in covariance and precision matrices](https://www.sciencedirect.com/science/article/abs/pii/S0047259X22000252), *JMVA* 2022

### Analytic methods for dynamical systems

Coupled ODEs get hard to simulate and analyze as the number of variables grows. Instead of just stepping through them numerically, we look for closed-form solutions and exact reductions that keep the essential dynamics intact. In particular, the Spectral Power Series (SPS) solutions give an explicit construction of the Koopman operator eigenfunctions.

- [Analytic solutions to nonlinear ODEs via spectral power series](https://www.sciencedirect.com/science/article/pii/S0024379524001940), *Linear Algebra and its Applications* 2024
- [Exact reduction of the generalized Lotka-Volterra equations via integral and algebraic substitutions](https://www.mdpi.com/2079-3197/9/5/49), *Computation* 2021

### Calibration, validation & uncertainty quantification

A lot of our work is motivated by a practical question: how do you calibrate an expensive or chaotic model against data, and then trust (or not trust) its predictions? We build stochastic operators that represent model-form error directly in the governing equations, fast calibration methods for expensive black-box codes, and UQ tools for settings like space-weather forecasting where only inputs and outputs are visible.

- [Representing model inadequacy: A stochastic operator approach](https://epubs.siam.org/doi/10.1137/16M1106419), *SIAM/ASA JUQ* 2018
- [Embedded model discrepancy: A case study of Zika modeling](https://pubs.aip.org/aip/cha/article/30/5/051103/341992/Embedded-model-discrepancy-A-case-study-of-Zika), *Chaos* 2020
- [The Ensemble Consistency Test: From CESM to MPAS and Beyond](https://gmd.copernicus.org/articles/18/2349/2025/), *Geoscientific Model Development* 2025
- Ultra-Fast unscented Kalman inversion for the calibration of expensive chaotic models, *SIAM J. Scientific Computing* (accepted)
- Accurate and Reliable Uncertainty Estimates for Deterministic Predictions: Extensions to Under and Overpredictions (in review), [arXiv](https://arxiv.org/abs/2604.08755)

### Applications

The methods above have been applied to combustion, epidemiology (Zika), climate and space weather, hypersonic/reentry-vehicle gas-surface chemistry, and structural dynamics (vibration isolation). We've also taken an interdisciplinary detour with the CU Museum of Natural History, using these tools to study the [origin of division of labor in colonial animals](https://academic.oup.com/pnasnexus/advance-article/doi/10.1093/pnasnexus/pgae476/7830526).

### Funding

Current and recent work has been supported by the National Science Foundation (including a Formal Methods in the Field award on verified probabilistic programming for hybrid systems), NASA, and the Johnson & Johnson WiSTEM2D Award. Full details are in the [CV](vita.pdf).
