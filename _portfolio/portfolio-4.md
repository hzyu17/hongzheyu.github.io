---
title: "Path Integral Control for Partially Observed Systems"
excerpt: "A sampling-based control framework for nonlinear stochastic systems under partial observability, leveraging path integral control."
collection: portfolio
---

### Optimal Control under Partial Observability

This research addresses the challenge of controlling nonlinear stochastic systems where the state is not directly accessible and must be inferred from **noisy measurements**—formally known as the continuous-space Partially Observable Markov Decision Process (POMDP).

We propose a novel framework that generalizes the **Fully Observable Value Approximation** method from discrete domains to continuous-time environments. By integrating this approximation with **Path Integral Control**, we derive a sampling-based control strategy that is computationally efficient and applicable to complex nonlinear dynamics.

The resulting controller exhibits a structure analogous to classical linear controllers but retains the capability to handle significant nonlinearities and measurement noise.

### Mathematical Formulation

**Optimal Control Objective:**
We seek to minimize a cost function subject to stochastic dynamics.
<img src='https://hzyu17.github.io/hongzheyu.github.io/images/ocp.png' style="width:100%; max-width:600px; margin-bottom: 20px;">

**System Dynamics & Measurement Model:**
The system evolves according to stochastic differential equations with partial observations.
<img src='https://hzyu17.github.io/hongzheyu.github.io/images/models.png' style="width:100%; max-width:600px; margin-bottom: 20px;">

### Methodology
Our approach approximates the value function to decouple the estimation and control problems effectively.
<img src='https://hzyu17.github.io/hongzheyu.github.io/images/method_POMDP.png' style="width:100%; max-width:800px; margin-bottom: 20px;">

### Results: Comparison with EKF + iLQG

We validated our method against a standard baseline: the Extended Kalman Filter (EKF) combined with Iterative Linear Quadratic Gaussian (iLQG) control.

**Performance Analysis:**
As shown in the trajectory plots and the performance table below, our method significantly outperforms the EKF-iLQG baseline in terms of cost accumulation and robustness to noise.

<div style="display:flex; flex-direction: column; align-items: center; gap: 20px;">
  <figure style="text-align:center;">
    <img src='https://hzyu17.github.io/hongzheyu.github.io/images/result_POMDP.png' style="width:100%; max-width:700px;">
    <figcaption>Trajectory comparison demonstrating superior convergence of our method.</figcaption>
  </figure>
  
  <figure style="text-align:center;">
    <img src='https://hzyu17.github.io/hongzheyu.github.io/images/result_table_POMDP.png' style="width:100%; max-width:700px;">
    <figcaption>Quantitative comparison of costs (lower is better).</figcaption>
  </figure>
</div>