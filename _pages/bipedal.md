---
permalink: /rnp/bl/
title: "Bipedal Locomotion"
toc: false
toc_sticky: true
---
<span style="font-size:0.8em;">
    I worked on reinforcement learning based bipedal robot locomotion with Bolt10 model. Main task is to configure profound policy that applies well on real world robot. State-Estimator Multi Layer Perceptron was concurrently trained to perform adaptive locomotion on alien terrains. The framework is as below.
    <br>![image](/assets/images/NetworkStructure.png){: width="450" height="450"  .align-center}
    <br>Simulation and learning is conducted on IsaacGym(NVIDIA) framework with cuda12.2. using RL framework rsl-rl. Sim2Sim vertification was done on MuJoCo. Simultaneous training of state estimator has shown improvements on Sim2Sim performance on policy training. I intend to implement trained policies on real Bolt6 robot.
</span>
<br><span style="font-size:0.8em;">**Walking in IsaacGym Env**</span><br>
![gif](/assets/images/walking_bolt6.gif){: width="450" height="450"  .align-center}
<br><span style="font-size:0.8em;">**Walking in MuJoCo Env**</span><br>
![gif](/assets/images/mujoco_walk_well.gif){: width="450" height="450"  .align-center}

<br><span style="font-size:0.9em;">**Below are some other motions made during training**</span>
<br><span style="font-size:0.8em;">**Crouched Walking**</span><br>
![gif](/assets/images/walking_crouch.gif){: width="450" height="450" .align-center}
<br><span style="font-size:0.8em;">**Swing Walking**</span><br>
![gif](/assets/images/bolt6_swing.gif){: width="450" height="450" .align-center}
<br>
<br><span style="font-size:0.9em;">**Poster Presentation at SNU GSCST(2024.08.29)**</span><br>
![image](/assets/images/dyros_poster.png){: .align-center}

> This page will be updated as my research proceeds.