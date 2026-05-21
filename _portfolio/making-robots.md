---
title: "Making Robots"
excerpt: "Robots I built from scratch: Cartrasche, SAJOGI (Spot Micro), and BOLT6.<br/><img src='/images/sajogi1.gif' width='200'>"
collection: portfolio
---

## CARTRASCHE

<iframe width="560" height="315" src="https://www.youtube.com/embed/4_D-vN_osZ8?si=-ZHxmYW6tNzZhRvq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

A "Creative Product Design" class project. Our team designed and built an **autonomous driving robot platform with a tri-shelf rotating mechanism** that follows a specific worker, provides task-specific tools, and automatically refills empty shelves to reduce labor at large manufacturing plants.

I was responsible for **constructing the actuation parts and circuit design of the whole system under restricted battery constraints**. I developed the BLDC motor control algorithm without an encoder, using only hall-sensor feedback and precise PWM control with a hand-made RC filter. We are preparing a patent and a publication for this product.

**[GitHub](https://github.com/Cartrasche-CreativeProductDesign)**

**Achievements**
- **Award:** [National ICT Smart Device Competition](https://www.msit.go.kr/bbs/view.do?sCode=user&mPid=238&mId=113&bbsSeqNo=94&nttSeqNo=3184856), **Grand Prize (1st place)**, 2024, Ministry of Science and ICT (granted by the Minister).
- **Patent:** Wonjun Kim*, Hyunjin Park*, **Minjun Chang***, Meedum Cho, Hyunjun Kim*, "AUTONOMOUS DRIVING AUXILIARY CART ROBOT FOR ASSEMBLY PROCESS," Korea (KR 1020240177135), *equal contribution.

## SAJOGI — a Spot Micro

Built a Spot Micro robot from scratch based on an [open-source model](https://www.thingiverse.com/thing:3761340).

![SAJOGI 1](/images/sajogi1.gif){: width="230" }
![SAJOGI 2](/images/sajogi2.gif){: width="230" }
![SAJOGI 3](/images/sajogi3.gif){: width="230" }

My SPOT, **SAJOGI**, uses high-torque servo motors and a *RaspberryPi 4B* controller. Twelve motors are driven by a PCA9685 driver with a modified 1200 μF capacitor. He can walk forward and crouch. LiDAR and SLAM experiments are ongoing. He has some structural defects due to unexpected motor sizing, so further work is needed to make him function perfectly.

**Code repository:** [SpotMicro_SAJOGI](https://github.com/wkdalswns0427/SpotMicro_SAJOGI)

## BOLT6 — 6DoF Bipedal Robot

Hardware configuration from the [Open Dynamic Robot Initiative](https://github.com/open-dynamic-robot-initiative/open_robot_actuator_hardware/blob/master/mechanics/biped_6dof_v1/README.md).

![BOLT6](/images/bolt6_img.jpeg){: width="250" }

*To be continued…*
