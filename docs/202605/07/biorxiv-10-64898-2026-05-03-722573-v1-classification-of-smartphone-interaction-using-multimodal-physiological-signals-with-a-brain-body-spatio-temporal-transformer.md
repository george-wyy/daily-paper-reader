---
title: Classification of Smartphone Interaction Using Multimodal Physiological Signals with a Brain-Body Spatio-Temporal Transformer
title_zh: 基于脑-体时空 Transformer 的多模态生理信号智能手机交互分类
authors: "Mishra, P., Kagathara, V., Gandhi, T. K."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.03.722573v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 包含眼动追踪的多模态信号用于智能手机交互分类
tldr: 本研究针对智能手机不同交互行为（如短视频和游戏）引起的生理反应差异，提出了名为BB-STT的脑体时空Transformer框架。该框架整合了EEG、EDA、PPG和眼动追踪等多模态信号，在区分手机使用及具体交互类型上表现优异。通过跨模态注意力机制，模型实现了高精度的分类，并揭示了不同生理特征在识别数字参与度中的层次化作用，为自然场景下的实时评估提供了可能。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的研究往往将智能手机使用视为单一行为，忽视了不同交互方式（如刷视频与玩游戏）所引发的独特认知和生理反应。
method: 提出了一种名为BB-STT的深度学习框架，利用跨模态注意力机制动态整合脑电、皮电、脉搏和眼动等多模态生理信号。
result: "该模型在区分手机与非手机活动中达到83.51%的准确率，在三类交互行为分类中达到74.13%的准确率，且具有良好的泛化能力。"
conclusion: 研究证明了多模态生理信号在客观、实时评估自然环境下数字交互参与度方面的巨大潜力。
---

## 摘要
不同的智能手机交互行为（如短视频刷屏和手机游戏）会引发性质迥异的认知和生理反应。然而，将智能手机使用视为单一行为的方法往往忽略了这种差异。本文提出了脑-体时空 Transformer（BB-STT），这是一个统一的深度学习框架，用于从包括脑电图（EEG）、皮肤电活动（EDA）、光电容积脉搏波（PPG）和眼动追踪在内的多模态信号中分类特定交互的生理特征。BB-STT 在区分智能手机与非智能手机活动方面达到了 83.51% 的准确率，在短视频、游戏和基准观看的三分类任务中达到了 74.13% 的准确率。该模型表现出很强的泛化能力，其留一法（LOSO）性能与 5 折交叉验证准确率相当。跨模态注意力机制成为关键组件，通过多模态信号的动态整合，将三分类准确率提高了 16.74 个百分点。可解释性分析表明生理反应具有层级结构。眼动追踪特征（尤其是注视深度）能够实现智能手机与非智能手机活动的粗略区分。相比之下，对智能手机上被动视频观看和主动游戏进行更精细的区分，则依赖于双侧瞳孔扩大和中央区 EEG 特征的共同贡献。总之，这些结果证明了多模态生理信号在自然环境下对数字参与度进行客观、实时评估的潜力。

## Abstract
Distinct smartphone interaction behaviors, like short-form video scrolling and mobile gaming, elicit qualitatively different cognitive and physiological responses. However, such distinctions is often overlooked by approaches that treat smartphone use as a monolithic behavior. This paper presents BrainBody Spatio-Temporal Transformer (BB-STT), a unified deep learning framework for classifying interaction-specific physiological signatures from multimodal signals, including EEG, EDA, PPG, and eye-tracking. BB-STT achieves 83.51% accuracy in distinguishing smartphone from non-smartphone activity and 74.13% accuracy in three-class classification of short-form video, gaming, and baseline viewing. The model demonstrates strong generalization with leave-one-subject-out (LOSO) performance that is also comparable to 5-fold cross-validation accuracy. Crossmodal attention emerges as the key component, improving three-class accuracy by 16.74 points through dynamic integration of multimodal signals. Interpretability analysis indicates a hierarchical organization of physiological responses. Eye-tracking features, particularly gaze depth, enable coarse separation between smartphone and non-smartphone activity. In contrast, finer discrimination between passive video viewing and active gaming on smartphones relies on the joint contribution of bilateral pupil dilation and central EEG features. Together, these results demonstrate the potential of multimodal physiological signals for objective, real-time assessment of digital engagement in naturalistic settings.

---

## 论文详细总结（自动生成）

这篇论文介绍了一种名为 **BB-STT（Brain-Body Spatio-Temporal Transformer）** 的深度学习框架，旨在通过多模态生理信号对智能手机的不同交互行为进行精细化分类。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：现有的情感计算和行为识别研究通常将“智能手机使用”视为一种单一（Monolithic）的行为。然而，刷短视频（被动消费、多巴胺寻求、低唤醒）与手机游戏（主动策略、高参与度、流向状态）在认知和生理机制上存在本质区别。
*   **研究动机**：由于缺乏对特定交互行为生理特征的区分，现有的数字健康评估工具难以准确衡量用户的心理状态。本研究旨在证明，通过整合中枢神经系统（EEG）和外周生理信号（眼动、皮电、脉搏），可以客观、实时地识别不同的数字参与模式。

### 2. 方法论：核心思想与关键技术
BB-STT 框架采用了一种端到端的架构，核心思想是利用 Transformer 机制捕捉脑电的时空特征，并通过跨模态注意力动态融合身体信号。
*   **多尺度时间编码器**：使用四个并行的 1D-CNN 分支，分别对应 EEG 的不同频段（δ, θ/α, β, γ），捕捉不同尺度的振荡动力学。
*   **特征编码器**：将原始信号编码与手工提取的领域特征（如微分熵 DE、Hjorth 参数等）进行拼接投影。
*   **空间 Transformer**：通过自注意力机制学习 64 通道 EEG 电极间的“软邻接矩阵”，利用 `[CLS]` Token 聚合全局空间特征。
*   **外周信号编码器**：对 EDA（皮电）、PPG（脉搏）和 ET（眼动）特征进行 MLP 编码。
*   **跨模态注意力融合（核心技术）**：以 EEG 嵌入作为 **Query (Q)**，外周信号嵌入作为 **Key (K)** 和 **Value (V)**。这种设计允许模型根据大脑状态动态地对自主神经、心脏和眼动信号进行加权。

### 3. 实验设计
*   **数据集与场景**：
    *   受试者：21 名健康参与者。
    *   场景：短视频滚动（SV）、手机游戏（Game）、基准视频观看（BL）。
    *   数据：64 通道 EEG、EDA、PPG、眼动追踪（Tobii Pro Glasses 2）。
*   **任务设置**：
    *   二分类：手机使用 vs. 基准观看。
    *   三分类：BL vs. SV vs. Game。
    *   成对分类：SV vs. Game 等。
*   **Benchmark 与对比方法**：
    *   **经典机器学习**：LR, SVM, RF, XGBoost, LightGBM, KNN（基于 1576 维手工特征）。
    *   **深度学习**：EEGNet, CNN-1D, LSTM, CNN-LSTM, 纯 Transformer。
*   **评估协议**：采用受试者独立的 5 折交叉验证和留一法（LOSO）交叉验证，确保模型具有跨人泛化能力。

### 4. 资源与算力
*   **硬件**：使用单张 **NVIDIA RTX A4000 GPU**。
*   **软件/框架**：PyTorch，采用自动混合精度（AMP）加速训练。
*   **训练细节**：Batch size 为 1024，最大 Epoch 为 100，使用 AdamW 优化器和余弦退火学习率调度。文中未明确说明总训练时长，但提到使用了早停机制（Patience=50）。

### 5. 实验数量与充分性
*   **实验规模**：总计 18,900 个 1 秒长度的样本。
*   **消融实验**：
    *   **模态消融**：测试了 11 种不同的模态组合（如仅 EEG、EEG+ET 等）。
    *   **架构消融**：对比了单尺度 vs. 多尺度编码、均值池化 vs. 空间 Transformer、拼接融合 vs. 跨模态注意力。
*   **充分性评价**：实验设计非常充分且客观。通过 LOSO 验证证明了模型不是在背诵受试者特征；通过 SHAP 值和排列重要性分析提供了生理学上的可解释性，增强了结果的说服力。

### 6. 主要结论与发现
*   **分类性能**：BB-STT 在二分类任务中达到 **83.51%** 准确率，在三分类任务中达到 **74.13%**，显著优于所有基准模型（F1 分数提升高达 19.45 点）。
*   **两阶段生理层级**：
    1.  **第一阶段（设备区分）**：注视深度（Gaze Depth）是区分手机使用与非手机使用的核心特征。
    2.  **第二阶段（交互区分）**：区分被动视频和主动游戏主要依赖于双侧瞳孔扩大（唤醒度指标）和中央区 EEG 特征（运动/执行控制）。
*   **融合机制的重要性**：跨模态注意力相比简单拼接，在三分类任务上准确率提升了 **16.74%**，证明了动态加权在复杂行为识别中的必要性。

### 7. 优点
*   **创新的融合策略**：提出的以 EEG 为导向的跨模态注意力机制，有效解决了不同生理信号在不同上下文中贡献度不一的问题。
*   **强泛化性**：LOSO 结果（84.32%）甚至略高于 5 折交叉验证，证明了模型捕捉的是普适的生理规律。
*   **深度可解释性**：结合 SHAP 和空间注意力图，清晰地揭示了从视觉皮层到自主神经系统的层级化响应模式。

### 8. 不足与局限
*   **样本量限制**：21 名受试者的规模相对较小，且 SV 与 Game 组的人数不平衡（14:7），可能导致模型对游戏类别的估计方差较大。
*   **内容混淆风险**：由于参与者是自选手机内容，分类结果可能部分受到了具体视频内容或游戏类型的影响，而非纯粹的交互行为差异。
*   **实时性验证不足**：虽然论文提到“实时评估”，但实验主要在离线分段数据上完成，尚未在真实的移动端流式数据中验证延迟和稳定性。
*   **环境单一**：所有数据均在受控的实验室坐姿下采集，未考虑步行、通勤等真实生活场景中的运动伪影干扰。

（完）
