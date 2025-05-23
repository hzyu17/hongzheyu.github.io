---
title: "Covariance Control for Hybrid Systems"
excerpt: " This project studies covariance control for linear stochastic systems with hybrid transitions. <br/>"
collection: portfolio
---

Robotic systems in contact with the environment can be modeled as hybrid systems, yet controlling them under disturbances is challenging due to discontinuous jump dynamics, varying state dimensions, and noise-induced timing shifts. 

For \textit{linear} stochastic flows with hybrid transitions, I developed Hybrid Covariance Steering (H-CS) to control state covariances around a mean trajectory, approximating jump dynamics with the Saltation Matrix. When jumps are nonsingular, this yields a closed-form solution; otherwise, a convex optimization over path distributions is formulated via Schrodinger’s Bridge duality, enforcing covariance propagation at hybrid events as equality constraints. This approach scales linearly with the number of jumps, enabling efficient, optimal solutions.

Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_hcs.png'>

Results

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/h_cs_slip_samples.png'>