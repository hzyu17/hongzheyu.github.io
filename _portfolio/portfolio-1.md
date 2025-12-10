---
title: "Gaussian Variational Inference Motion Planning"
excerpt: "Leveraging control-inference duality for robust motion planning under uncertainty via Gaussian Variational Inference."
collection: portfolio
---

This project leverages **Gaussian Variational Inference (GVI)** to address motion planning under uncertainty, grounded in the framework of control-inference duality.

We formulate the planning objective as a continuous-time trajectory optimization problem. By approximating the trajectory distribution as a Gaussian, our method simultaneously minimizes control costs and obstacle collision risks. The algorithm exploits the problem's inherent sparsity to enable efficient, parallelizable GPU execution.

Validated on point robots, quadrotors, and manipulators, this approach demonstrates superior optimality and robustness compared to state-of-the-art planning-as-inference techniques.

### Formulation
<img src='https://hzyu17.github.io/hongzheyu.github.io/images/formulation_gvimp.png' style="width:100%; max-width:800px;">

### Video Demonstration
[Watch the detailed results and experiments here](https://www.youtube.com/watch?v=c4sFOlEki0Q)

### Results: 7-DOF Robot Arm Comparison
*Comparison of robustness against disturbances between classical RRT-Connect and our GVIMP method.*

<div style="display:flex; justify-content:center; gap:2rem; margin-top: 1em;">
  <figure style="margin:0; text-align:center;">
    <img src="https://hzyu17.github.io/hongzheyu.github.io/images/RRTConnect_disturbed.png"
         alt="RRT-Connect Performance"
         style="max-width:100%; height:auto; border: 1px solid #ddd;">
    <figcaption style="margin-top:0.5em; font-style:italic; font-size: 0.9em;">
      (a) RRT-Connect (Baseline)
    </figcaption>
  </figure>

  <figure style="margin:0; text-align:center;">
    <img src="https://hzyu17.github.io/hongzheyu.github.io/images/GVIMP_disturbed.png"
         alt="GVIMP Performance"
         style="max-width:100%; height:auto; border: 1px solid #ddd;">
    <figcaption style="margin-top:0.5em; font-style:italic; font-size: 0.9em;">
      (b) GVIMP (Ours)
    </figcaption>
  </figure>
</div>