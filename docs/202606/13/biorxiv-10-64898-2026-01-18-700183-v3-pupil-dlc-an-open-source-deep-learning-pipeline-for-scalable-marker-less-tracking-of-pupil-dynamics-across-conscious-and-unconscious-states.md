---
title: "Pupil-DLC: an open-source deep learning pipeline for scalable, marker-less tracking of pupil dynamics across conscious and unconscious states"
title_zh: Pupil-DLC：一个开源深度学习流水线，用于跨意识与无意识状态的可扩展、无标记瞳孔动态追踪
authors: "Seyfourian, P., Marks, L. C., Claar, L. D., Nahas, Y., Keating, M., Koch, C., Rembado, I."
date: 2026-06-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.18.700183v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 开源瞳孔追踪流水线，眼动追踪数据
tldr: 现有瞳孔追踪工具难以兼顾可扩展性与鲁棒性。本文提出基于DeepLabCut的开源管道Pupil-DLC，用21750帧小鼠视频训练，采用通用与个体模型双架构，精准追踪清醒、药物诱导等状态下的瞳孔动态。在老鼠和人类视频中均优于现有方法，帧保留率高且计算高效，为脑状态研究提供可复现平台。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有瞳孔检测软件缺乏跨物种、跨实验条件的鲁棒性和可扩展性，亟需一个适应多种脑状态的通用框架。
method: "构建包含21,750标注帧的数据集，训练DeepLabCut双模型（通用模型用于高通量，个体模型用于会话优化），捕捉瞳孔形状变化与伪影。"
result: 在清醒、致幻剂、麻醉等状态下追踪准确率优于现有工具，帧保留率高；无需重新训练即可泛化到人类白天/智能手机视频。
conclusion: Pupil-DLC提供可复现、多物种适用的瞳孔动力学量化工具，桥接基础小鼠神经科学与人类转化研究。
---

## 摘要
背景：瞳孔直径是脑状态的非侵入性生物标志物，与觉醒、注意、认知加工和意识相关。然而，现有的瞳孔测量软件在多样实验条件和物种中通常缺乏可扩展性和鲁棒性。新方法：我们介绍Pupil-DLC，一个基于DeepLabCut的开源离线流水线，用于可扩展、无标记的瞳孔追踪，主要针对小鼠设计。该流水线在来自超过140个头部固定小鼠视频的21,750张手动标注帧上训练，这些视频涵盖清醒和药物诱导状态（包括致幻剂和麻醉），数据集特意选择以最大化瞳孔大小变异性和模型泛化能力。Pupil-DLC实现了一种双模型架构：用于高通量分析的通用模型（GM）和用于会话特定优化的个体模型（IM）。结果：Pupil-DLC在清醒、致幻剂和麻醉状态下捕捉瞳孔动态，与真实值高度一致，并且在主动运动和安静休息期间具有相同的追踪保真度。置信度指标与人工帧质量评估一致，实现了准确性-保留权衡的原则性调整。作为次要演示，Pupil-DLC无需重新训练即可扩展到未见的人类视频，涵盖不同条件和帧率，包括日光和智能手机记录。与现有方法比较：Pupil-DLC在准确性和帧保留方面优于现有自动化方法，同时保持与实时工具相当的计算效率。这些改进源于基于学习的关键点表示，对瞳孔形状变化、遮挡、反射和成像伪影具有鲁棒性。GM/IM框架支持一种平衡通量和精度的分层策略。结论：Pupil-DLC提供了一个可重复、可适应的平台，用于跨实验范式和物种量化与瞳孔相关的脑状态动态，桥接了基础小鼠神经科学和转化人类应用。

## Abstract
Background: Pupil diameter is a non-invasive biomarker of brain state, correlating with arousal, attention, cognitive processing, and consciousness. However, existing pupillometry software often lacks scalability and robustness across diverse experimental conditions and species. New method: We introduce Pupil-DLC, an open-source, offline, DeepLabCut-based pipeline for scalable, marker-less pupil tracking, primarily designed for mice. Trained on 21,750 manually annotated frames from over 140 videos of head-fixed mice spanning wakefulness and drug-induced states, including psychedelics and anesthesia, the dataset was deliberately selected to maximize pupil size variability and model generalization. Pupil-DLC implements a dual-model architecture: a General Model (GM) for high-throughput analysis and an Individual Model (IM) for session-specific optimization. Results: Pupil-DLC captures pupil dynamics across awake, psychedelic, and anesthetized conditions with high agreement with ground truth and equal tracking fidelity during active locomotion and quiet rest. Confidence metrics aligned with human frame quality assessments, enabling principled tuning of accuracy-retention trade-offs. As a secondary demonstration, Pupil-DLC extends to unseen human videos across diverse conditions and frame rates, including daylight and smartphone recordings, without retraining. Comparison with existing methods: Pupil-DLC outperforms existing automated methods in accuracy and frame retention while maintaining computational efficiency comparable to real-time tools. These improvements stem from a learned keypoint-based representation robust to pupil shape variability, occlusions, reflections, and imaging artifacts. The GM/IM framework supports a tiered strategy balancing throughput and precision. Conclusions: Pupil-DLC provides a reproducible, adaptable platform for quantifying pupil-linked brain state dynamics across experimental paradigms and species, bridging basic mouse neuroscience and translational human applications.