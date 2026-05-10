---
title: Multi-modal Ensemble Approach for Decoding Player Intentions in Table Tennis
title_zh: 乒乓球运动中解码选手意图的多模态集成方法
authors: "Pham, T. Q., Funai, S. S., Kanai, R., Chikazoe, J."
date: 2026-05-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.04.721564v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.5
evidence: 利用姿态和脑电信号进行玩家意图的多模态解码
tldr: 本研究旨在通过脑电图（EEG）和姿态特征预测乒乓球运动员的击球意图。研究利用公开数据集，针对9名球员开发了基于SGD的姿态分类器和基于EEGNet的脑电分类器。结果显示，脑电信号在击球前500毫秒即可提供预测信息，而姿态特征在100毫秒时效果最佳。通过多模态集成方法，模型在预测左右进攻意图上达到了0.563的F1分数，优于单一模态，为神经假体和运动训练工具提供了新思路。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探索在乒乓球等高强度运动中，如何结合脑电信号和身体姿态提前准确预测运动员的击球意图。
method: 采用基于随机梯度下降的姿态分类器和改进的EEGNet脑电分类器，并构建多模态集成模型进行意图识别。
result: 多模态集成模型的平均F1分数达到0.563，表现优于单一的姿态（提升0.03）或脑电（提升0.02）分类器。
conclusion: 研究证明了结合脑电与姿态的多模态方法在运动意图解码中的有效性，具有应用于神经假体和运动反馈训练的潜力。
---

## 摘要
本研究旨在预测剧烈运动过程中的人类意图，特别是乒乓球运动。利用包含同步脑电图（EEG）和视频记录的公开“真实世界乒乓球数据集”（Real World Table Tennis dataset），我们基于姿态特征和脑电信号，为九名选手（7名男性，2名女性；年龄范围18-30岁）开发了一系列针对特定参与者的分类器。基于姿态的分类器采用了带有逻辑损失的随机梯度下降模型，而基于脑电的分类器则采用了改进的卷积神经网络架构（EEGNet）。两种分类器均成功地从球拍触球前的时间窗口预测了左右进攻意图，其中姿态特征的最佳解码时间点为-100毫秒，脑电信号为-500毫秒。基于脑电的解码性能优于基于姿态的解码，而多模态集成进一步提升了预测效果，平均宏F1分数达到0.563（自助法95%置信区间：0.523-0.603），相比仅使用姿态和仅使用脑电的分类器分别提升了0.03和0.02。由于每个分类器都是独立训练的，该集成模型在未来可以可行地扩展以纳入更多模态。这些结果表明，该方法在神经假体系统和体育训练的神经反馈工具中具有潜在的应用前景。

## Abstract
This study aims to predict human intentions during intense sports activities, specifically in table tennis. Using a publicly available Real World Table Tennis dataset containing simultaneous EEG and video recordings, we developed a series of participant-specific classifiers for nine players (7 males and 2 females; age range 18-30), based on pose features and EEG signals. The pose-based classifier used a stochastic gradient descent model with logistic loss, whereas the EEG-based classifier employed a modified convolutional neural network architecture (EEGNet). Both classifiers successfully predicted left-right attack intentions from the time windows preceding racket-ball impact, with optimal decoding occurring at -100 ms for pose features and -500 ms for EEG signals. EEG-based decoding achieved higher performance than pose-based decoding, and a multi-modal ensemble further improved prediction, reaching a mean macro F1 score of 0.563 (bootstrapped 95% CI: 0.523-0.603), corresponding to gains of +0.03 over pose-only and +0.02 over EEG-only classifiers. Because each classifier is trained independently, the ensemble can be feasibly extended to incorporate additional modalities in the future. These results suggest potential applications in neural prosthetic systems and neurofeedback tools for sports training.