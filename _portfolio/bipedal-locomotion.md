---
title: "Bipedal Locomotion"
excerpt: "<img src='/images/NetworkStructure.png' width='300'>"
collection: portfolio
---

I worked on reinforcement-learning-based bipedal robot locomotion with the Bolt10 model. The main task is to learn a robust policy that transfers well to the real world. A state-estimator MLP is concurrently trained to perform adaptive locomotion on unfamiliar terrain. The framework is shown below.

![Network structure](/images/NetworkStructure.png){: width="450" .align-center}

Simulation and training are conducted in IsaacGym (NVIDIA, CUDA 12.2) using the `rsl-rl` RL framework. Sim-to-sim verification is done in MuJoCo. Simultaneous training of the state estimator has shown improvements in sim-to-sim transfer. I intend to deploy the trained policy on a real Bolt6 robot.

**Walking in IsaacGym**

<iframe width="560" height="315" src="https://www.youtube.com/embed/gF4Cx_plCgI?si=yOIdqSnkE4pdLtKp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Walking in MuJoCo**

<iframe width="560" height="315" src="https://www.youtube.com/embed/dKqpyepDTVs?si=WnQeL3yO04mTHI_M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Other motions developed during training**

*Crouched walking*
![Crouched walking](/images/walking_crouch.gif){: width="450" .align-center}

*Swing walking*
![Swing walking](/images/bolt6_swing.gif){: width="450" .align-center}

**Poster presentation at SNU GSCST (2024.08.29)**
![DYROS poster](/images/dyros_poster.png){: .align-center}
