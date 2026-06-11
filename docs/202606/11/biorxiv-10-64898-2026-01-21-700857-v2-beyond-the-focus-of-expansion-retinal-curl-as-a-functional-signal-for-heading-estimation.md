---
title: "Beyond the Focus of Expansion: Retinal curl as a functional signal for heading estimation."
title_zh: 超越扩张焦点：视网膜旋度作为朝向估计的功能信号
authors: "Zorpala, K. I., Lopez-Moliner, J."
date: 2026-06-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.21.700857v2.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 利用眼动注视和视网膜卷曲建模人类朝向估计
tldr: 传统的航向估计模型普遍假设需要从光流场中精确恢复膨胀焦点（FoE）并补偿眼球运动带来的旋转分量，这一过程计算复杂且易受噪声干扰。本文提出一种替代假说：视觉系统直接利用注视点周围视网膜区域的平均卷曲（curl）作为航向的代理信号，而无需显式提取FoE。通过实时操纵注视点的中央凹卷曲成分，实验发现当卷曲被取消时偏差消失，过度取消时偏差反转，证明卷曲是感知偏差的具体驱动因素。一个结合注视依赖性抑制和正前方先验的环吸引子网络模型成功模拟了行为结果。这一发现表明大脑将注视稳定产生的规律性视网膜卷曲视为有用的导航信号，而非需要滤除的噪声。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统航向估计依赖FoE和旋转补偿，计算复杂，本文探索视网膜卷曲作为更简单的替代信号。
method: 通过实时操控注视点中央凹卷曲成分，保持平移流不变，测量参与者感知航向偏差。
result: 自然条件下偏差与注视方向相反；取消卷曲偏差消失，过度取消时反转，证实卷曲驱动偏差。
conclusion: 大脑利用注视稳定产生的视网膜卷曲作为功能信号简化导航，而非噪声。
---

## 摘要
旨在解释朝向的主流模型假设人类需要恢复扩张焦点（FoE），同时考虑眼动引起的旋转。我们提出另一种观点：视觉系统利用注视产生的平均视网膜旋度作为朝向的替代信号，从而无需显式恢复FoE。静止的受试者观看大屏幕上模拟的行走路径，同时注视投影地面纹理上不同偏心率的点——这是一种自然行为，产生持续的视网膜旋度。受试者连续报告在3D场景坐标中感知到的朝向。为了分离视网膜旋度的作用，我们采用实时操作，保持平移流恒定，同时使中央凹旋度分量保持不变、取消或过度取消。在自然条件（未改变）下，受试者表现出与注视方向相反的系统性朝向偏差。关键的是，当我们取消预期的旋度时，这些偏差消失，当我们过度取消时则反转，从而识别出视网膜旋度是感知偏差的具体驱动因素。我们使用一个简单的反馈控制器和一个具有注视依赖性抑制和直行先验的环吸引子神经网络对这些结果进行建模。这些发现表明，大脑利用注视稳定的几何结构来简化导航，将视网膜旋度视为功能性信号而非需要过滤的噪声。

## Abstract
Prevailing models aiming at explaining heading assume that humans need to recover the Focus of Expansion (FoE) while accounting for eye-movement-induced rotation. We propose an alternative: the visual system utilizes mean retinal curl from fixations as a surrogate signal for heading, rendering the explicit recovery of the FoE unnecessary. Stationary participants viewed simulated walking paths on a large screen while fixating on points on the projected ground texture at varying eccentricities --a natural behavior inducing sustained retinal curl. Participants continuously reported perceived heading in 3D scene coordinates. To isolate the role of retinal curl, we employed a real-time manipulation that kept translational flow constant while the foveal curl component was either unaltered, cancelled, or overcancelled. Under natural conditions (unaltered), participants exhibited systematic heading biases opposite the direction of gaze. Crucially, these biases vanished when we cancelled the expected curl, and flipped when we overcancelled it, identifying retinal curl as the specific driver of perceptual bias. We modeled these results using a simple feedback controller and a ring-attractor neural network featuring gaze-contingent inhibition and a  straight-ahead prior. These findings suggest the brain exploits the geometry of gaze stabilization to simplify navigation, treating retinal curl as a functional signal rather than noise to be filtered.