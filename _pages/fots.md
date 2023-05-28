---
layout: default
title: "FOTS: A Fast Optical Tactile Simulator for Sim2Real Learning of Tactile-guided Robot Manipulation Skills"
permalink: /fots/
author_profile: false
---

## [code](https://github.com/Rancho-zhao/FOTS)&nbsp;&nbsp;&nbsp;&nbsp;[paper](https://github.com/Rancho-zhao/FOTS)

## Abstract

Simulation is a commonly-used tool in robotics to reduce hardware consumption and gather large-scale data. Despite the efforts of several works to simulate optical tactile sensors, there remains challenges in synthesizing images efficiently and mimicking marker motion under different contact loads. In this work, we propose a fast optical tactile simulator, named FOTS, for simulating optical tactile sensors. We utilize a multi-layer perceptron mapping and planar shadow generation to simulate the optical response, and marker distribution approximation to simulate the motion of surface markers caused by the surface stretch of the elastomer. Meanwhile, a Sim2Real transferable tactilemotor policy learning method is proposed, which integrates the proposed FOTS with physical engines such as MuJoCo. Experiment results reveal that FOTS outperforms other methods in terms of image generation quality and rendering speed, achieving 28.6 fps for optical simulation and 326.1 fps for marker motion simulation. In addition, the proposed method is applied to three tactile-guided robot manipulation tasks: cable-following, peg-in-hole, and door-opening. The experiments demonstrate the effectiveness of our method in zero-shot Sim2Real learning of tactile-guided robot manipulation skills.

<div align=center>
<img src="/images/fots/optical_quality.jpg" width="75%" height="75%">
</div>

<center style="font-size:14px;color:#C0C0C0;text-decoration:underline">Figure 1: The comparison of optical simulation among our method, TACTO, Phong, and Taxim with the real data.</center>

&nbsp;

<div align=center>
<img src="/images/fots/marker_quality.jpg" width="75%" height="75%">
</div>

<center style="font-size:14px;color:#C0C0C0;text-decoration:underline">Figure 2: Marker motion field simulation results. We visualize the marker motions (scaled up by 5 for better visualization) on the objects under different normal, shear, and twist displacements.</center>

&nbsp;

<div align=center>
<img src="/images/fots/snapshot.jpg" width="50%" height="50%">
</div>

<center style="font-size:14px;color:#C0C0C0;text-decoration:underline">Figure 3: Tactile-guided robot manipulation in real-world scenarios. The first row is the tactile-images-guided Cable-Following task. The middle row and the last row are the tacile-flow-guided Peg-in-hole task and Door-Opening task, respectively.</center>