---
title: Prior scene context reshapes feature reliance during rapid perception
title_zh: 先验场景上下文重塑了快速感知过程中的特征依赖
authors: "Tasliyurt-Celebi, S., de Haas, B., L.-H. Vo, M., Dobs, K."
date: 2026-05-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.10.724088v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 结合眼动追踪与编码模型预测检测延迟
tldr: 本研究探讨了先验场景背景如何影响快速视觉处理。通过眼动追踪和特征编码模型，研究者在自然场景的人脸检测任务中发现，先验背景能显著缩短检测延迟，且这种促进作用在首次眼动中即有体现。模型分析显示，背景信息增加了对空间先验的依赖，同时减少了对感官驱动特征的依赖，揭示了先验知识在重塑感知策略中的关键作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究先验场景背景信息如何影响人类在快速视觉感知过程中对感官输入与预期信息的权衡。
method: 结合眼动追踪技术与特征编码模型，通过操纵无脸场景预览和外周视觉限制，分析自然场景中人脸检测的反应延迟。
result: 先验背景显著提升了检测效率，并使处理过程从依赖深度神经网络提取的感官特征转向依赖场景衍生的空间先验。
conclusion: 研究表明先验场景背景通过将信息处理重心从感官驱动转向预期引导的空间导航，从而重塑了快速感知的特征依赖。
---

## 摘要
人类的感知受感官输入和先验知识或预期的共同塑造。但先验上下文信息如何影响快速视觉处理？本研究通过两项实验（每项实验 N = 38），结合眼动追踪与基于特征的编码模型，预测了一项核心视觉任务中的检测延迟：自然场景中的快速人脸检测。在第一个实验中，我们操纵了无脸场景预览的出现。在第二个实验中，我们还利用移动窗口范式限制了外周视觉输入，从而增加了对先验信息的依赖。在两项实验中，先验上下文都促进了人脸检测，特别是对于具有挑战性的图像。这种促进作用在第一次眼动中就已经显现，表明预览从一开始就塑造了感知策略。为了量化引导行为的信息，我们使用一组基于图像的预测因子对检测延迟进行了建模，这些预测因子捕捉了 (i) 感官信息和 (ii) 场景衍生的空间先验：预期的人脸位置。两类预测因子都解释了图像间延迟的变化。在感官预测因子中，由人脸出现引起的深度神经网络响应差异提供了最强的检测延迟样本外预测。关键的是，当场景预览可用时，空间先验的贡献增加，而对感官驱动特征的依赖通常会减少。总之，这些发现表明，先验场景上下文将用于快速人脸检测的信息平衡从感官驱动转向了基于预期的空间引导。

## Abstract
Human perception is shaped by both sensory input and prior knowledge or expectations. But how does prior contextual information influence rapid visual processing? Here, we combined eye tracking with feature-based encoding models across two experiments to predict detection latencies in a core visual task: rapid face detection in natural scenes (N = 38 per experiment). In the first experiment, we manipulated the presence of faceless scene previews. In the second experiment, we additionally restricted peripheral visual input using a moving-window paradigm, thereby increasing reliance on prior information. Across both experiments, prior context facilitated face detection, particularly for challenging images. This facilitation was already evident in the very first eye movement, suggesting that previews shape perceptual strategies from the outset. To quantify what information guided behavior, we modeled detection latencies using a set of image-based predictors capturing (i) sensory information and (ii) a scene-derived spatial prior: the expected face location. Both predictor classes explained latency variation across images. Among sensory predictors, the difference in deep neural network responses induced by the presence of the face provided the strongest out-of-sample prediction of detection latency. Critically, when scene previews were available, the contribution of the spatial prior increased, while reliance on sensory-driven features was generally reduced. Together, these findings indicate that prior scene context shifts the balance of information used for rapid face detection from sensory-driven to expectation-based spatial guidance.