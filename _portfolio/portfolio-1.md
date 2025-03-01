---
title: "Gaussian Variational Inference Motion Planning"
excerpt: " This project studies the motion planning problem under uncertainty using Gaussian Variational Inference techniques. <br/>"
collection: portfolio
---

There is an interesting "control-inference duality", which states that the optimal control problem can be transformed into an inference problem under certaint assumption. This project studies the motion planning problem under uncertainty using Gaussian Variational Inference techniques. The goal is to find the optimal control policy that minimizes the expected cost of reaching the goal state while avoiding obstacles. The problem is formulated in the continuous-time domain and solved using the Gaussian Variational Inference (GVI) method. The GVI method approximates the posterior distribution of the hidden states using a Gaussian distribution. Sparsity of the problem is leveraged to propose a parallelizable algorithm on GPU. The proposed method is evaluated on various robot models: point robot, planar quadrotor, and robot manipulator. Our proposed method outperforms the state-of-the-art planning-as-inference methods in terms of optimallity and robustness in face of uncertainty.

Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_gvimp.png'>

Results

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/gvimp_2d_all.png'>
