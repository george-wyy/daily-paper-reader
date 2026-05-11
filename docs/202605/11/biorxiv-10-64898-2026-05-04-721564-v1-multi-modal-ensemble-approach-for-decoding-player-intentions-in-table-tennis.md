---
title: Multi-modal Ensemble Approach for Decoding Player Intentions in Table Tennis
title_zh: 乒乓球运动中解码选手意图的多模态集成方法
authors: "Pham, T. Q., Funai, S. S., Kanai, R., Chikazoe, J."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.04.721564v1.full.pdf"
tags: ["query:gaze-intent"]
score: 9.0
evidence: 使用EEG和姿态解码球员意图的多模态集成方法
tldr: 本研究旨在通过脑电图（EEG）和姿态特征预测乒乓球运动员的攻击意图。研究利用公开数据集，针对9名球员开发了基于EEGNet和随机梯度下降模型的分类器。结果表明，EEG在击球前500毫秒即具有预测性，而姿态特征在100毫秒时表现最佳。通过多模态集成方法，预测性能显著提升，为神经假体和运动训练工具的开发提供了新思路。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探索在激烈体育运动中，如何结合脑电信号和肢体动作提前预测人类的运动意图。
method: 采用基于EEGNet的脑电分类器和基于随机梯度下降的姿态分类器，并构建多模态集成模型进行预测。
result: 多模态集成模型在预测左右攻击意图上达到了0.563的F1分数，优于单一模态的预测效果。
conclusion: 该研究证明了多模态融合在运动意图解码中的有效性，对神经康复和体育竞技训练具有应用价值。
---

## 摘要
本研究旨在预测剧烈运动过程中的人类意图，特别是乒乓球运动。利用包含同步脑电图（EEG）和视频记录的公开“真实世界乒乓球数据集”（Real World Table Tennis dataset），我们基于姿态特征和脑电信号，为九名选手（7名男性，2名女性；年龄范围18-30岁）开发了一系列针对特定参与者的分类器。基于姿态的分类器采用了带有逻辑损失的随机梯度下降模型，而基于脑电的分类器则采用了改进的卷积神经网络架构（EEGNet）。两种分类器均成功地从球拍触球前的时间窗口预测了左右进攻意图，其中姿态特征的最佳解码时间点为-100毫秒，脑电信号为-500毫秒。基于脑电的解码性能优于基于姿态的解码，而多模态集成进一步提升了预测效果，平均宏F1分数达到0.563（自助法95%置信区间：0.523-0.603），相比仅使用姿态和仅使用脑电的分类器分别提升了0.03和0.02。由于每个分类器都是独立训练的，该集成模型在未来可以可行地扩展以纳入更多模态。这些结果表明，该方法在神经假体系统和体育训练的神经反馈工具中具有潜在的应用前景。

## Abstract
This study aims to predict human intentions during intense sports activities, specifically in table tennis. Using a publicly available Real World Table Tennis dataset containing simultaneous EEG and video recordings, we developed a series of participant-specific classifiers for nine players (7 males and 2 females; age range 18-30), based on pose features and EEG signals. The pose-based classifier used a stochastic gradient descent model with logistic loss, whereas the EEG-based classifier employed a modified convolutional neural network architecture (EEGNet). Both classifiers successfully predicted left-right attack intentions from the time windows preceding racket-ball impact, with optimal decoding occurring at -100 ms for pose features and -500 ms for EEG signals. EEG-based decoding achieved higher performance than pose-based decoding, and a multi-modal ensemble further improved prediction, reaching a mean macro F1 score of 0.563 (bootstrapped 95% CI: 0.523-0.603), corresponding to gains of +0.03 over pose-only and +0.02 over EEG-only classifiers. Because each classifier is trained independently, the ensemble can be feasibly extended to incorporate additional modalities in the future. These results suggest potential applications in neural prosthetic systems and neurofeedback tools for sports training.

---

## 论文详细总结（自动生成）

这篇论文介绍了一种在乒乓球运动中解码选手攻击意图的多模态集成方法。以下是详细的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：如何在剧烈、高速且充满干扰的真实运动场景（如乒乓球）中，提前解码人类的运动意图（即球向左还是向右攻击）。
*   **研究动机**：传统的意图解码多基于“运动想象”（Motor Imagery），且在受控实验室环境下进行，难以反映真实运动中的潜意识决策。乒乓球运动决策时间极短（数百毫秒），且选手常有欺骗性动作。
*   **整体含义**：通过结合内部神经信号（EEG）和外部运动学特征（姿态），构建一个鲁棒的解码框架，为神经假体、运动训练神经反馈及体育分析提供技术支撑。

### 2. 方法论
核心思想是构建一个**模块化的决策级集成框架**，并行处理脑电和姿态数据。
*   **姿态分类器**：
    *   使用 OpenPose 提取关键点，并创新性地推导出**链接坐标、方向（$\theta$）和长度（$L$）**作为额外特征。
    *   采用带有逻辑损失和 ElasticNet 正则化的**随机梯度下降（SGD）模型**。
*   **EEG 分类器**：
    *   基于 **EEGNet**（一种轻量级卷积神经网络）架构。
    *   **关键技术细节**：采用**迁移学习**策略。先在其他受试者数据上进行预训练（Group Model），再针对目标受试者进行微调（Fine-tuning），并冻结首层卷积以保留通用特征。
    *   针对类别不平衡（左攻多于右攻），在损失函数中引入类别权重，并结合过采样技术。
*   **集成策略**：
    *   采用决策级融合，对比了逻辑回归（Stacking）、KNN（Blending）、梯度提升和**决策树（Decision Tree）**。实验发现决策树在多数情况下表现最优。

### 3. 实验设计
*   **数据集**：使用公开的“Real World Table Tennis dataset”，包含同步的 120 通道 EEG 和全身体感视频。
*   **受试者**：筛选了 9 名具有一定经验的选手（7男2女）。
*   **Benchmark 与对比方法**：
    *   **单模态对比**：仅姿态 vs 仅 EEG。
    *   **模型架构对比**：EEGNet vs 传统 SGD vs Transformer 变体（EEGConformer, CTNet）。
    *   **训练策略对比**：从头训练 vs 迁移学习。
    *   **时间窗口分析**：测试了击球前 0ms 到 2s 的多个时间点，确定了 EEG 的最佳窗口为 -500ms，姿态为 -100ms。

### 4. 资源与算力
*   **硬件配置**：工作站配备 Intel Core i7 CPU，**128 GB RAM**，以及 **Quadro P6000 GPU**。
*   **软件环境**：Ubuntu 16.04 LTS，使用 PyTorch 和 Scikit-learn 库。
*   **训练时长**：文中未明确说明具体的训练总时长，但提到 EEGNet 属于轻量级模型，且在验证集损失 50 个 epoch 未改善时执行早停（Early Stopping）。

### 5. 实验数量与充分性
*   **实验规模**：对 9 名受试者分别建立了特定分类器，采用了 **8 折交叉验证**。
*   **充分性评价**：
    *   **统计严谨性**：使用了线性混合效应模型（Linear Mixed-effects Model）处理个体差异，并利用自助法（Bootstrapping）计算 95% 置信区间。
    *   **消融/对比实验**：涵盖了特征工程、模型架构、训练策略和集成算法的全面对比，实验设计较为客观、公平。
    *   **局限性**：样本量（9人）相对较小，且存在显著的类别不平衡问题。

### 6. 主要结论与发现
*   **集成优势**：多模态集成模型的平均宏 F1 分数达到 **0.563**，显著优于单一模态（比姿态高 0.03，比 EEG 高 0.02）。
*   **时间领先性**：EEG 信号在击球前 **500ms** 即可解码意图，早于姿态特征（**100ms**），证明了脑电信号在预判中的核心价值。
*   **迁移学习有效性**：在 EEG 解码中，迁移学习显著提升了“左攻 vs 其他”任务的性能（提升 8.8%）。
*   **互补性**：混淆矩阵显示，姿态分类器对右攻更敏感，而 EEG 对左攻更准确，集成模型平衡了两者的误差。

### 7. 优点
*   **真实场景应用**：突破了实验室“运动想象”的限制，在高速、高强度的真实体育竞技中实现了意图解码。
*   **模块化扩展性**：决策级集成允许独立优化各模态分类器，未来可轻松接入 IMU、EMG 等更多传感器。
*   **特征创新**：为姿态分类器引入了链接方向和长度特征，显著提升了基于静态帧的预测精度。

### 8. 不足与局限
*   **样本与偏差**：受试者数量较少，且数据集存在天然的“左攻偏好”偏见，可能影响模型的泛化能力。
*   **实时性限制**：目前为离线分析，120 通道 EEG 和复杂的姿态提取流程在实时部署上存在计算延迟挑战。
*   **标签可靠性**：意图标签是由外部观察者根据球的轨迹标注的，而非选手自述，可能存在“意图-行为”不一致的风险。
*   **特征深度**：姿态分析目前基于静态帧，未充分利用动作的动态时序信息（如速度、加速度）。

（完）
