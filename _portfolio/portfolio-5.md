---
title: "Convex Optimal Control using Koopman Operator"
excerpt: "Leveraging the Koopman operator and convex relaxation to solve infinite-time horizon optimal control problems with safety constraints."
collection: portfolio
---

### Convex Optimal Control for Nonlinear Systems

This research addresses the challenging **infinite-time horizon optimal control problem** for nonlinear systems, particularly when incorporating **safety constraints**. We achieve tractability by leveraging the Koopman operator theory and solving the problem in its dual form.

The **Koopman operator**  provides a methodology to "lift" the nonlinear system dynamics into an infinite-dimensional, yet **linear**, space. By applying this transformation, the original non-convex optimal control problem is recast as a **convex optimization problem**.

**Methodology:**
* **Convex Relaxation:** We utilize the dual form of the control problem, which, when expressed in the Koopman space, admits a convex relaxation.
* **Sum-of-Squares (SOS) Optimization:** The optimal control policy and invariant safety set are found using **Sum-of-Squares (SOS)** techniques. This transformation is exact when the safety constraints are defined by polynomial functions.
* **Tractability:** The final formulation is a **convex program**, allowing for efficient and guaranteed optimal solutions using standard Semi-Definite Programming (SDP) solvers.

### Formulation
The problem minimizes an objective over an infinite horizon subject to system dynamics and safety constraints $\mathcal{C}$.

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_data_driven_SOS.png' style="width:100%; max-width:800px; margin-bottom: 20px;">

### Results
The solution demonstrates robust convergence to the optimal, safe control policy while maintaining the system state within the constrained region (represented by the feasible set).

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/data_driven.png' style="width:100%; max-width:600px;">