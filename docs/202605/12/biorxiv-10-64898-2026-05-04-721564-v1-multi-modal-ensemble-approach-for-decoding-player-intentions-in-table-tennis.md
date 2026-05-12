---
title: Multi-modal Ensemble Approach for Decoding Player Intentions in Table Tennis
authors: "Pham, T. Q., Funai, S. S., Kanai, R., Chikazoe, J."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.04.721564v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 在运动中使用姿势和 EEG 信号进行多模态意图预测
tldr: 本研究旨在预测乒乓球运动中的人类意图，利用包含EEG和视频数据的公开数据集，开发了基于姿态特征和EEG信号的分类器。研究采用SGD模型处理姿态，EEGNet处理脑电信号，并构建了多模态集成模型。结果显示，集成模型在击球前预测进攻意图的表现优于单一模态，为神经假体和运动训练提供了新思路。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在通过多模态数据在激烈的体育活动中提前预测人类的运动意图。
method: 结合基于随机梯度下降的姿态分类器和基于卷积神经网络的脑电分类器，构建多模态集成模型。
result: 集成模型在击球前实现了0.563的平均F1分数，性能优于单一的姿态或脑电分类器。
conclusion: 该研究证明了多模态融合在运动意图解码中的有效性，对神经假体和体育神经反馈训练具有应用价值。
---

## Abstract
This study aims to predict human intentions during intense sports activities, specifically in table tennis. Using a publicly available Real World Table Tennis dataset containing simultaneous EEG and video recordings, we developed a series of participant-specific classifiers for nine players (7 males and 2 females; age range 18-30), based on pose features and EEG signals. The pose-based classifier used a stochastic gradient descent model with logistic loss, whereas the EEG-based classifier employed a modified convolutional neural network architecture (EEGNet). Both classifiers successfully predicted left-right attack intentions from the time windows preceding racket-ball impact, with optimal decoding occurring at -100 ms for pose features and -500 ms for EEG signals. EEG-based decoding achieved higher performance than pose-based decoding, and a multi-modal ensemble further improved prediction, reaching a mean macro F1 score of 0.563 (bootstrapped 95% CI: 0.523-0.603), corresponding to gains of +0.03 over pose-only and +0.02 over EEG-only classifiers. Because each classifier is trained independently, the ensemble can be feasibly extended to incorporate additional modalities in the future. These results suggest potential applications in neural prosthetic systems and neurofeedback tools for sports training.

---

## 论文详细总结（自动生成）

这是一份关于论文《Multi-modal Ensemble Approach for Decoding Player Intentions in Table Tennis》的结构化深入总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：如何在激烈、高速且具有欺骗性的真实运动场景（如乒乓球）中，准确且提前地解码人类的运动意图（左/右进攻方向）。
*   **研究背景**：传统的意图解码多基于“运动想象”（Motor Imagery），且在受控实验室环境下进行，难以反映真实运动中的潜意识决策。乒乓球运动要求极高的全身协调和快速反应（击球动作通常小于100ms），是研究动态、真实世界意图解码的理想模型。
*   **研究动机**：探索结合内部神经信号（EEG）和外部运动学线索（姿态）的多模态方法，是否能比单一模态更稳健地预测运动员意图，从而为神经假体和运动训练工具提供技术支持。

### 2. 核心方法论
研究提出了一种**模块化多模态集成框架**，主要包含以下三个部分：
*   **基于姿态的分类器**：
    *   使用 OpenPose 提取人体关键点。
    *   **关键技术**：除了原始坐标，还引入了肢体连接的**方向（$\theta$）和长度（$L$）**作为特征。
    *   **算法**：采用带有 ElasticNet 正则化的随机梯度下降（SGD）分类器。
*   **基于 EEG 的分类器**：
    *   使用 **EEGNet**（一种轻量级卷积神经网络）直接处理原始 EEG 信号。
    *   **关键技术**：采用**迁移学习（Transfer Learning）**策略。先在其他受试者数据上进行预训练（Group Model），再针对目标受试者进行微调（Fine-tuning），以克服单人数据量不足的问题。
*   **多模态集成（Ensemble）**：
    *   采用**决策级融合**策略。对比了逻辑回归、K-近邻（KNN）、梯度提升和决策树。
    *   **核心思想**：独立训练各模态分类器，通过集成模型对各模态的预测结果进行投票/加权，利用模态间的互补性减少误报。

### 3. 实验设计
*   **数据集**：使用公开的“Real World Table Tennis dataset”，包含 9 名受试者（7男2女）在真实比赛中的 120 通道 EEG 和同步视频。
*   **任务目标**：二分类任务，预测球落点是在对方球台的“左侧”还是“右侧”。
*   **Benchmark 与对比方法**：
    *   **模态对比**：仅姿态（Pose-only） vs. 仅脑电（EEG-only） vs. 多模态集成。
    *   **模型对比**：EEGNet 与传统的 SGD 以及最新的 Transformer 架构（EEGConformer, CTNet）进行对比。
    *   **时间窗口分析**：测试了击球前不同时间点（0ms 到 -2s）的预测性能。

### 4. 资源与算力
*   **硬件配置**：工作站配备 Intel Core i7 CPU，128 GB RAM，以及 **NVIDIA Quadro P6000 GPU**。
*   **软件环境**：Ubuntu 16.04 LTS，使用 PyTorch 1.12.1 和 Scikit-learn 1.0.2。
*   **训练细节**：文中未详细说明具体的训练总时长，但提到 EEGNet 属于轻量级模型，适合未来在线应用。

### 5. 实验数量与充分性
*   **实验规模**：对 9 名受试者分别建立了特定分类器。
*   **验证方法**：采用 **8 折交叉验证**（8-fold cross-validation）以防止数据泄露。
*   **统计严谨性**：使用 **10,000 次自助法（Bootstrapping）**计算 95% 置信区间，并使用线性混合效应模型（Linear Mixed-effects Model）评估集成程序的显著性。
*   **充分性评价**：实验设计考虑了类别不平衡（左侧进攻较多）并采用了加权损失函数和过采样。通过消融实验验证了新增姿态特征和迁移学习的有效性，实验设计较为客观、公平。

### 6. 主要结论与发现
*   **预测提前量**：EEG 信号在击球前 **500ms** 达到最优解码效果，而姿态特征在击球前 **100ms** 最优。这证实了神经信号先于物理动作的生物学特性。
*   **性能提升**：集成模型达到了 **0.563 的平均 Macro F1 分数**，相比纯姿态模型提升了 0.03，相比纯 EEG 模型提升了 0.02。
*   **迁移学习价值**：在 EEG 解码中，迁移学习显著提升了“左侧进攻”任务的 F1 分数（提升约 8.8%）。
*   **模型选择**：在小样本真实数据下，轻量级的 EEGNet 表现优于参数量巨大的 Transformer 模型。

### 7. 优点与亮点
*   **真实场景应用**：突破了实验室运动想象的局限，直接在高速对抗运动中提取意图。
*   **特征工程创新**：在姿态识别中引入肢体角度和长度特征，显著提升了 SGD 分类器的表现。
*   **模块化设计**：决策级集成框架具有良好的扩展性，未来可以轻松接入 EMG（肌电）或 IMU（惯性测量单元）等其他模态。
*   **迁移学习应用**：成功证明了跨受试者预训练在处理稀缺、高噪声体育 EEG 数据中的价值。

### 8. 不足与局限
*   **样本量限制**：仅分析了 9 名受试者，且样本存在严重的类别不平衡（受试者多倾向于攻击左侧）。
*   **离线分析**：目前研究基于离线分段数据，尚未实现真正的实时闭环系统。
*   **个体差异**：不同受试者的最优集成策略不尽相同，模型泛化到未见过的新选手时可能性能下降。
*   **动作简化**：仅做了左右方向的二分类，未涉及更复杂的战术意图（如旋转类型、扣杀 vs 搓球等）。
*   **伪影风险**：尽管进行了预处理，但激烈运动中的 EEG 仍可能残留运动伪影，可能对解码贡献了非神经元信息。

（完）
