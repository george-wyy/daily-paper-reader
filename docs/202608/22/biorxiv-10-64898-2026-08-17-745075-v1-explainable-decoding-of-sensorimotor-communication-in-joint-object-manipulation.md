---
title: Explainable Decoding of Sensorimotor Communication in Joint Object Manipulation
title_zh: 联合物体操纵中感觉运动沟通的可解释解码
authors: "Liu, Y., Verdel, D., Leib, R., Burdet, E., Franklin, D. W."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.17.745075v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 从持续多模态行为信号中可解释地解码人类意图，可迁移到实时意图识别
tldr: 人类协作中常存在信息不对称，例如两人抬桌仅一人知道目的地，需通过动作线索进行无声协调。本文提出可解释机器学习框架，从运动学与触觉等多模态信号中解码意图，并量化各特征的信息贡献。将解码信号接入漂移扩散模型，能准确预测未被告知一方的目标选择与决策时间。该框架揭示了通过行动沟通的原理，为协作机器人推断和表达意图提供了设计指导。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1921, \"height\": 944, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1477, \"height\": 1217, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1827, \"height\": 1337, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1635, \"height\": 1852, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1496, \"height\": 1896, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1876, \"height\": 1873, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-17-745075-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1796, \"height\": 1393, \"label\": \"Figure\"}]"
motivation: 人类协作中存在信息不对称，需通过动作线索沟通，但这些信号既执行任务又传递信息，含义依赖上下文，难以表征。
method: 构建可解释机器学习框架，从运动学与触觉等多模态信号中解码意图，量化特征贡献，并融入漂移扩散模型预测决策。
result: 将解码信号融入漂移扩散模型后，能准确预测未被告知方的目标选择与决策时间，并量化出各特征的信息贡献。
conclusion: 揭示了人类通过行动沟通的机制，为协作机器人感知与表达意图提供了设计原则。
---

## 摘要
人类常在信息不对称的情况下协作，例如两人抬桌子时只有一人知道目的地。他们无需言语，通过运动学、交互力和物体状态的线索进行协调。描述这种感觉运动沟通颇具挑战，因为这些信号既执行任务又传递信息，且其意义取决于情境。在此，我们研究了一项虚拟抬桌任务，其中一方知道目标，另一方则从视觉-触觉反馈中推断目标。参与者灵活地跨情境调整运动学和触觉线索以传达意图。我们引入了一个可解释的机器学习框架，从持续的多模态信号中解码意图，并量化各个特征的信息量。将解码信号纳入漂移扩散模型，可准确预测未知信息一方的目标选择与决策时间。综上，我们的框架解释了人类如何通过行动进行沟通，并为协作机器人通过物理交互推断和表达意图提供了原则。

## Abstract
Humans often collaborate under asymmetric information, for example when two people carry a table and only one knows the destination. They coordinate without speech using cues from movement kinematics, interaction forces, and object states. Characterizing this sensorimotor communication is difficult because these signals both execute the task and convey information, whose meaning is context-dependent. Here, we investigated a virtual table-carrying task where one partner knew the target while the other inferred it from visuo-haptic feedback. Participants flexibly adapted kinematic and haptic cues across contexts to convey intention. We introduce an explainable machine-learning framework that decodes intent from ongoing multimodal signals and quantifies where individual features are informative. Incorporating the decoded signals into a drift-diffusion model accurately predicted the uninformed partner's target choices and decision times. Together, our framework explains how humans communicate through action and offers principles for collaborative robots to infer and express intent through physical interaction.