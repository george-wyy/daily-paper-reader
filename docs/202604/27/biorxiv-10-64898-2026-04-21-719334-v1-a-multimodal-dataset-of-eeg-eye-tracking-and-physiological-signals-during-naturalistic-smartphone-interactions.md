---
title: "A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions"
title_zh: 自然状态下智能手机交互过程中的脑电图（EEG）、眼动追踪及生理信号多模态数据集
authors: "Mishra, P., Gandhi, T. K., Gandhi, S. R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719334v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 包含自然交互过程中眼动追踪的多模态数据集
tldr: 本研究发布了一个包含EEG、眼动、PPG和GSR的多模态生理数据集，旨在揭示自然智能手机使用中的神经生理动态。研究记录了23名参与者在使用常用应用及观看基准视频时的同步信号，并结合了手机成瘾量表。该数据集遵循BIDS规范并已公开，为研究真实场景下的智能手机行为提供了重要支持。
source: biorxiv
selection_source: fresh_fetch
motivation: 智能手机已普及，但其在自然使用场景下的神经生理动态尚未得到充分表征。
method: 采集了23名参与者在使用手机应用及观看基准视频时的64通道EEG、眼动、PPG和GSR数据，并同步收集了行为量表。
result: 成功构建并公开了一个经过精确时间同步、符合BIDS规范的多模态生理信号数据集。
conclusion: 该数据集为在保持生态效度的前提下，深入研究智能手机交互过程中的神经、眼动及自主神经反应提供了有力工具。
---

## 摘要
智能手机已成为通信、信息消费和数字交互的普及工具，然而与自然状态下使用智能手机相关的神经生理动力学特征尚未得到充分描述。在此，我们展示了一个在具有生态效度的智能手机交互以及随后的标准化低参与度基线条件下收集的多模态生理数据集。23名参与者使用了他们最常用的智能手机应用程序（主要是游戏或短视频）10分钟，随后被动观看5分钟的标准化自然视频。实验同步获取了脑电图（EEG；64通道）、可穿戴眼动追踪、光电容积脉搏波（PPG）和皮肤电反应（GSR）传感器的记录。此外，还收集了包括智能手机成瘾量表（SAS）和手机问题使用量表（MPPUS）在内的问卷评估，以表征智能手机相关行为特征的个体差异。所有数据流均使用晶体管-晶体管逻辑（TTL）触发信号进行同步，以确保跨模态的精确时间对齐。该数据集根据脑成像数据结构（BIDS）规范进行组织，并已在 OpenNeuro 上公开（访问编号：ds007537）。该数据集有助于研究智能手机交互过程中的神经、眼动和自主神经反应，并支持在保持生态效度的同时对多种智能手机行为进行多模态分析。

## Abstract
Smartphones have become pervasive tools for communication, information consumption, and digital interaction, yet the neurophysiological dynamics associated with naturalistic smartphone use remain insufficiently characterized. Here, we present a multimodal physiological dataset collected during ecologically valid smartphone interaction and a subsequent standardized low-engagement baseline condition. Twenty-three participants engaged with their most frequently used smartphone application (primarily gaming or short form video) for ten minutes, followed by a five-minute passive viewing of a standardized nature video. Simultaneous recordings were obtained from electroencephalography (EEG; 64 channels), wearable eye-tracking, photoplethysmography (PPG), and galvanic skin response (GSR) sensors. Questionnaire-based assessments, including the smartphone addiction scale (SAS) and the mobile phone problematic use scale (MPPUS), are also collected to characterize individual differences in smartphone-related behavioral traits. All data streams are synchronized using transistor-transistor logic (TTL) trigger signals to ensure precise temporal alignment across modalities. The dataset is organized according to the Brain Imaging Data Structure (BIDS) specification and is publicly available on OpenNeuro (Accession Number: ds007537). This dataset enables the investigation of neural, ocular, and autonomic responses during smartphone interaction and supports multimodal analysis of diverse smartphone behaviors while preserving ecological validity.

---

## 论文详细总结（自动生成）

这篇论文介绍了一个名为“自然状态下智能手机交互过程中的脑电图（EEG）、眼动追踪及生理信号多模态数据集”的研究。以下是对该论文的结构化总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
*   **核心问题**：尽管智能手机已成为人类认知的延伸，但科学界对其在“自然使用状态”下的神经生理动态（如大脑活动、眼动模式、自主神经反应）缺乏深入了解。
*   **研究动机**：现有的研究大多采用实验者指定的任务（如阅读指定文本、打字），缺乏**生态效度（Ecological Validity）**。本研究旨在提供一个在真实、自发使用场景下的多模态同步数据集，以支持对智能手机成瘾、认知负荷及数字交互行为的深入研究。

### 2. 论文提出的方法论
*   **核心思想**：通过同步记录多种生理信号，捕捉用户在操作自选应用程序时的全方位生理反馈。
*   **关键技术细节**：
    *   **多模态采集**：集成64通道脑电（EEG）、可穿戴式眼动追踪眼镜、光电容积脉搏波（PPG）和皮肤电反应（GSR）。
    *   **时间同步**：使用**TTL（晶体管-晶体管逻辑）触发信号**。在实验开始、结束及过程中（每20秒）发送脉冲，确保EEG系统与眼动仪之间的时间对齐精度达到亚秒级。
    *   **数据标准化**：遵循**BIDS（Brain Imaging Data Structure）**规范组织数据，便于研究人员使用标准工具（如MNE-Python）进行复现和分析。
    *   **行为测评**：结合了智能手机成瘾量表（SAS）和手机问题使用量表（MPPUS），将生理数据与心理特质关联。

### 3. 实验设计
*   **参与者与场景**：23名健康成年人（20-32岁）。
*   **实验流程**：
    1.  **自然交互阶段（SM，10分钟）**：参与者自由使用自己手机上最常用的App（主要是短视频如TikTok/Instagram，或游戏如Subway Surfers）。
    2.  **基准放松阶段（VE，5分钟）**：被动观看标准化的自然风景视频，作为低认知参与的对照。
*   **验证基准（Benchmark）**：研究未对比其他算法，而是通过已知的生理现象验证数据质量，例如：
    *   **EEG**：验证放松状态下的Alpha波增强现象。
    *   **眼动**：验证手机使用（向下看）与看显示器（平视）时的垂直视线偏移。
    *   **生理**：验证交互任务（SM）比被动观看（VE）具有更高的皮肤电反应（SCR）频率。

### 4. 资源与算力
*   **算力说明**：论文主要关注数据集的构建与技术验证，**未涉及深度学习模型的训练**，因此未提及GPU型号、数量或训练时长。
*   **软件工具**：使用了Python、MNE-Python（版本1.7.0）进行信号处理和质量评估。

### 5. 实验数量与充分性
*   **实验规模**：共23组完整的多模态样本。
*   **充分性评估**：
    *   **多维度验证**：对EEG的信噪比（SNR）、眼动的空间分布、瞳孔直径的生理范围、心率变异性（HRV）等均进行了统计验证。
    *   **客观性**：通过自动化预处理流程（如ICA去除眼动伪影、自动坏道检测）减少了人为干预。
    *   **公平性**：实验设计包含了受试者内对比（Within-subject contrast），即同一人在不同任务下的对比，有效抵消了个体差异。

### 6. 论文的主要结论与发现
*   **数据集有效性**：成功构建并公开了一个高时间分辨率、精确同步的多模态数据集。
*   **生理特征发现**：
    *   **EEG**：在手机使用期间，Delta和Theta波表现出较高的信噪比；放松状态下Alpha波显著增强，符合预期。
    *   **眼动**：手机使用时的视线集中在屏幕中下部，且头部微动频率高于观看视频时期。
    *   **自主神经**：手机交互诱发了更高的皮肤电唤醒水平（SCR率更高）。

### 7. 优点
*   **高生态效度**：允许参与者使用自己的手机和App，捕捉到了最真实的数字行为模式。
*   **多模态同步**：首次公开结合了EEG、可穿戴眼动和外周生理信号的智能手机研究数据集。
*   **规范化程度高**：严格遵循BIDS标准，极大地降低了其他学者使用该数据的门槛。

### 8. 不足与局限
*   **样本量中等**：23名参与者的规模对于复杂的机器学习模型（如深度学习）可能略显不足。
*   **人群偏差**：参与者年龄集中在20-32岁，无法代表青少年或老年群体的智能手机使用习惯。
*   **应用类型局限**：虽然是“自由使用”，但大多数参与者选择了游戏或短视频，对于社交聊天、信息搜索等其他行为的覆盖可能不够均衡。
*   **环境限制**：虽然是自然交互，但在实验室环境下佩戴大量传感器（EEG帽、眼动眼镜）仍可能对用户的自然行为产生一定干扰。

（完）
