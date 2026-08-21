---
title: Explainable Decoding of Sensorimotor Communication in Joint Object Manipulation
title_zh: 联合物体操作中感觉运动通信的可解释解码
authors: "Liu, Y., Verdel, D., Leib, R., Burdet, E., Franklin, D. W."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.17.745075v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 在协作操作中利用多模态感觉运动信号解码人类意图，可作为多模态意图预测的方法参考
tldr: 在不对称信息的联合物体操作中，人类通过运动学和触觉线索传递意图，且线索含义随情境变化。本文提出可解释的机器学习框架，从视觉-触觉多模态信号中解码操作意图，并量化不同特征的信息贡献。将解码信号整合进漂移扩散模型，能够准确预测不知情伙伴的目标选择与决策时间。该框架揭示了动作通信的内在机制，并为协作机器人通过物理交互推断和表达意图提供了设计原则。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究不对称信息下人类在联合操作中如何通过运动与触觉信号传递意图，以理解动作通信机制并为协作机器人提供参考。
method: 提出可解释机器学习框架，从视觉-触觉多模态信号中解码操作意图并量化特征信息量；将解码信号融入漂移扩散模型，建立决策预测。
result: 解码信号与漂移扩散模型结合，能准确预测不知情伙伴的目标选择与决策时间，验证了特征的可解释性。
conclusion: 揭示了人类通过动作传达意图的机制，为协作机器人推断和表达意图提供了基于物理交互的设计原则。
---

## 摘要
人类经常在信息不对称的情况下协作，例如当两个人抬一张桌子而只有一个人知道目的地时。他们不使用言语，而是通过运动学、交互力和物体状态的线索进行协调。刻画这种感觉运动通信是困难的，因为这些信号既执行任务又传递信息，其含义依赖于上下文。在这里，我们研究了一个虚拟抬桌任务，其中一方知道目标，而另一方从视觉-触觉反馈中推断目标。参与者灵活地调整跨情境的运动学和触觉线索以传达意图。我们引入了一个可解释的机器学习框架，从持续的多模态信号中解码意图，并量化各个特征在何处具有信息量。将解码信号纳入漂移扩散模型，可以准确预测信息缺失方的目标选择及决策时间。我们的框架共同解释了人类如何通过行动进行交流，并为协作机器人通过物理交互推断和表达意图提供了原则。

## Abstract
Humans often collaborate under asymmetric information, for example when two people carry a table and only one knows the destination. They coordinate without speech using cues from movement kinematics, interaction forces, and object states. Characterizing this sensorimotor communication is difficult because these signals both execute the task and convey information, whose meaning is context-dependent. Here, we investigated a virtual table-carrying task where one partner knew the target while the other inferred it from visuo-haptic feedback. Participants flexibly adapted kinematic and haptic cues across contexts to convey intention. We introduce an explainable machine-learning framework that decodes intent from ongoing multimodal signals and quantifies where individual features are informative. Incorporating the decoded signals into a drift-diffusion model accurately predicted the uninformed partner's target choices and decision times. Together, our framework explains how humans communicate through action and offers principles for collaborative robots to infer and express intent through physical interaction.