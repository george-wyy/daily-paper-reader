---
title: The Computational and Neural Basis of Zero-Shot Control in Dynamic Pursuit
title_zh: 动态追逐中零样本控制的计算与神经基础
authors: "Kim, D., Lee, J. J., Hayden, B. Y., Yoo, S. B. M."
date: 2026-05-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.30.715455v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 动态追踪中灵活控制和聚光灯注意力的计算基元
tldr: 本研究探讨了生物体在无需额外训练的情况下灵活适应新目标的计算原理。研究者提出了关系结构、聚光灯注意力和可供性计算三个核心认知构件，并基于多模块图卷积网络构建了模型。该模型在动态追踪任务中实现了跨物理环境、目标属性和交互策略的零样本迁移，并展现了生物特有的“改变主意”行为。灵长类动物大脑前扣带回皮层的神经记录进一步验证了该计算架构的生物合理性。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在揭示生物智能如何在无需额外训练的情况下，灵活适应新目标和环境需求的底层计算与神经机制。
method: 提出由关系结构、聚光灯注意力和可供性计算组成的计算基元，并利用多模块图卷积网络在动态追踪任务中进行实现。
result: 模型实现了在多种新颖追踪场景下的零样本迁移，并自发产生了类似生物的“改变主意”决策行为，且得到了灵长类神经数据的支持。
conclusion: 关系结构、注意力和可供性计算是实现灵活控制的关键计算基元，为理解生物和人工智能的零样本控制提供了统一框架。
---

## 摘要
生物智能体能够灵活地调整其行为以适应新的目标和环境需求，而无需额外的训练，但实现这种控制的计算原理仍不清楚。在此，我们提出三个认知构件构成了这种灵活控制的最小计算基元：关系结构、聚光灯注意力和可负担性计算。我们研究了这些构件是否在具身动态追逐任务中支撑了灵活控制，该任务需要持续整合实体间关系、奖励和动作可行性，使其成为实时控制的理想试验场。通过在多模块图卷积网络中实现这些构件，我们展示了该模型在物理特性、目标属性和交互策略（如逃跑或追逐）各异的新型追逐场景中实现了零样本迁移，且无需额外训练。尽管没有经过显式训练，该模型还表现出“改变主意”（CoM）行为，即中途修正目标，这是生物智能体所表现出的灵活控制的一个标志。来自灵长类动物背侧前扣带回皮层的神经记录揭示了将这些构件与神经动力学联系起来的群体水平特征，为所提出的计算架构提供了生物学支持。

## Abstract
Biological agents flexibly adapt their behavior to novel goals and environmental demands without additional training, yet the computational principles enabling such control remain unclear. Here, we propose that three cognitive constructs constitute minimal computational motifs for such flexible control: relational structure, spotlight attention, and affordance computation. We examine whether these constructs underpin flexible control in an embodied dynamic pursuit task that requires continuous integration of inter-entity relations, reward, and action feasibility, making it a suitable testbed for real-time control. By implementing these constructs within a multi-module graph convolutional network, we show that the model achieves zero-shot transfer across novel pursuit scenarios that vary in physics, target properties, and interaction policies such as fleeing or chasing, without additional training. Although not explicitly trained to do so, the model also exhibits change-of-mind (CoM) behavior, or mid-course target revision, a hallmark of flexible control exhibited by biological agents. Neural recordings from the primate dorsal anterior cingulate cortex revealed population-level signatures that link these constructs to neural dynamics, providing biological support for the proposed computational architecture.