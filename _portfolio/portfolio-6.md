---
title: "Environment Representation in Sim-to-Real Imitation Learning"
excerpt: "Evaluating the impact of sensor fusion and semantic abstraction on sim-to-real transfer for robot navigation."
collection: portfolio
---

### Bridging the Sim-to-Real Gap via Semantic Representations

This project investigates how different environmental representations affect the transfer of navigation policies from simulation to the real world (**Sim-to-Real**).

We employed an **imitation learning** framework to train a collision-avoidance policy using synthetic sensor data. The core study focused on evaluating various sensor fusion strategies before feeding the data into the neural control policy.

**Key Findings:**
Real-world experiments revealed that **categorical and semantic information** (e.g., semantic segmentation) is far more critical for robust navigation than low-level visual features like color or texture. This suggests that abstracting the environment is key to successful sim-to-real transfer.

### Methodology & Network Architecture
<div style="text-align: center;">
    <img src='https://hzyu17.github.io/hongzheyu.github.io/images/local_navigation_method.png' style="width:100%; max-width:600px; margin: 0 auto;">
</div>

### Video Demonstration
[Watch the experiment video](https://youtu.be/ucGyuMjlgEk)