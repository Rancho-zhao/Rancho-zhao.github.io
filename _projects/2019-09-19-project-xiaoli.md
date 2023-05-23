---
title: "Xiaoli: A Robotic Arm for Table Tennis Grasping"
collection: projects
type: "Projects"
permalink: /projects/2019-09-19-project-xiaoli
date: 2019-09-19
---

Xiaoli has three functions including *remote control movement*, *robotic arm control* and *autonomous grasping*.

![fig1](/images/project-xiaoli/overall.jpg "xiaoli")

## Hardware

|Modules|Information|
| ----- |-----------|
|Controller| STM32 |
|Sensor| ov2640 |
|HRI interface| PS2 handle, Wireless transceiver |
| Power source| 4S battery, Voltage Control System|
|Actuator| DC motor, 3-joints robotic arm|

The following figure shows the relationship between modules. Yellow represents power module, black represents actuator module, and red represents core circuit.

![fig2](/images/project-xiaoli/hardware.jpg "hardware")

## Sofeware

|Iterms|Information|
|------|-----------|
|Debugging tools | PC, Oscilloscope, Function generator|
|Platforms|WIN10, KEIL, Arduino, Spyder|

### remote control movement

This function involves data collection and analysis of handle input (digital quantity), calculation of robot angular and linear velocities, and motor output.

|Items|Information|
|-----|-----------|
|Handle rocker digital quantity|$X=-128-127$, $Y=-128-127$|
|Output speed|$w=X(angular velocity)$, $v=Y(linear velocity)$|
|Motor output|$Motor1 PWM=v-w$, $Motor2 PWM=v+w$|

![fig3](/images/project-xiaoli/movement.jpg "movement")

### robotic arm control

Using a robotic arm with 3 joints that are in the same plane, but the pan tilt can rotate. Model the robot as following:

![fig4](/images/project-xiaoli/control.jpg "control")

Three joints are simplified as spherical coordinate system vectors of $R0$, $R1$, and $R2$ in space. The joint points are simplified as $J0$, $J1$, and $J2$, as well. The coordinate origin is the joint point where the base of the robotic arm is located.

![fig5](/images/project-xiaoli/control-1.jpg "control-1")

### autonomous grasping

The recognized object is a table tennis ball, and the recognition results are the position and size of the table tennis ball in the field of view (considered as distance).

![fig6](/images/project-xiaoli/auto-1.jpg "auto-1")

The key parameters and results are as follows:

|Items|Information|
|-----|-----------|
|Image size|$160\times 120$|
|Threshold in H channel|$10-60$|
|Filtering method|convolution($9\times 9$)|
|fps|$6.6$|