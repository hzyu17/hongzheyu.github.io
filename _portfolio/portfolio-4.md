---
title: "Path Integral Control for Partially Observed Systems"
excerpt: " This project studies path integral control for nonlinear stochastic systems with partial observations. <br/>"
collection: portfolio
---

This study considers a partially observed optimal control problem in which the state is measured through a noisy output, focusing on continuous-time and continuous-space settings.
To develop a control algorithm for this challenging problem, we extend the so-called fully observable value approximation, originally developed for the partially observable Markov decision problems (POMDPs) in discrete-time and discrete-space domains, to the continuous ones.
The approximation yields a suboptimal controller with a structure analogous to that of a controller obtained through the separation principle for the so-called linear-quadratic settings.
Combined with the path integral control method, the proposed extension allows for a suboptimal policy synthesis for partially observable systems.

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