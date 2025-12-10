---
title: "Convex optimal control using Koopman operator"
excerpt: "This project studies the infinite-time horizon optimal control problem under safety constraints in its dual form by leveraging the Koopman operator. <br/>"
collection: portfolio
---

### Controlling Complex Systems Using a New Mathematical Approach

This project uses a mathematical tool called the **Koopman operator** to solve a complex control problem.

Instead of solving the original problem directly, we "lift" it into a new, simplified space where it becomes a **convex optimization problem**. This is a type of problem that is much easier to solve.

To find the best solution—the optimal control signal and the system's trajectory—we use a method called **Sum-of-Squares (SOS)**. We can also easily add **safety constraints** to our framework by including them as part of the optimization problem.

When the constraints are defined by simple polynomial equations, the entire program becomes a **convex program**, which can be solved efficiently using existing software.
Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_data_driven_SOS.png'>

Results

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/data_driven.png'>