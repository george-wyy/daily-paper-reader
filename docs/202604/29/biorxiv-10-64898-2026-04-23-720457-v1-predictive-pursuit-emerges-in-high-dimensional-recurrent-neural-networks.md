---
title: Predictive pursuit emerges in high-dimensional recurrent neural networks
authors: "Redman, W. T., Dinc, F. D., Lin, X., Chan, M. G., Alexander, A. S."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.23.720457v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 神经网络中目标位置的预测性追踪和内部预测
tldr: 模拟循环神经网络如何生成内部预测以追踪移动物体。
source: biorxiv
selection_source: fresh_fetch
motivation: 神经网络中目标位置的预测性追踪和内部预测。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
Tracking dynamic moving objects in the external world is ethologically important for many organisms. Recent experiments have examined neural dynamics supporting such behaviors by employing visually-guided pursuit in freely moving rodents, yet computational principles underlying this cognitive process are not well understood. To address this, we developed a recurrent neural network model for examining the predictive behaviors and computations that emerge during pursuit. We demonstrate that the model generates internal predictions of the targets future locations, with anticipatory behaviors increasing with exposure to stereotyped trajectories of the target. These internal predictions can be used by the model to pursue a target in a complex environment, and the RNNs emergent strategy is aligned with behavior when tested in rodents. In investigating the computations that underlie the RNNs ability to perform predictive pursuit, we found units sensitive to the position of the target relative to the artificial agent, a representation analogous to egocentric target neurons observed in animals performing pursuit tasks. Ablating these units significantly reduced model performance, establishing a causal role of this functional response type in efficient pursuit. Given the complexity of the task and agent behavior, we hypothesized that RNN models may use high-dimensional neural codes to support predictive pursuit. To test this, we trained models of varying rank and found that anticipatory behavior emerged only when the rank was sufficiently high, despite strong pursuit performance in lower rank models. All RNNs encoded the egocentric location of the target, whereas allocentric self and target locations emerged only in high-dimensional networks. Overall, our results suggest that, unlike commonly studied vision, motor, or memory tasks, predictive pursuit emerges in high-dimensional networks with sufficient resources.