---
title: Intermittent movement control emerges from information-based planning
authors: "Takagi, A., Verdel, D., Burdet, E."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.05.641580v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 用于运动启动与规划的信息预测控制框架
tldr: 哺乳动物的运动控制具有离散性，但现有模型难以解释纠正动作的触发时机和持续时间。本研究提出了信息预测控制（IPC）框架，将模型预测控制与信息论相结合。IPC 仅在出现意外偏差且纠正动作可能成功时才触发修正，通过量化“惊奇度”来整合传感器噪声和任务约束。仿真结果显示，IPC 能在多种任务中重现类人行为，并能根据环境不确定性动态调整规划视野，为理解生物运动控制提供了新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决现有运动控制模型无法明确解释离散动作纠正的触发时机与持续时间的问题。
method: 提出 IPC 框架，结合模型预测控制与信息论，利用“惊奇度”量化偏差并决定是否启动纠正动作。
result: 仿真证明 IPC 在离散到达、连续追踪和不确定性规划任务中均能产生类人行为，并能动态适应复杂环境。
conclusion: 该研究表明间歇性运动控制可以从基于信息的规划机制中自然涌现，为生物运动控制提供了统一的理论框架。
---

## Abstract
Mammalian motor control is inherently discrete, with movement corrections occurring at rates determined by task demands and the quality of sensory information. While several models have been proposed to explain this discreteness, it remains unclear when a new movement should be initiated and how long it should last. To address this gap, we introduce the Information Predictive Control (IPC) framework, which combines model predictive control with information theory. IPC triggers corrections only when unexpected deviations arise and when corrective actions are likely to succeed. By quantifying "surprise" relative to predicted internal and external states, IPC generates successful movements while robustly integrating sensorimotor noise, task constraints, and target variability. Simulations show that IPC reproduces human-like behavior in discrete reaching, continuous target tracking, and adaptive planning under uncertainty, while dynamically adjusting the planning horizon in complex, unpredictable environments.