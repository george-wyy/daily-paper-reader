---
title: Intrinsic rewards guide visual resource allocation via reinforcement learning
title_zh: 内源性奖励通过强化学习引导视觉资源分配
authors: "Tomic, I., Raimundo, R., Bays, P. M."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.1101/2025.04.25.650663v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 内在奖励引导视觉资源分配和编码优先级
tldr: 本研究探讨了内在奖励（如胜任感）对视觉资源分配的影响。通过视觉估计实验操纵参与者的主观自信，发现观察者会优先处理低误差刺激，导致资源分配偏离最优策略并损害整体准确性。研究结合强化学习与神经资源分配模型，揭示了内在奖励塑造认知表现的计算机制，证明了动机偏差对资源分配的引导作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究内在奖励（如主观胜任感）如何影响人类视觉系统在处理不同刺激时的资源分配决策。
method: 通过视觉估计实验操纵反馈和刺激可靠性，并利用结合强化学习规则的归一化模型进行定量分析。
result: 观察者倾向于将资源分配给已表现良好的刺激，这种基于奖励的偏差导致其偏离了误差最小化的最优策略。
conclusion: 内在奖励信号通过强化学习机制引导资源分配，为理解认知表现中的动机偏差提供了计算基础。
---

## 摘要
人类和其他动物会优先处理预示奖励的视觉刺激。虽然先前的研究主要集中在有形激励（如金钱或食物）上，但内源性激励（如感知的胜任感）的影响尚不明确。通过一系列视觉估计实验，我们利用欺骗性的逐试次反馈或刺激可靠性的真实差异，操纵了观察者对其判断的主观自信感。我们发现，观察者会优先编码与较低不确定性或误差相关的刺激，这有利于那些已被准确估计的刺激的表现，但进一步损害了那些估计较差的刺激的表现。这些由奖励驱动的偏差虽然可能具有适应性，但由于导致资源分配偏离了误差最小化策略，从而损害了当前任务的整体准确性。为了解释这些发现，我们在神经资源分配的归一化模型中补充了一个简单的强化学习规则。内源性和外源性奖励累积地塑造了模型分配给不同刺激的价值，由此产生的差异使资源分配产生偏差，进而影响估计误差，在定量上与数据相匹配。这些发现揭示了内源性奖励信号如何以既具适应性又具反作用的方式塑造资源分配，为认知表现背后的动机偏差提供了计算基础。

## Abstract
Humans and other animals prioritise visual processing of stimuli that signal rewards. While prior research has focused on tangible incentives (e.g., money or food), the effects of intrinsic incentives -- such as perceived competence -- are less well understood. Across a series of visual estimation experiments, we manipulated observers' subjective sense of confidence in their judgements using either deceptive trial-by-trial feedback or real discrepancies in stimulus reliability. We found that observers prioritised encoding of stimuli associated with lower uncertainty or error, benefiting performance for stimuli already estimated accurately, while further impairing performance for those estimated poorly. These reward-driven biases, while potentially adaptive, impaired overall accuracy in the present tasks by causing resource allocation to deviate from the error-minimizing strategy. To account for these findings, we supplemented a normalization model of neural resource allocation with a simple reinforcement learning rule. Intrinsic and extrinsic rewards cumulatively shaped the values assigned to different stimuli by the model, and the resulting discrepancies biased resource allocation and thereby estimation error, quantitatively matching the data. These findings reveal how intrinsic reward signals can shape resource allocation in ways that are both adaptive and counterproductive, offering a computational basis for the motivational biases underlying cognitive performance.