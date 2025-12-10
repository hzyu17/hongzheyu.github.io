---
title: "Gaussian Variational Inference Motion Planning"
excerpt: " Solve Motion Planning Problem under Uncertainty using Variational Inference. <br/>"

collection: portfolio
---

This project applies Gaussian Variational Inference (GVI) to solve motion planning problems under uncertainty, a method inspired by the "control-inference duality."

The objective is to find the best way for a robot to reach a goal, minimizing cost and avoiding obstacles, even when faced with uncertainty. We formulate the problem in a continuous-time framework and use GVI to approximate the robot's possible paths as a Gaussian distribution.

By leveraging the problem's sparsity, we developed an algorithm that can run in parallel on a GPU, significantly improving performance. Our approach has been successfully tested on various robots, including a point robot, a quadrotor, and a manipulator. The results show that our method is more optimal and robust than other leading planning-as-inference techniques.

### Formulation

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_gvimp.png'>

### Results: [(More results available in this video)](https://www.youtube.com/watch?v=c4sFOlEki0Q) 

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/RRTConnect_disturbed.png'>

<img src='https://hzyu17.github.io/hongzheyu.github.io/images/GVIMP_disturbed.png'>

### Video 

[Hardware experiment results]()

#### 7-DOF Robot Arm: Comparison with classical sampling based planning algorithm (RRT-Connect)
<div style="display:flex; justify-content:center; gap:2rem;">
  <figure style="margin:0; text-align:center;">
    <img src="https://hzyu17.github.io/hongzheyu.github.io/images/RRTConnect_disturbed.png"
         alt="RRTConnect disturbed"
         style="max-width:100%; height:auto;">
    <figcaption style="margin-top:0.4em; font-style:italic;">
      (a) RRT-Connect 
    </figcaption>
  </figure>

  <figure style="margin:0; text-align:center;">
    <img src="https://hzyu17.github.io/hongzheyu.github.io/images/GVIMP_disturbed.png"
         alt="GVIMP disturbed"
         style="max-width:100%; height:auto;">
    <figcaption style="margin-top:0.4em; font-style:italic;">
      (b) GVIMP 
    </figcaption>
  </figure>
</div>