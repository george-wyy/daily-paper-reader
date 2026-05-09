---
title: Augmenting the Bayesian Brain with learned and reusable world-model components for flexible cognition
title_zh: 以学习且可重用的世界模型组件增强贝叶斯大脑，实现灵活认知
authors: "Findling, C., Lee, J. K., Bakermans, J. J. W., Pouget, A., Wyart, V."
date: 2026-05-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.06.722922v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 用于贝叶斯大脑和世界模型组件的模块化神经状态空间模型
tldr: 贝叶斯大脑假说认为认知依赖于内部生成模型，但现有模型受限于预设结构和高计算开销。本研究提出模块化神经状态空间模型，通过可学习的世界模型组件和摊销神经更新取代固定规则。该框架支持组件在不同任务间重组与复用，实现了零样本泛化。实验证实人类行为符合该模型预测，揭示了灵活认知的计算原理。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统贝叶斯大脑模型因依赖预设的特定任务结构和高复杂度的迭代推理，难以解释人类认知的灵活性和可扩展性。
method: 提出模块化神经状态空间模型，利用可学习的世界模型组件和摊销推理取代固定的生成结构与推理规则。
result: 该模型支持组件在相似动力学任务间的无缝重组与复用，实现了零样本泛化，并得到了人类行为实验的验证。
conclusion: 可学习且可复用的世界模型组件是实现灵活认知的关键计算原则，为扩展贝叶斯大脑框架提供了新路径。
---

## 摘要
贝叶斯大脑假设认为认知依赖于世界的内部生成模型，然而现有的实现仍受限于预先指定的、特定于任务的生成结构以及计算繁重的迭代推理方案。在此，我们引入模块化神经状态空间模型作为贝叶斯大脑的一种可扩展实现，用学习到的世界模型组件和摊销神经更新取代了固定的生成结构和预先指定的推理规则。该框架保留了通过隐藏原因解释观测结果的核心承诺，同时使推理变得可学习且可重用，而非预先指定且特定于任务。我们对这些模型的模块化实现使得学习到的组件能够在共享相似潜在动力学的、表面上不同的任务之间无缝重组和堆叠。这种计算重用支持零样本泛化，并预测了任务间推理参数的选择性相关性。我们在人类行为中证实了这些关键预测，将学习且可重用的世界模型组件确定为灵活认知的一种候选计算原理。

## Abstract
The Bayesian Brain hypothesis assumes that cognition relies on internal generative models of the world, yet existing implementations remain constrained by pre-specified, task-specific generative structures and computationally heavy iterative inference schemes. Here, we introduce modular neural state-space models as a scalable realization of the Bayesian Brain, replacing fixed generative structures and pre-specified inference rules with learned world-model components and amortized neural updates. This framework preserves the core commitment to explaining observations through hidden causes while making inference learned and reusable rather than pre-specified and task-specific. Our modular implementation of these models affords learned components to be seamlessly recombined and stacked across superficially different tasks that share similar latent dynamics. Such computational reuse supports zero-shot generalization and predicts selective correlations of inference parameters between tasks. We confirm these key predictions in human behavior, identifying learned and reusable world-model components as a candidate computational principle for flexible cognition.