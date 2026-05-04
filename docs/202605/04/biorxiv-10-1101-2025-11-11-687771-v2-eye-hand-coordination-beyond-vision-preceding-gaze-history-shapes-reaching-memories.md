---
title: "Eye-hand coordination beyond vision: preceding gaze history shapes reaching memories"
title_zh: 超越视觉的眼手协调：先前的注视历史塑造触及记忆
authors: "Abekawa, N., Gomi, H."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.11.687771v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 先前的注视历史塑造了触及记忆与协调
tldr: 本研究探讨了眼手协调在视觉引导之外的功能，发现到达动作的记忆形成与先前的注视历史紧密相关。通过实验证明，当不同的到达动作与特定的先前眼动关联时，可以同时学习两个相互干扰的视觉运动映射。研究揭示了注视状态的时间加权距离决定了学习的泛化模式，强调了眼动在灵活运动学习中的关键作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究先前的眼动历史是否会影响到达动作记忆的形成及其在运动学习中的作用。
method: 通过让受试者在不同的先前眼动条件下学习两个相互冲突的视觉运动映射，并分析其泛化模式。
result: 发现受试者能同时习得相互干扰的映射，且泛化模式可用注视状态的时间加权距离来解释。
conclusion: 到达动作记忆与近期注视历史紧密关联，眼手协调在协调灵活的运动学习中具有重要功能。
---

## 摘要
熟练的触及行为（如抓取杯子或接球）需要根据误差信号进行适应性改变。我们的自然触及通常与先前的眼动相协调。尽管具有这种行为相关性，但先前眼动与触及记忆形成之间的潜在联系在很大程度上被忽视了。我们展示了两个相反的触及视觉运动映射（通常因干扰而阻碍学习），当它们分别与不同的紧接在前的眼动相关联时，是可以被学习的。我们进一步表明，触及学习在不同注视条件下的泛化模式可以通过利用时间加权计算的注视状态距离来解释。这些发现表明，触及记忆的编码与先前注视状态的近期历史紧密相关。我们的结果将眼手协调的功能作用扩展到了视觉引导之外，揭示了其在协调灵活运动学习中的重要性。

## Abstract
Skilled reaching behaviors, such as grasping a cup or catching a ball, require adaptive changes in response to error signals. Our natural reaches are usually coordinated with preceding eye movements. Despite this behavioral relevance, the potential linkage between preceding eye movements and memory formation for reaching has been largely overlooked. We show that two opposing visuomotor maps for reach, which normally prevent learning due to interference, can be learned when each is associated with a different immediately preceding eye movement. We further show that the generalization pattern of reach learning across different gaze conditions can be explained by the gaze state's distance computed with temporal weighting. These findings indicate that reaching memories are encoded in tight association with the recent history of preceding gaze states. Our results expand the functional role of eye-hand coordination beyond visual guidance, revealing its importance in orchestrating flexible motor learning.

---

## 论文详细总结（自动生成）

这篇论文由日本 NTT 通讯科学实验室和早稻田大学的研究人员完成，探讨了眼手协调在视觉引导之外的深层功能。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：在触及动作（reaching）发生之前的**动态注视历史（gaze history）**是否会影响大脑对运动记忆的编码和提取？
*   **背景**：传统的眼手协调研究主要关注注视如何提供视觉引导（如目标定位）。然而，在现实生活中（如打网球），眼动往往先于手部动作。
*   **研究动机**：研究者试图探究注视状态是否能作为一种“上下文（Context）”，帮助大脑区分并存储相互冲突的运动映射（如在不同注视路径下应对不同的视觉运动干扰）。

### 2. 论文提出的方法论
*   **核心思想**：利用“视觉运动旋转（Visuomotor Rotation）”任务，将相互冲突的干扰（顺时针 CW vs. 逆时针 CCW 旋转）与特定的注视历史关联。如果受试者能同时学会这两种相反的映射，则证明注视历史是有效的记忆上下文。
*   **关键技术细节**：
    *   **上下文关联学习**：在实验中，不同的眼动模式（如静态注视 vs. 动态扫视，或不同路径的序列扫视）被赋予不同的视觉反馈干扰。
    *   **时间加权模型**：为了量化注视历史的影响，研究者提出了一个计算“注视状态距离”的模型。该模型通过高斯函数对触及动作发生前的时间点进行加权，计算当前注视状态与学习状态之间的差异。
    *   **公式逻辑**：$d_P(t) = \{x_P(t) - x_L(t)\}^2 \cdot \exp(-\frac{t^2}{2\sigma_t^2})$，其中 $x$ 是眼球位置，$t$ 是相对于触及开始的时间，$\sigma_t$ 是时间窗口宽度。

### 3. 实验设计
*   **场景与设备**：受试者在数字化平板上移动笔，在显示器上观察光标。使用 Eyelink 2000 追踪眼动。
*   **主要实验**：
    *   **实验 1**：对比静态注视（中心或外围）与动态扫视。设置了三组不同的时间间隔（短、中、长），观察注视历史效应随时间的衰减。
    *   **实验 2**：对比两种不同的序列扫视路径（左侧路径 vs. 右侧路径），排除单一静态注视点的干扰。
    *   **实验 3（泛化实验）**：在 14 种不同的注视条件下测试学习效果，用于拟合时间加权模型。
*   **对照实验**：
    *   **对照 1 & 2**：仅提供视觉上的目标跳变，但不允许眼动，以证明效应源于“眼动状态”而非单纯的“视觉信号”。

### 4. 资源与算力
*   **算力说明**：论文未提及使用高性能 GPU 或大规模算力。由于这是一项人类行为学实验，数据处理主要涉及常规的统计分析（ANOVA、T-检验）和基于 MATLAB 的非线性最小二乘拟合。
*   **软件环境**：使用 MATLAB (R2012a) 和 Psychophysics Toolbox (PTB-3)。

### 5. 实验数量与充分性
*   **样本量**：共招募了 84 名健康受试者，分为 7 个组（每组 12 人，包括 3 个主实验和 4 个对照/分支组）。
*   **充分性**：
    *   实验设计非常严密，通过对照实验排除了“视觉引导差异”和“单纯视觉刺激”的影响。
    *   通过操纵时间间隔（Gap duration）深入探讨了记忆的时间特性。
    *   泛化实验涵盖了 14 种条件，为模型拟合提供了足够的数据点。
    *   统计分析采用了 Bonferroni 校正和 Tukey 后验检验，确保了结果的客观性。

### 6. 主要结论与发现
*   **注视历史作为上下文**：大脑可以利用触及前的动态眼动模式来区分并存储相反的运动记忆。
*   **时间敏感性**：这种效应具有明显的时间衰减特性。当眼动结束与触及开始之间的间隔超过 1 秒时，注视历史的上下文作用显著减弱或消失。
*   **时间窗口**：模型估计显示，触及前约 **600 毫秒**内的注视历史对运动记忆的形成和提取贡献最大。
*   **功能意义**：眼手协调不仅是为了“看清目标”，更是为了在复杂的动态行为中组织和协调灵活的运动学习。

### 7. 优点
*   **视角新颖**：首次系统地证明了动态眼动历史（而非仅仅是静态注视位置）是运动记忆编码的关键维度。
*   **实验控制严谨**：成功区分了视觉输入（Visual input）与运动状态（Motor state）对学习的贡献。
*   **量化建模**：不仅观察到现象，还通过数学模型量化了注视历史的时间加权影响，增强了理论深度。

### 8. 不足与局限
*   **任务单一性**：实验主要基于实验室环境下的视觉运动旋转任务，尚不清楚在更复杂的力场适应或真实体育运动中，这种效应的强度如何。
*   **神经机制推测**：虽然论文讨论了顶叶皮层（LIP）和前额叶皮层（FEF）的潜在作用，但缺乏直接的神经生理学证据（如 fMRI 或电生理记录）。
*   **应用限制**：研究发现的时间窗口较短（<1s），这可能限制了其在某些长时延反应场景中的应用。

（完）
