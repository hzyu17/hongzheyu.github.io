---
title: "Decentralized Field Coverage with Micro-Drone Swarms"
excerpt: "Implementing a decentralized coverage control strategy on micro-drone hardware with collision avoidance and deadlock resolution."
collection: portfolio
---

### Autonomous Area Coverage

This project implements a **decentralized control strategy** for optimal area coverage using a swarm of micro-drones, validated on hardware using Vicon motion capture.

**Methodology:**
* **Sensor Modeling:** We model sensor efficacy using a bell-shaped function. The control law drives the drones to maximize total area coverage based on the vector sum of attraction forces within their sensor range.
* **Robustness & Safety:** We integrated a switching control strategy to resolve local minima (deadlocks) and employed **Artificial Potential Fields (APF)** to ensure real-time collision avoidance between agents.

### Video Demonstration
<div style="text-align: center;">
  <a href="https://www.youtube.com/watch?v=SJ7_cbu2aSc">Watch the coverage experiment</a>
</div>