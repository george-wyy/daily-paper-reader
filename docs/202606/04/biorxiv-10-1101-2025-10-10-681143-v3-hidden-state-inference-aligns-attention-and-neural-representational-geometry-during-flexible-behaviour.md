---
title: Hidden-state inference aligns attention and neural representational geometry during flexible behaviour
title_zh: 隐藏状态推理在灵活行为中协调注意与神经表征几何结构
authors: "Kerren, C., Theves, S., Johansson, M., Gardenfors, P., Doeller, C. F."
date: 2026-06-04
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.10.681143v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 利用眼动行为作为注意力的代理，在隐状态推断任务中关联眼动与意图识别
tldr: 在不确定环境中灵活决策需要推断潜在任务状态并优先处理行为相关信息。本研究通过串行反转学习任务结合眼动追踪和脑磁图，发现隐状态推理模型优于强化学习模型解释人类行为。眼动注意力聚焦于相关特征并随信念更新动态调整；神经表征编码当前上下文，预测误差较大时上下文表征减弱。成功表现伴随神经几何重组织，放大任务相关表征距离。研究表明隐状态推理、注意力和神经表征几何紧密协调，为灵活决策的神经机制提供系统级解释。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究灵活决策中隐状态推理如何与注意力和神经表征结构变化相关联。
method: 结合串行反转学习任务、眼动追踪和脑磁图，比较隐状态推理与强化学习模型，分析注意力和神经表征。
result: 隐状态推理模型最佳预测行为；注意力聚焦相关特征；神经编码上下文并受预测误差调节；成功时表征几何选择性放大任务相关距离。
conclusion: 隐状态推理、注意力和神经表征几何在灵活决策中紧密协调，支持自适应行为。
---

## 摘要
在不确定环境中的灵活决策需要推断潜在的任务状态并优先处理行为相关信息。我们检验了该假说：这一过程与注意和神经表征结构的系统性变化有关。人类参与者执行一项序列反转学习任务，需识别当前相关的刺激维度。行为上，参与者迅速适应情境切换，隐藏状态推理模型最能解释这些适应行为，在预测选择和推断情境方面优于多个强化学习变体。眼动行为为选择性注意提供收敛证据，注视逐渐集中于相关特征，追踪逐试次的信念更新，并在高预测错误后短暂拓宽。在这些结果指导下，我们使用脑磁图检查潜在状态推理如何反映在神经活动中。神经表征编码当前推断的情境，并受近期预测错误调控，较大的预测错误与后续试次中较弱的情境表征相关。表征分析进一步揭示，成功表现与神经几何结构的系统性重组相关，其特征是任务相关表征距离的选择性放大以及行为相关刺激值的分离增强。总之，我们的发现表明在灵活决策过程中，潜在状态推理、注意和神经表征几何结构紧密协调，为行为相关信息如何被选择性优先化并表征以支持适应行为提供了系统层面的解释。

## Abstract
Flexible decision-making in uncertain environments requires inferring latent task states and prioritising behaviourally relevant information. We tested the hypothesis that this process is associated with systematic changes in attention and neural representational structure. Human participants performed a serial reversal learning task that required identifying which stimulus dimension(s) were currently relevant. Behaviourally, participants rapidly adapted to context switches, and a hidden-state inference model best explained these adaptations, outperforming multiple reinforcement-learning variants in predicting both choices and inferred contexts. Oculomotor behaviour provided converging evidence for selective attention, with gaze increasingly concentrated on relevant features, tracking trial-by-trial belief updates, and transiently broadening following high prediction errors. Guided by these results, we used magnetoencephalography to examine how latent-state inference was reflected in neural activity. Neural representations encoded the currently inferred context and were modulated by recent prediction errors, with larger prediction errors associated with weaker context representations on subsequent trials. Representational analyses further revealed that successful performance was associated with a systematic reorganisation of neural geometry, characterised by selective amplification of task-relevant representational distances and increased separation of behaviourally relevant stimulus values. Together, our findings demonstrate that latent-state inference, attention, and neural representational geometry are tightly coordinated during flexible decision-making, providing a systems-level account of how behaviourally relevant information is selectively prioritised and represented to support adaptive behaviour.