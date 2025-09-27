---
title: "Gaussian Variational Inference Motion Planning"
excerpt: " This project studies the motion planning problem under uncertainty using Gaussian Variational Inference techniques. <br/>"
collection: portfolio
---

There is an interesting "control-inference duality", which states that the optimal control problem can be transformed into an inference problem under certaint assumption. This project studies the motion planning problem under uncertainty using Gaussian Variational Inference techniques. The goal is to find the optimal control policy that minimizes the expected cost of reaching the goal state while avoiding obstacles. The problem is formulated in the continuous-time domain and solved using the Gaussian Variational Inference (GVI) method. The GVI method approximates the posterior distribution of the hidden states using a Gaussian distribution. Sparsity of the problem is leveraged to propose a parallelizable algorithm on GPU. The proposed method is evaluated on various robot models: point robot, planar quadrotor, and robot manipulator. Our proposed method outperforms the state-of-the-art planning-as-inference methods in terms of optimallity and robustness in face of uncertainty.

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