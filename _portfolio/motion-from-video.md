---
title: "Worker Motion Transfer from Video"
excerpt: "<img src='/images/learn_from_vid.gif' width='300'>"
collection: portfolio
---

I am building a pipeline that turns ordinary video of a worker into motion a humanoid can be trained on. The aim is a reusable library of construction operations collected without motion capture equipment on site.

![Learning from video](/images/learn_from_vid.gif){: width="450" .align-center}

The pipeline reconstructs human pose from a single video, segments it into motion classes, retargets it onto the humanoid and trains a tracking policy by reinforcement learning in IsaacLab. Tool and material interaction is carried through as object state, so operations that involve picking something up are handled rather than dropped.

I am responsible for:
- **Human pose reconstruction and retargeting** across three isolated environments.
- **Forward kinematics and resampling** to produce the per-link states and velocities the trainer needs.
- **Object annotation and asset authoring** for tools that are not in the framework registry.
- **Teacher and student policy training** with and without object interaction.

Segmented motion classification is what this line of work adds. Field video is continuous activity rather than isolated demonstrations, so the useful unit is the recognized operation and not the clip. Classification and jobsite-scale collection are the current direction.

This is separate from my retargeting studies, which ask what a demonstration should carry onto the robot. That work is on the [Humanoid Motion Retargeting](/portfolio/humanoid-retargeting/) page.
