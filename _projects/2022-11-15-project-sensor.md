---
title: "Reproducation and Improvement of Vision-based Tactile Sensors"
collection: projects
type: "Projects"
permalink: /projects/2022-11-15-project-sensor
date: 2022-11-15
---

我复现和改进了GelSight-like的触觉传感器，包括Gelsight和DIGIT。

## 硬件材料准备

- 通用设备
稳压电源 1个
喷枪	1把
烤箱    1个
电烙铁  1个

- GelSight
弹性体凝胶（elastomer gel）	1袋/1卷
涂层凝胶（coating gel）	1瓶
锡粉	1袋
LED灯带 red, green, blue, white
鱼眼摄像头	1个
3D打印	外壳+内壳各1个


- DIGIT
全透明硅胶（A/B） 各1瓶
硅胶胶水    1条
6mm亚克力板 1个
3D打印外壳 1个
纹身贴  1张

## GelSight

<img src="{{ site.url }}/images/project-sensor/gelsight_soildworks.gif">

### 鱼眼相机标定

使用7*7棋盘格（单格边长6mm），采集了四十张各个角度的图片如下：

### 反射层制作

对于凝胶，使用的是网上卖的7cm*7cm的防震垫，根据实际需求，需要将其裁剪成大概2.5cm*2.5cm

硅胶还是采用网上购买的防震垫

对于反射层的制作，目前发现的比较不错的流程如下：

1. 将硅胶一面用锡粉覆盖（因为硅胶本身有粘性，所以直接把硅胶放在锡粉里就行；还有就是锡粉一定要比较细，不要有颗粒感）
2. 用金属漆喷涂（注意不要涂太多）
3. 等喷漆大致晾干之后，用涂层胶水覆盖表面（可以保护反射层，提高反射层的耐用性）
4. 继续晾干

**注意！全程保护硅胶的边缘侧面**

## DIGIT

### 硅胶模制作

1. 3D打印Digit硅胶模具，使用邵氏硬度为5度的食品级全透明液态硅胶，硅胶AB胶1:1混合，烤箱90°加热10min
2. 稀释手感油（手感油：固化剂：稀释剂=100：3：400），均匀喷涂在硅胶表面，制造哑光效果，先常温静置5-10min，然后烤箱180-200°加热15-20min
3. 稀释白色硅胶油墨（油墨：固化剂：稀释剂=100：3：500），使用喷枪均匀喷涂在手感油表面之上
4. 定制了6mm和5mm的透明亚克力板作为硅胶支撑
5. 使用硅胶胶水将亚克力板和硅胶进行粘合

### 锚点制作

使用水印手艺（纹身贴制作）