---
title: "Path Integral Control for Partially Observed Systems"
excerpt: " This project studies path integral control for nonlinear stochastic systems with partial observations. <br/>"
collection: portfolio
---

### Controlling Systems with Incomplete Information 

This research focuses on controlling a system when you can't see its full state directly, and instead must rely on **noisy measurements**. This is a **partially observed control problem**. 

To solve this, we adapted a method called **fully observable value approximation**—originally for simple, discrete systems—to work in continuous, real-world environments. 

The resulting algorithm provides a controller that's similar to those used in simpler linear systems. By combining it with the **path integral control method**, our approach allows us to create an effective control strategy for systems where our information is incomplete.

Formulation

Optimal Control Objective:

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/ocp.png'>

Dynamical System and Measurement Models:

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/models.png'>

Method:

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/method_POMDP.png'>

Results: out-performed EKF+iLQG

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/result_POMDP.png'>

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/result_table_POMDP.png'>