---
title: "Environment representation in sim-to-real imitation learning based robot navigation"
excerpt: "This project studies the . <br/>"
collection: portfolio
---

In this project, we studied the impact of environment representations (sensor data fusion) in imitation-learning based sim-to-real robot navigation tasks. We applied different sensor data fusion methods on raw data collected in a simulated (ROS Gazebo) environment, and feeded the fused data to train a neural network that learns a local collision-avoiding policy for navigation tasks. The model was then deployed directly in real-world hardwares for similar tasks. We tested the test-time performances under fused sensor data inputs from different representations. We found that the categorical and semantic information are more critical than textual and color information for navigation tasks.

Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/local_navigation_method.png'>


[Video Introduction](https://youtu.be/ucGyuMjlgEk)