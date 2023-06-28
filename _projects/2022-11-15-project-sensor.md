---
title: "Reproducation and Improvement of Vision-based Tactile Sensors"
collection: projects
type: "Projects"
permalink: /projects/2022-11-15-project-sensor
date: 2022-11-15
---

I reproduce and improve the design of GelSight-like tactile sensors, including GelSight and DIGIT.

## 0. Preparation of Hardware Materials

|Type| Item|
|:---:|:---:|
|**General equipment**|Voltage-stabilized source; Air brush; Oven; Electric soldering iron|
|**Materials for GelSight**|TPU; TPU coating glue; Metallic paint; Tin powder (high purity);<br> Acrylic board (3cmx3cm); LED lamp belt (red, green, blue, white);<br> Fisheye camera; Shell (3D printed)|
|**Materials for DIGIT**|Fully transparent silicone; Silicone glue; Acrylic board (6mm); <br>Shell (3D printed); Marker paper (water printed)|


## 1. GelSight

<img src="{{ site.url }}/images/project-sensor/gelsight_soildworks.gif">

### 1.1 Fisheye camera calibration

Using a 7 * 7 chessboard grid (with a single edge length of 6mm), the original image and the distorted image are as follows:

<img src="{{ site.url }}/images/project-sensor/fisheye_2.jpg" width="50%" height="50%" align=center>

<img src="{{ site.url }}/images/project-sensor/fisheye_3.jpg" width="50%" height="50%" align=center>

The calibration method refers to [gelsight](https://github.com/wrslab/gelsight)

### 1.2 Reflection membrane production

For gel elsotmer, the 7cm * 7cm shockproof pad (made of TPU) sold online is used. According to the actual demand, it needs to be cut to about 2.5cm * 2.5cm.

For the production of reflection membrane, a relatively good process has been found as follows:

1. Cover one side of the silicone with tin powder (because the silicone itself is sticky, simply put the silicone in the tin powder; also, the tin powder must be relatively fine and not have a grainy texture);
2. Spray with metallic paint (be careful not to apply too much);
3. After the paint is roughly dried, cover the surface with TPU coating glue (which can protect the reflection membrane and improve its durability);
4. Continue drying.

**Attention! Protect the edges and sides of TPU throughout the entire process**

### 1.3 Finished product display

<img src="{{ site.url }}/images/project-sensor/gelsight_0.jpg" width="50%" height="50%" align=center>

- Depth reconstruction

<img src="{{ site.url }}/images/project-sensor/circle.png" width="50%" height="50%" align=center>

<img src="{{ site.url }}/images/project-sensor/moon.png" width="50%" height="50%" align=center>

- Equipped to robot arm

<img src="{{ site.url }}/images/project-sensor/robot_arm.jpg" width="50%" height="50%" align=center>

## 2. DIGIT

### 2.1 Production of gel elastomer and reflection membrane

1. 3D printed the gel mold of DIGIT, using food grade fully transparent liquid silicone with a shore hardness of 5 degrees, mixed with silicone A & B adhesive in a 1:1 ratio, heated in an oven at 90 ° C for 10 minutes;

<img src="{{ site.url }}/images/project-sensor/3dprint.jpg" width="50%" height="50%" align=center>

2. Dilute the hand feeling oil (hand feeling oil: curing agent: diluent=100:3:400) and evenly spray it on the surface of silicone to create a matte effect. First, let it stand at room temperature for 5-10 minutes, then heat it in an oven at 180-200 ° C for 15-20 minutes;
3. Dilute white silicone ink (ink: curing agent: diluent=100:3:500) and spray evenly on the surface of the hand felt oil using a air brush;
4. Use 6mm thick transparent acrylic board as the support of gel elastomer;
5. Use silicone glue to bond the acrylic board with the gel.

### 2.2 Production of markers

Using watermark techniques (similar to water soaked tattoo stickers)

The pattern of the marker is shown in the following figure:

<img src="{{ site.url }}/images/project-sensor/marker.png" width="25%" height="25%">

### 2.3 Finished product display

<img align="middle" src="{{ site.url }}/images/project-sensor/digit_video.gif">