---
title: "A multimodal dataset of EEG, eye-tracking, and physiological signals during naturalistic smartphone interactions"
title_zh: 自然状态下智能手机交互过程中的脑电图、眼动追踪及生理信号多模态数据集
authors: "Mishra, P., Gandhi, T. K., Gandhi, S. R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719334v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 包含智能手机交互过程中眼动追踪和脑电的多模态数据集
tldr: 本研究发布了一个多模态生理数据集，记录了23名参与者在自然使用智能手机（如游戏或短视频）及随后放松状态下的生理反应。数据集涵盖了64通道EEG、眼动、PPG和GSR信号，并结合了手机成瘾量表评估。所有数据均通过TTL同步并遵循BIDS标准，为研究真实场景下智能手机交互的神经生理机制提供了重要资源。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决目前对自然状态下智能手机使用所关联的神经生理动态特征研究不足的问题。
method: 采集了受试者在操作常用APP及观看放松视频时的多模态生理信号，并收集了手机成瘾相关量表数据。
result: 成功构建并公开了一个经过精确同步、符合BIDS规范的多模态生理信号数据集。
conclusion: 该数据集为深入分析不同手机使用行为下的神经、眼动及自主神经响应提供了具有生态效度的科研支持。
---

## 摘要
智能手机已成为通信、信息消费和数字交互的普及工具，但与自然状态下智能手机使用相关的神经生理动力学特征尚未得到充分描述。在此，我们展示了一个在具有生态效度的智能手机交互及随后的放松状态下收集的多模态生理数据集。23名参与者使用其最常用的智能手机应用程序（主要是游戏或短视频）10分钟，随后被动观看5分钟的标准自然视频。研究同步记录了脑电图（EEG；64通道）、可穿戴眼动追踪、光电容积脉搏波（PPG）和皮肤电反应（GSR）传感器的信号。此外，还收集了包括智能手机成瘾量表（SAS）和手机问题使用量表（MPPUS）在内的问卷评估，以表征智能手机相关行为特征的个体差异。所有数据流均使用晶体管-晶体管逻辑（TTL）触发信号进行同步，以确保跨模态的精确时间对齐。该数据集根据脑成像数据结构（BIDS）规范进行组织，并已在 OpenNeuro 上公开（获取编号：ds007537）。该数据集有助于研究智能手机交互过程中的神经、眼动和自主神经反应，并在保持生态效度的同时支持对多种智能手机行为的多模态分析。

## Abstract
Smartphones have become pervasive tools for communication, information consumption, and digital interaction, yet the neurophysiological dynamics associated with naturalistic smartphone use remain insufficiently characterized. Here, we present a multimodal physiological dataset collected during ecologically valid smartphone interaction and a subsequent relaxation condition. Twenty-three participants engaged with their most frequently used smartphone application (primarily gaming or short form video) for ten minutes, followed by a five-minute passive viewing of a standardized nature video. Simultaneous recordings were obtained from electroencephalography (EEG; 64 channels), wearable eye-tracking, photoplethysmography (PPG), and galvanic skin response (GSR) sensors. Questionnaire-based assessments, including the smartphone addiction scale (SAS) and the mobile phone problematic use scale (MPPUS), are also collected to characterize individual differences in smartphone-related behavioral traits. All data streams are synchronized using transistor-transistor logic (TTL) trigger signals to ensure precise temporal alignment across modalities. The dataset is organized according to the Brain Imaging Data Structure (BIDS) specification and is publicly available on OpenNeuro (Accession Number: ds007537). This dataset enables the investigation of neural, ocular, and autonomic responses during smartphone interaction and supports multimodal analysis of diverse smartphone behaviors while preserving ecological validity.