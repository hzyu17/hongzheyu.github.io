---
title: "Covariance Control for Hybrid Systems"
excerpt: "Optimal covariance steering for linear stochastic systems with hybrid transitions, applicable to contact-rich robotics."
collection: portfolio
---

### Controlling Robots in Contact-Rich Environments

Controlling robotic systems in contact-rich environments (e.g., legged locomotion or manipulation) is challenging due to the presence of hybrid dynamics—systems that involve both continuous evolution and discrete mode switches—compounded by stochastic noise.

This research introduces **Hybrid Covariance Steering (H-CS)**, a control framework designed to steer the distribution of the system state across hybrid transitions. Rather than tracking a single deterministic trajectory, H-CS regulates the covariance of the system state to ensure robust performance.

**Key Contributions:**
* **Closed-Form Solutions:** For systems with fixed mode sequences, we derive explicit, closed-form optimal control policies.
* **Convex Optimization:** For autonomous mode-switching, we reformulate the intractable problem into a convex Semi-Definite Program (SDP).
* **Scalability:** The approach is computationally efficient, scaling linearly with the number of hybrid jumps, providing a fast and optimal solution for complex stochastic systems.

### Mathematical Formulation
The problem is framed as steering the state distribution through a sequence of hybrid jumps while minimizing control effort and state deviation.

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_hcs.png' style="width:100%; max-width:800px; margin-bottom: 20px;">

### Equivalent Convex SDP Formulation
By lifting the dynamics into a higher-dimensional space, we convert the covariance steering problem into a solvable convex optimization problem.

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/hcs_SDP.png' style="width:100%; max-width:800px; margin-bottom: 20px;">

### Results: Stochastic Spring-Loaded Inverted Pendulum (SLIP)
The figure below demonstrates the H-CS controller applied to a SLIP model. The algorithm successfully regulates the state distribution (shown as ellipses) through ground impacts, maintaining stability despite stochastic disturbances.

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/h_cs_slip_samples_stable.png' style="width:100%; max-width:600px;">