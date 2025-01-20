---
title: "Convex optimal control using Koopman operator"
excerpt: "This project studies the infinite-time horizon optimal control problem under safety constraints in its dual form by leveraging the Koopman operator. <br/><img src='https://hzyu17.github.io/hongzheyu.github.io/images/data_driven.png'>"
collection: portfolio
---

In this project, we use the Koopman operator and its dual operator to lift the optimal control problem into the space of measure, resulting in a convex optimization problem equivalent to the original optimal control problem. We then use the Sum-of-Squares (SOS) techniques to solve this optimization to obtain the optimal control signal and the controlled trajectory. The safety constraint can be naturally incoporated into our framework by using indicator functions in the measure space and be lifted as costs. For semi-algebraic sets, the whole program end up being a convex program and can be solved using off-the-shelf solvers.
