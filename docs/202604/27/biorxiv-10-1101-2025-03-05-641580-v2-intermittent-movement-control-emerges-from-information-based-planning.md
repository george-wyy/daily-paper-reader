---
title: Intermittent movement control emerges from information-based planning
title_zh: 间歇性运动控制源于基于信息的规划
authors: "Takagi, A., Verdel, D., Burdet, E."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.05.641580v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 基于惊喜度的运动校正信息预测控制框架
tldr: 哺乳动物的运动控制具有固有的离散性，但现有模型难以解释动作修正的触发时机和持续时间。本研究提出了信息预测控制（IPC）框架，将模型预测控制与信息论相结合。IPC 仅在出现意外偏差且修正动作可能成功时才触发修正，通过量化“意外”程度来整合感觉运动噪声和任务约束。该框架在多种任务中成功模拟了类人行为，揭示了间歇性控制源于基于信息的规划机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决现有运动控制模型中关于动作修正触发时机和持续时间不明确的问题。
method: 提出结合模型预测控制与信息论的 IPC 框架，利用“意外”程度和成功概率来动态触发运动修正。
result: 仿真证明 IPC 能在离散到达、目标追踪和不确定性规划等任务中复现人类的运动特征。
conclusion: 研究表明间歇性运动控制是基于信息的规划过程的自然产物，为解释复杂环境下的运动行为提供了理论基础。
---

## 摘要
哺乳动物的运动控制本质上是离散的，运动校正的频率由任务需求和感觉信息的质量决定。尽管已有多种模型被提出用于解释这种离散性，但关于何时应启动新运动以及运动应持续多久，目前仍不清楚。为了填补这一空白，我们引入了信息预测控制（Information Predictive Control, IPC）框架，该框架将模型预测控制与信息论相结合。IPC 仅在出现意外偏差且校正动作可能成功时才触发校正。通过量化相对于预测的内部和外部状态的“惊奇度”，IPC 在稳健地整合感觉运动噪声、任务约束和目标变异性的同时，生成成功的运动。仿真结果表明，IPC 在离散触及、连续目标追踪以及不确定性下的自适应规划中重现了类人行为，同时在复杂且不可预测的环境中动态调整规划时界。

## Abstract
Mammalian motor control is inherently discrete, with movement corrections occurring at rates determined by task demands and the quality of sensory information. While several models have been proposed to explain this discreteness, it remains unclear when a new movement should be initiated and how long it should last. To address this gap, we introduce the Information Predictive Control (IPC) framework, which combines model predictive control with information theory. IPC triggers corrections only when unexpected deviations arise and when corrective actions are likely to succeed. By quantifying "surprise" relative to predicted internal and external states, IPC generates successful movements while robustly integrating sensorimotor noise, task constraints, and target variability. Simulations show that IPC reproduces human-like behavior in discrete reaching, continuous target tracking, and adaptive planning under uncertainty, while dynamically adjusting the planning horizon in complex, unpredictable environments.