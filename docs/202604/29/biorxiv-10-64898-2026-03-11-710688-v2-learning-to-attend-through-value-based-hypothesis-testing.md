---
title: Learning to Attend Through Value-Based Hypothesis Testing
authors: "Maher, C., Saez, I., Radulescu, A."
date: 2026-04-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.11.710688v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 通过计算模型推断潜在注意力动态和假设驱动学习
tldr: 该研究利用循环神经网络推断隐性注意力状态，并区分不同的学习策略。
source: biorxiv
selection_source: fresh_fetch
motivation: 通过计算模型推断潜在注意力动态和假设驱动学习。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
In complex environments, humans must determine which features are relevant for learning and decision-making. Psychological theories offer competing accounts of this process: associative models suggest that attention emerges gradually through learned changes in feature values, whereas hypothesis-driven accounts propose that learners selectively attend to actively tested rules. Because attentional states are covert, similar behavior can arise from different underlying strategies, making these accounts difficult to distinguish using choice data alone. We inferred latent attention dynamics during learning and decision-making by training recurrent neural networks on synthetic data generated from feature-based reinforcement learning (FRL) and serial hypothesis testing (SHT) models. A network trained on hybrid (FRL+SHT) data outperformed single-model networks, decoding latent human attention with more than 80% accuracy. These results suggest that human attention reflects an interaction between value-based learning and hypothesis testing, in which learned feature value guides the generation and evaluation of candidate rules.