---
title: Changes in perceptual sampling contribute to representational drift
title_zh: 感知采样的变化导致表征漂移
authors: "Yuan, Y., Aoi, M. C., Serences, J."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.734121v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 眼动追踪实验分析注视模式
tldr: 表征漂移通常归因于内在神经动力学，但本研究提出行为变化（如注视）可能也是原因之一。通过纵向眼动实验，发现14名被试的自由观看注视模式随时间系统性漂移，且漂移方向一致。利用CORnet-S模型模拟，发现由注视差异引起的表征距离随实验间隔增加而增大，支持行为采样变化足以驱动视觉皮层表征漂移。该发现表明，即使简单任务中行为也会发生细微变化，这可能是表征漂移的普遍来源。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究系统性行为变化（如注视）是否是表征漂移的补充原因。
method: 纵向眼动实验（14人，6次）计算注视密度图Wasserstein距离，并用CORnet-S模型分析表征距离。
result: 注视模式随时间方向性漂移，模型表征距离随实验间隔增大。
conclusion: 行为采样变化足以引起视觉皮层表征漂移，无需内在神经重配置。
---

## 摘要
随着时间的推移，对同一刺激的神经反应模式逐渐发生变化，这种现象被称为表征漂移，已在多个皮层区域广泛观察到。漂移通常归因于由突触可塑性或更新驱动的内在神经动力学。在这里，我们测试了一个补充假设：漂移是由于行为中的系统性变化（如注意力或注视转移）而产生的。我们进行了一项纵向眼动追踪实验，14名成年人在跨越2-4周的6个实验阶段中自由观看自然图像，部分图像在阶段内和阶段间重复出现。对于每位参与者，我们使用Wasserstein距离量化了阶段对之间注视密度图的相似性。随着阶段间时间间隔的增加，注视模式变得越来越不相似，表明注视行为存在系统性和方向性的漂移。为了评估这些行为变化是否可能合理地引起神经表征的变化，我们将注视遮蔽的图像通过CORnet-S，这是一个灵长类动物腹侧视觉流的分层深度神经网络模型。表征距离（以配对激活差异的Frobenius范数量化）随着分离注视图的阶段数在所有四个模型层（V1、V2、V4、IT）中增加。基于核的最大均值差异检验进一步证实，表征距离的经验分布与随机打乱的对照显著不同。这些发现表明，随着时间的推移，视觉场景采样的微小但系统性的变化足以引起视觉皮层中的表征漂移。更一般地，这些结果表明，即使在简单任务中，行为随时间发生的细微变化也是不可避免的，而且这些变化可能足以在没有内在神经代码重构的情况下驱动表征漂移。

## Abstract
Gradual changes in neural response patterns to the same stimulus over time, termed representational drift, have been widely observed across cortical areas. Drift is typically attributed to intrinsic neural dynamics driven by synaptic plasticity or turnover. Here we test a complementary hypothesis that drift arises due to systematic changes in behavior such as shifts in attention or gaze. We conducted a longitudinal eye-tracking experiment in which fourteen adults freely viewed naturalistic images across 6 experimental sessions spanning 2-4 weeks, with a subset of images repeated within and across sessions. For each participant, we quantified the similarity of fixation density maps between session pairs using the Wasserstein distance. Fixation patterns became increasingly dissimilar with greater temporal separation between sessions, indicating systematic and directional drift in gaze behavior. To assess whether these behavioral changes could plausibly induce changes in neural representations, we passed fixation-masked images through CORnet-S, a hierarchical deep neural network model of the primate ventral visual stream. Representational distances, quantified as the Frobenius norm of pairwise activation differences, increased with the number of sessions that separated the fixation maps across all four model layers (V1, V2, V4, IT). A kernel-based maximum mean discrepancy test further confirmed that the empirical distribution of representational distances differed significantly from shuffled controls. These findings suggest that small but systematic shifts in the sampling of a visual scene over time are sufficient to cause representational drift in visual cortex. More generally, these results suggest that subtle changes in behavior over time are inevitable, even in simple tasks, and that these changes may be sufficient to drive representational drift in the absence of intrinsic reconfigurations of neural codes.