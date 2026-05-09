---
title: Multi-modal Ensemble Approach for Decoding Player Intentions in Table Tennis
title_zh: 乒乓球运动中解码选手意图的多模态集成方法
authors: "Pham, T. Q., Funai, S. S., Kanai, R., Chikazoe, J."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.04.721564v1.full.pdf"
tags: ["query:gaze-intent"]
score: 9.5
evidence: 结合EEG和姿态特征的多模态玩家意图解码
tldr: 本研究旨在通过脑电图（EEG）和姿态特征预测乒乓球运动员的击球意图。研究利用公开数据集，针对9名球员开发了基于EEGNet和随机梯度下降模型的分类器。结果表明，EEG信号在击球前500毫秒即可提供预测信息，而姿态特征在100毫秒时表现最佳。通过多模态集成方法，预测性能显著提升，宏F1分数达到0.563，为神经假体和运动训练工具提供了技术支持。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探索在乒乓球等高强度运动中，如何结合脑电信号和身体姿态提前预测人类的运动意图。
method: 采用基于EEGNet的脑电分类器和基于随机梯度下降的姿态分类器，并构建多模态集成模型进行独立训练与预测。
result: 多模态集成模型在击球前取得了0.563的平均宏F1分数，性能优于单一的脑电或姿态分类器。
conclusion: 该研究证明了多模态融合在运动意图解码中的有效性，并展示了其在神经假体和运动反馈训练领域的应用潜力。
---

## 摘要
本研究旨在预测剧烈运动过程中的人类意图，特别是乒乓球运动。利用包含同步脑电图（EEG）和视频记录的公开“真实世界乒乓球数据集”（Real World Table Tennis dataset），我们基于姿态特征和脑电信号，为九名选手（7名男性，2名女性；年龄范围18-30岁）开发了一系列针对特定参与者的分类器。基于姿态的分类器采用了带有逻辑损失的随机梯度下降模型，而基于脑电的分类器则采用了改进的卷积神经网络架构（EEGNet）。两种分类器均成功地从球拍触球前的时间窗口预测了左右进攻意图，其中姿态特征的最佳解码时间点为-100毫秒，脑电信号为-500毫秒。基于脑电的解码性能优于基于姿态的解码，而多模态集成进一步提升了预测效果，平均宏F1分数达到0.563（自助法95%置信区间：0.523-0.603），相比仅使用姿态和仅使用脑电的分类器分别提升了0.03和0.02。由于每个分类器都是独立训练的，该集成模型在未来可以可行地扩展以纳入更多模态。这些结果表明，该方法在神经假体系统和体育训练的神经反馈工具中具有潜在的应用前景。

## Abstract
This study aims to predict human intentions during intense sports activities, specifically in table tennis. Using a publicly available Real World Table Tennis dataset containing simultaneous EEG and video recordings, we developed a series of participant-specific classifiers for nine players (7 males and 2 females; age range 18-30), based on pose features and EEG signals. The pose-based classifier used a stochastic gradient descent model with logistic loss, whereas the EEG-based classifier employed a modified convolutional neural network architecture (EEGNet). Both classifiers successfully predicted left-right attack intentions from the time windows preceding racket-ball impact, with optimal decoding occurring at -100 ms for pose features and -500 ms for EEG signals. EEG-based decoding achieved higher performance than pose-based decoding, and a multi-modal ensemble further improved prediction, reaching a mean macro F1 score of 0.563 (bootstrapped 95% CI: 0.523-0.603), corresponding to gains of +0.03 over pose-only and +0.02 over EEG-only classifiers. Because each classifier is trained independently, the ensemble can be feasibly extended to incorporate additional modalities in the future. These results suggest potential applications in neural prosthetic systems and neurofeedback tools for sports training.

---

## 论文详细总结（自动生成）

这篇论文介绍了一种结合脑电图（EEG）和身体姿态特征的多模态集成方法，用于在乒乓球运动中提前预测选手的击球意图。以下是对该研究的详细总结：

### 1. 核心问题与整体含义
*   **研究动机**：在乒乓球等高强度、快节奏的运动中，人类的决策和动作执行发生在极短的时间内。准确预测选手的运动意图（如击球方向）对于开发神经假体、运动训练反馈系统以及人机交互具有重要意义。
*   **核心问题**：如何利用嘈杂的真实世界数据（脑电和视频），在击球动作发生前有效地解码选手的左右进攻意图，并探讨不同模态（生理信号与物理姿态）在预测时间窗口上的贡献差异。

### 2. 方法论
该研究采用了多模态集成学习框架，主要包含以下核心组件：
*   **脑电分类器 (EEG-based)**：采用改进的 **EEGNet**（一种专为脑电信号设计的紧凑型卷积神经网络）。它通过深度可分离卷积提取空间和时间特征，能够处理非平稳的脑电信号。
*   **姿态分类器 (Pose-based)**：首先从视频中提取选手的骨骼姿态特征，然后使用带有 **逻辑损失（Logistic Loss）的随机梯度下降（SGD）模型** 进行分类。
*   **多模态集成 (Ensemble Approach)**：采用集成学习策略，将 EEG 分类器和姿态分类器的预测结果进行加权融合。由于两个分类器是独立训练的，这种架构具有良好的扩展性，便于未来加入更多模态（如眼动追踪）。
*   **时间窗口分析**：研究分析了击球前 1000 毫秒至击球瞬间（0 毫秒）的不同时间段，以确定各模态的最佳预测提前量。

### 3. 实验设计
*   **数据集**：使用公开的“真实世界乒乓球数据集”（Real World Table Tennis dataset），包含 9 名受试者（7男2女，18-30岁）在实际比赛中的同步 EEG 和视频数据。
*   **实验场景**：二分类任务，即预测选手是将球打向对方球台的“左侧”还是“右侧”。
*   **对比基准 (Benchmark)**：
    *   仅使用姿态特征的分类器。
    *   仅使用 EEG 信号的分类器。
    *   随机水平（Chance level）作为基准线。

### 4. 资源与算力
*   **算力说明**：论文摘要及提取文本中**未明确说明**具体的 GPU 型号、数量或训练时长。通常此类基于 EEGNet 的研究在单块商用 GPU（如 RTX 3080 级别）或高性能 CPU 上即可完成训练。

### 5. 实验数量与充分性
*   **实验规模**：针对 9 名选手分别训练了特定于参与者的分类器。
*   **验证方法**：使用了宏 F1 分数（Macro F1 score）作为评价指标，并计算了自助法（Bootstrapping）95% 置信区间。
*   **充分性评价**：实验覆盖了从击球前 1s 到击球时的多个时间点，对比了单模态与多模态的效果，逻辑较为严密。但受限于公开数据集，样本量（9人）相对较小，属于探索性研究。

### 6. 主要结论与发现
*   **预测性能**：多模态集成模型表现最优，平均宏 F1 分数达到 **0.563**，优于任何单一模态。
*   **时间特性差异**：
    *   **EEG 信号**在击球前 **500 毫秒** 左右即表现出较强的预测能力，反映了大脑的早期运动规划。
    *   **姿态特征**在击球前 **100 毫秒** 表现最佳，反映了身体动作在临近击球时的物理特征。
*   **模态优劣**：在整体预测表现上，基于 EEG 的解码性能略优于基于姿态的解码。

### 7. 优点
*   **多模态融合**：成功结合了“内在”生理信号（EEG）和“外在”物理表现（姿态），实现了互补。
*   **真实场景应用**：不同于实验室受控环境，该研究使用的是真实运动数据，具有更高的实际应用参考价值。
*   **时间窗口洞察**：揭示了脑电和姿态在运动意图形成过程中的时间先后顺序，具有神经科学意义。

### 8. 不足与局限
*   **样本量限制**：仅 9 名受试者，可能存在个体差异导致的泛化性问题。
*   **分类任务简单**：目前仅限于左右二分类，实际乒乓球运动涉及更复杂的意图（如旋转、力度、落点深度等）。
*   **性能上限**：F1 分数（0.563）虽然高于随机水平，但对于高可靠性的神经假体控制来说，准确率仍有待进一步提升。
*   **环境噪声**：真实世界中的 EEG 信号极易受动作伪影干扰，尽管使用了 EEGNet，但信号清洗和特征提取的鲁棒性仍是挑战。

（完）
