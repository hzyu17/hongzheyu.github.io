---
title: "Path Integral Control for Hybrid Systems"
excerpt: " This project studies path integral control for nonlinear stochastic systems with hybrid transitions. <br/>"
collection: portfolio
---

Robotic systems in contact with the environment can be modeled as hybrid systems, yet controlling them under disturbances is challenging due to discontinuous jump dynamics, varying state dimensions, and noise-induced timing shifts. 

For \textit{nonlinear} flows, I introduced the Hybrid Path Integral (H-PI) framework, leveraging an analogous ratio among hybrid path distributions to derive the optimal controller via a path integral. Importance sampling with a Hybrid iLQR-based proposal distribution reduces variance, and extensive numerical experiments confirm the effectiveness of both methods across various hybrid systems.

Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_h_pi.png'>

Results

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/method.png'>