---
title: Inverse reinforcement learning reveals action-oriented value signals in naturalistic decision making
title_zh: 逆强化学习揭示自然主义决策中的行动导向价值信号
authors: "Lee, S. H., Chung, C., Oh, M.-h., Ahn, W.-Y."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.733779v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 使用逆强化学习从实时行为推断潜在评估状态
tldr: 自然决策中价值计算面临挑战，标准模型难以适用。逆强化学习（IRL）可从实时行为推断潜在奖励轨迹，但其神经基础未知。本研究通过fMRI驾驶任务发现，IRL奖励轨迹与背侧纹状体等价值相关脑区活动显著关联，并涉及认知控制与感觉运动区域。这表明IRL奖励提供了行动导向估值的动态神经代理。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究逆强化学习（IRL）能否从自然决策行为中提取具有神经相关性的价值信号。
method: 在fMRI扫描下执行真实驾驶任务，应用IRL推断时刻奖励轨迹，并与全脑活动进行回归分析。
result: IRL奖励轨迹与背侧纹状体、前扣带回及感觉运动皮层等区域的活动显著相关。
conclusion: IRL奖励可作为自然决策中行动导向估值的神经代理，桥接行为与价值计算。
---

## 摘要
认知神经科学的一个主要挑战是解释复杂自然环境中目标导向行为的价值是如何计算的。标准的决策计算模型在受控的、基于试验的范式中非常成功，但通常不适用于自然范式中实时展开的行为。逆强化学习提供了一种从自然环境中观察到的行为推断潜在评估状态的方法，但其神经可解释性在很大程度上仍未知。在这里，我们研究了在fMRI扫描期间进行实时驾驶任务时，从IRL导出的逐时刻奖励轨迹是否映射到大脑中的价值信号。IRL导出的奖励轨迹与背侧纹状体（一个通常与价值导向行动选择相关的区域）的活动关联最为显著。它们还与支持额外过程（包括认知控制和感觉运动处理）的分布区域显示出关联。这种模式表明，IRL奖励捕获了以奖励回路为中心的分布式神经活动，可能反映了价值评估如何与其他过程相互作用。总之，这些发现表明，在自然主义决策中，IRL奖励为行动导向的评估提供了一个行为上基于、时间上可分辨的代理指标。

## Abstract
A major challenge for cognitive neuroscience is to explain how value of a goal-directed behavior is computed in complex and naturalistic environments. Standard computational models of decision making have been highly successful in controlled, trial-based paradigms, but they are often ill-suited to real-time behavior unfolding in naturalistic paradigms. Inverse reinforcement learning (IRL) offers a way to infer latent evaluative state from observed behavior in naturalistic environments, but its neural interpretability remains largely unknown. Here, we investigated whether moment-to-moment reward trajectories derived from IRL map onto value signals in the brain during a real-time driving task performed during fMRI scanning. IRL-derived reward trajectories were most robustly associated with activity in the dorsal striatum, a region often linked to value-guided action selection. They also showed associations with distributed regions supporting additional processes, including cognitive control and sensorimotor processing. This pattern suggests that IRL reward captures distributed neural activity centered on the reward circuitry, potentially reflecting how valuation interacts with other processes. Together, these findings suggest that IRL reward provides a behaviorally grounded, temporally resolved proxy for action-oriented valuation during naturalistic decision making.