---
title: "Humanoid Motion Retargeting"
excerpt: "<img src='/images/RobotSpecificMotion.png' width='300'>"
collection: portfolio
order: 1
---

![Robot-specific motion](/images/RobotSpecificMotion.png){: .align-center}

I study what a construction worker's demonstrated motion should carry onto a humanoid. The demonstration gives the robot the task. It does not have to give the robot the worker's joint angles. All experiments run on an adult-sized Unitree H1-2.

## Robot-Specific Execution

I compared human-derived motion against robot-specific motion over a material-handling sequence. Human-derived motion was captured by vision and retargeted onto the robot. Robot-specific motion used inverse kinematics and minimum-jerk transfers to reach the same targets from a different posture. Robot-specific motion finished the sequence in less time, over a shorter trajectory and at lower mechanical work. I scored both conditions with RULA to confirm they were different movement strategies.

**Publication:** **Minjun Chang**, Taehyung Kim, Yong K. Cho, Francis Baek, "Beyond Human-Derived Motion: Exploring Robot-Specific Execution for Construction Humanoids," *IROS 2026 Workshop on the Future of Construction*.

## Task-Defined Retargeting

I found that the worker's configuration enters a retargeted reference through two routes. The first is the posture term in the solver. The second is the wrist target itself, which is built from the worker's limb directions and inherits the worker's arm extension. Setting the posture weight to zero removes only the first.

I keep the reach direction from the demonstration and re-set the reach magnitude to a range the robot serves well. This removed joint-limit contact on the operations with sustained forward reach, without any change to the solver. I verified the result over five motion classes, a reach-extent sweep and two demonstrators, then replayed the trajectories on hardware.

**Manuscript:** **Minjun Chang**, Francis Baek, "Keep the Direction, Reset the Reach: Task-Defined Retargeting for Construction and Manufacturing Humanoids," in preparation.

Ongoing work on acquiring these motions from video is on the [Worker Motion Transfer from Video](/portfolio/motion-from-video/) page.
