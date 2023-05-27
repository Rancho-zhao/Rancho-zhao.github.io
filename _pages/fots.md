---
layout: archive
title: "FOTS: A Fast Optical Tactile Simulator for Sim2Real Learning of Tactile-guided Robot Manipulation Skills"
permalink: /fots/
author_profile: false
---

## [code](https://github.com/Rancho-zhao/FOTS)            [paper](https://github.com/Rancho-zhao/FOTS)

## Abstract

Simulation is a commonly-used tool in robotics to reduce hardware consumption and gather large-scale data. Despite the efforts of several works to simulate optical tactile sen-sors, there remains challenges in synthesizing images effi-ciently and mimicking marker motion under different con-tact loads. In this work, we propose a fast optical tactile simulator, named FOTS, for simulating optical tactile sen-sors. We utilize a multi-layer perceptron mapping and pla-nar shadow generation to simulate the optical response, and marker distribution approximation to simulate the motion of surface markers caused by the surface stretch of the elas-tomer. Meanwhile, a Sim2Real transferable tactilemotor policy learning method is proposed, which integrates the proposed FOTS with physical engines such as MuJoCo. Experiment results reveal that FOTS outperforms other methods in terms of image generation quality and rendering speed, achieving 28.6 fps for optical simulation and 326.1 fps for marker motion simulation. In addition, the proposed method is applied to three tactile-guided robot manipula-tion tasks: cable-following, peg-in-hole, and door-opening. The experiments demonstrate the effectiveness of our method in zero-shot Sim2Real learning of tactile-guided robot manipulation skills.

![fig1](/images/fots/optical_quality.jpg "fig1")