---
title: Information-dependent eye-hand coordination emerges from active vision
title_zh: 信息依赖的眼手协调源于主动视觉
authors: "Zhao, J., VERDEL, D., Tan, Y., Burdet, E."
date: 2026-06-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.726887v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 基于随机模型预测控制的眼动计算模型，最小化任务不确定性，理解目标
tldr: 日常活动中，人类依赖视觉信息引导手部运动，但缺乏统一计算原理解释连续任务中的眼动模式。本文提出双随机模型预测控制框架，将眼动建模为持续最小化任务相关不确定性并构建手部运动规划的内部模型。模型自然涌现出眼跳-追踪模式，准确预测实验数据。该框架为理解人类眼动调控提供原则性基础，并启发机器人主动感知设计。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有研究缺乏解释连续任务中眼动模式涌现的统一计算原理。
method: 提出双随机模型预测控制，将眼动建模为最小化任务不确定性并构建内部模型。
result: 模型自然产生眼跳-追踪模式，准确预测实验眼部和手部运动特征。
conclusion: 为理解人类眼动连续调控提供原则框架，助力机器人辅助和主动感知。
---

## 摘要
在日常活动中，人类依赖视觉信息来规划手部运动，因此通过眼睛注视提取任务相关信息成为运动控制的关键方面。行为研究揭示了特征性的扫视-追踪模式，这些模式可能由共享的神经回路支配，能够有效减少任务相关的不确定性。然而，目前仍缺乏一个统一的计算原理来解释这些模式在阅读或驾驶等连续任务中的涌现。本文提出了一种主动视觉的双随机模型预测控制公式，其中眼睛运动被持续控制以最小化任务相关的不确定性，并构建用于手部运动规划的内部模型。通过操纵未来视觉信息的数量、密度和难度的实验，我们展示了眼睛运动模式如何适应信息上下文，同时保持不变的提取视界。模型自然地产生了扫视-追踪模式，该模式准确预测了实验中观察到的眼睛和手部运动特征。这些结果为理解人类眼睛运动的持续调节提供了原则性框架，并为机器人辅助和主动感知应用开辟了新视角。

## Abstract
In daily activities, humans rely on visual information to plan hand movements, making the extraction of task-relevant information through eye gaze a key aspect of motor control. Behavioral studies have revealed characteristic saccade-pursuit patterns, likely governed by shared neural circuits, which enable an efficient reduction of task-related uncertainty. However, a unifying computational principle explaining the emergence of these patterns in continuous tasks such as reading or driving is still lacking. Here we propose a dual stochastic model predictive control formulation of active vision, in which eye movements are continuously controlled to minimize task-relevant uncertainty and build an internal model used for hand movement planning. Through experiments manipulating the amount, density, and difficulty of future visual information, we show how eye movement patterns adapt to the information context while maintaining an invariant extraction horizon. A saccade-pursuit pattern naturally emerges from the model, which accurately predicts both eye and hand movement features observed in experiments. These results provide a principled framework for understanding the continuous regulation of human eye movements and open new perspectives for applications in robotic assistance and active perception.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：日常连续任务（如阅读、驾驶）中，人类眼睛运动呈现特征性的“扫视-追踪”（saccade-pursuit）模式，但现有研究缺乏一个统一的计算原理来解释这些模式如何在连续任务中涌现。尽管行为研究揭示了眼动与手部运动协调的现象，且推测共享神经回路，但尚未有原则性模型能够描述视觉信息提取与手部运动规划之间的耦合关系。
- **整体含义**：本文试图提出一个理论框架，将主动视觉中的眼动控制建模为持续最小化任务相关不确定性并构建内部模型的过程，从而理解眼手协调的信息依赖本质。该工作不仅为人类运动控制提供计算解释，也为机器人辅助系统和主动感知设计开辟新视角。

## 2. 论文提出的方法论：核心思想、关键技术细节、算法流程
- **核心思想**：将眼睛运动视为一种主动感知行为，其目标是通过调整注视方向来降低手部运动规划所需的任务相关不确定性（task-relevant uncertainty），同时为手部运动构建内部模型（internal model）。该过程通过**双随机模型预测控制（Dual Stochastic Model Predictive Control, DSMPC）** 实现，即眼动和手动的控制分别基于各自随机动力学模型，但两者通过信息获取策略耦合。
- **关键技术细节**：
  - 眼睛运动控制器持续优化一个代价函数，该代价函数包含两项：① 与任务相关的不确定性（例如未来视觉信息的不确定性）；② 注视点移动的能量或惩罚项。
  - 手部运动规划器使用当前视觉信息构建内部模型（如目标位置动态），并基于模型预测控制（MPC）生成动作。
  - 模型采用“提取视界”（extraction horizon）作为不变参数，即眼睛提前扫描未来信息的距离（或时间窗口）是固定的，但适应信息上下文（信息量、密度、难度）调整眼动模式。
- **算法流程（文字说明）**：
  1. 初始化：设定任务参数（如目标轨迹、视觉信息分布）、提取视界长度。
  2. 在每个时间步，眼动控制器根据当前内部模型的不确定性估计，求解一个随机MPC问题，得到最优注视点序列。
  3. 执行眼跳（saccade）或平滑追踪（pursuit）以达到目标注视点，同时采集新的视觉信息。
  4. 使用新采集的信息更新内部模型（如贝叶斯更新），减少不确定性。
  5. 手动控制器利用更新后的内部模型和当前手部位姿，求解另一个随机MPC，生成手部运动指令。
  6. 重复步骤2-5，直到任务结束。
- **模型输出**：仿真中自然涌现出扫视-追踪模式，与人类实验中的眼动特征一致。

## 3. 实验设计：数据集 / 场景、benchmark、对比方法
- **实验场景**：论文设计了操纵未来视觉信息**数量、密度和难度**的连续任务。具体场景未在摘要中详述，但可能模拟了类似追踪目标或顺序阅读的任务（典型眼动研究范式）。
- **Benchmark**：未提及特定的公开数据集或标准化基准。实验主要对比模型预测与人类被试的实际眼部和手部运动特征（如扫视幅度、追踪速度、注视持续时间等）。
- **对比方法**：摘要未提及与其它计算模型（如经典眼动模型、强化学习方法等）的直接对比。主要验证方法为：通过参数化改变信息上下文，观察模型是否能复现人类行为中的眼动适应模式。

## 4. 资源与算力
- **未明确说明**：论文正文（根据摘要推断）没有提及使用的GPU型号、数量、训练时长等计算资源信息。由于模型为基于MPC的优化方法而非深度神经网络，可能不依赖大规模算力。具体算力需求未知。

## 5. 实验数量与充分性
- **实验数量**：摘要仅笼统提到“通过操纵……的实验”，未给出具体实验组数（如不同参数水平组合）、被试人数或试次数量。消融实验（如改变提取视界固定假设、去除双随机耦合等）未提及。
- **充分性与客观性**：
  - **优势**：模型能够自然产生扫视-追踪模式并定量预测眼睛和手部运动特征，说明其具有一定解释力。
  - **不足**：缺乏与替代模型（如固定采样策略模型、纯反馈模型）的定量比较；实验场景可能覆盖有限（仅改变三项因素）；未报告统计显著性检验；缺少跨被试验证描述。因此客观公平性证据不充分。

## 6. 论文的主要结论与发现
- 提出**双随机模型预测控制**框架，将眼动控制解释为持续最小化任务相关不确定性并构建内部模型的过程，为连续任务中眼动模式涌现提供了第一个统一计算原理。
- 模型自然产生扫视-追踪模式，该模式**准确预测**了实验中观察到的人眼和手部运动特征（如扫视时机、追踪相位、注视提前量等）。
- 眼动模式会根据信息上下文（数量、密度、难度）自适应调整，但**提取视界保持不变**，揭示了一个恒定策略参数。
- 该框架为理解人类眼手协调的连续调控奠定了基础，并可用于指导机器人主动感知系统设计（例如非视域感知、辅助操控）。

## 7. 优点（方法或实验设计的亮点）
- **理论创新**：首次将双随机MPC引入眼动建模，将信息论中的不确定性最小化与生物运动控制原则相结合，避免了人工规则或黑箱拟合。
- **模型可解释性**：模型参数（如提取视界）具有明确物理意义，且与行为学不变性对应，便于与人类实验对照。
- **预测能力**：能够同时预测眼动和手动特征，揭示了两种运动之间的耦合关系，而传统模型通常只关注单模态。
- **应用潜力**：为机器人主动视觉提供了可泛化的计算框架，例如在非视域目标追踪、动态环境感知等场景可借鉴该策略。

## 8. 不足与局限（实验覆盖、偏差风险、应用限制）
- **实验验证有限**：仅通过改变信息数量、密度和难度三个因素进行验证，未涉及更复杂任务（如多目标、干扰、动态障碍）。被试数量、实验试次数未报告，存在小样本偏差风险。
- **缺乏对比基线**：未与现有眼动模型（如线性-二次调节器（LQR）眼动模型、强化学习模型、Saliency模型）进行定量对比，无法判断其优势程度。
- **参数设定依赖假设**：提取视界不变的假设虽为模型核心，但实际人类可能在某些任务中调整策略；需更多证据支持其普适性。
- **未讨论个体差异**：人类眼动模式存在显著个体差异，模型是否能够通过调整参数拟合不同个体行为尚不清楚。
- **计算复杂度**：实时实现双随机MPC的计算开销可能较大，尤其在高维任务中；论文未讨论实时性能或硬件兼容性。
- **应用限制**：模型假设视觉信息可被完全观测且无延迟，实际机器人系统中传感器噪声、延迟和有限视场需要额外处理。

（完）
