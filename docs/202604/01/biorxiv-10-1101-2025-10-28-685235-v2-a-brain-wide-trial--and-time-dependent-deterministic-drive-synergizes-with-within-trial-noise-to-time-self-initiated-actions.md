---
title: "A brain-wide, trial- and time-dependent deterministic drive synergizes with within-trial noise to time self-initiated actions"
title_zh: 全脑范围、依赖于试次和时间的确定性驱动与试次内噪声协同作用，共同决定自发动作的时机
authors: "Elbaz, M. A., Butterer, K., Solla, S. A., Glaser, J. I., Miri, A."
date: 2026-03-29
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.28.685235v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 从神经模式预测动作发生的时机
tldr: 本研究探讨了小鼠在无外部提示下自主启动动作的神经机制。通过同步记录皮层、丘脑、苍白球和小脑等多个脑区的大规模神经元活动，研究者发现动作触发受全脑范围内的确定性驱动力影响，该驱动力的初始值和速率随试次变化。计算建模表明，这种跨试次的确定性驱动与试次内的随机噪声协同作用，共同决定了动作时机。这一发现挑战了传统的层级化决策模型，揭示了自主动作定时是一个全脑分布式的动态过程。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-001.webp\", \"caption\": \"\", \"page\": 4, \"index\": 1, \"width\": 1430, \"height\": 1247}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-002.webp\", \"caption\": \"\", \"page\": 7, \"index\": 2, \"width\": 1430, \"height\": 1522}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-003.webp\", \"caption\": \"\", \"page\": 9, \"index\": 3, \"width\": 2174, \"height\": 1419}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-004.webp\", \"caption\": \"\", \"page\": 11, \"index\": 4, \"width\": 1932, \"height\": 355}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-005.webp\", \"caption\": \"\", \"page\": 14, \"index\": 5, \"width\": 2056, \"height\": 1819}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-006.webp\", \"caption\": \"\", \"page\": 18, \"index\": 6, \"width\": 1188, \"height\": 2319}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-007.webp\", \"caption\": \"\", \"page\": 22, \"index\": 7, \"width\": 2056, \"height\": 2003}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-008.webp\", \"caption\": \"\", \"page\": 24, \"index\": 8, \"width\": 1858, \"height\": 1424}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-009.webp\", \"caption\": \"\", \"page\": 25, \"index\": 9, \"width\": 2335, \"height\": 3170}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-010.webp\", \"caption\": \"\", \"page\": 27, \"index\": 10, \"width\": 1005, \"height\": 447}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-011.webp\", \"caption\": \"\", \"page\": 28, \"index\": 11, \"width\": 2056, \"height\": 2336}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-28-685235-v2/fig-012.webp\", \"caption\": \"\", \"page\": 30, \"index\": 12, \"width\": 1529, \"height\": 2335}]"
motivation: 旨在厘清在缺乏外部线索时，大脑自主决定动作时机的神经机制是基于确定性驱动还是随机过程。
method: 同步记录小鼠多个脑区的神经元群体活动，并利用计算模型分析动作预测性及试次间与试次内的变异性。
result: 发现动作时间可提前数秒预测，且全脑范围内的确定性驱动力与试次内噪声协同决定了动作的发生。
conclusion: 自主动作的定时源于全脑分布式的决策过程，而非单一的层级化模块控制。
---

## 摘要
在缺乏外部线索的情况下决定何时行动，对于探索、学习和生存至关重要。然而，此类决策背后的神经机制仍存在争议，目前的观点倾向于确定性或随机性基础。我们在小鼠自发进行自愿动作时，同时记录了皮层、丘脑、苍白球和小脑区域的大规模神经元群体。动作开始的时间可以提前数秒根据放电模式进行预测，且各区域间的预测具有相关性，这表明存在一种跨区域的显著确定性驱动。计算建模表明，这种驱动具有随试次变化的初始值和速率，且速率在试次内增加。尽管确定性驱动足以触发动作，但试次内的噪声也有助于设定动作时机。因此，离散（跨试次）和连续（试次内）的变异源协同作用，共同决定自发动作的时机。这种协同作用在全脑范围内均可观察到，表明这是一个分布式的决策过程，而非层级化、模块化的过程。

## Abstract
Deciding when to act in the absence of external cues is essential for exploration, learning, and survival. Yet the neural mechanisms underlying such decisions remain controversial, with current views favoring either deterministic or stochastic underpinnings. We simultaneously recorded from large neuronal populations in cortical, thalamic, pallidal, and cerebellar regions as mice self-initiated voluntary actions. Action onset timing was predictable from firing patterns up to several seconds in advance with predictions correlated across regions, demonstrating a prominent deterministic drive that spans regions. Computational modeling indicated that this drive has an initial value and rate that vary trial-by-trial, and the rate increases within trials. Although the deterministic drive is sufficient to trigger action, noise within trials also contributes to setting action timing. Therefore, discrete (across-trial) and continuous (within-trial) sources of variability synergize to time self-initiated actions. This synergy is observed brain-wide, suggesting a distributed decision-making process rather than a hierarchical, modular one.