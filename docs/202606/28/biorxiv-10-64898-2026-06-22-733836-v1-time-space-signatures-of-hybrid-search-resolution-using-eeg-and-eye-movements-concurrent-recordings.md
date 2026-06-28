---
title: Time space signatures of hybrid search resolution using EEG and eye movements concurrent recordings
title_zh: 利用脑电图和眼动同步记录的混合搜索解决的时间空间特征
authors: "Care, D., Gonzalez, J. E., Ison, M. J., Kamienkowski, J. E."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733836v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 同步脑电与眼动数据的去卷积方法，其多模态解析思路可用于意图预测
tldr: 自然场景下的视觉搜索需要注意力和记忆协同，传统事件相关方法难以分离时间重叠的神经响应。本文采用基于去卷积的方法处理同步EEG和眼动数据，在混合搜索任务中提取精细的时间响应函数，成功复现了P300等经典成分，并揭示了漏检响应。该方法结合模型性能评估和方差膨胀因子，能够稳健地探索多变量交互，为理解自由观看行为下的注意力-记忆动态交互提供了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统事件相关方法无法分离自然场景中视觉搜索重叠的神经信号，阻碍生态效度研究。
method: 使用去卷积方法分析同步记录的EEG和眼动数据，建立层级模型提取时间响应函数。
result: 复现P300成分，发现漏检引发类似但更弱响应；模型性能随复杂度提升而稳定。
conclusion: 去卷积法结合模型评估可揭示自由观看中注意力与记忆的动态交互。
---

## 摘要
理解大脑如何在自然环境中支持视觉搜索——其中注意力和记忆必须协同工作以在干扰物中找到目标——需要分析神经信号，其中响应在时间上重叠且多个环境变量同时相互作用。传统的与事件相关的方法无法分离这些重叠信号，这为在生态有效环境中研究认知造成了根本性的瓶颈。在这里，我们试图在自然场景下的混合视觉和记忆搜索任务中隔离激活模式。我们表明，我们基于反卷积的方法应用于共配准的脑电图和眼动追踪数据解决了这一问题，捕获了时间响应函数（TRF）中主效应及其相互作用的精细激活模式。从假设驱动模型开始，我们在无限制眼动的混合搜索任务中复制了已建立的视觉处理和目标检测成分。此外，将我们的方法扩展到层次更大的数据驱动模型使我们能够探索效应之间的相互作用，而这些效应此前是分别研究的。我们表明，TRF估计值随着模型复杂度的增加而保持稳定，这得益于模型性能的改善（皮尔逊相关系数）并由方差膨胀因子（VIF）控制。我们识别出一个与目标检测P300成分一致的晚期激活，并揭示漏检引发了相似但较弱的响应，表明其作用比简单检测更为微妙。这些发现证明了反卷积方法如何——辅以支持其在特征空间扩展的稳健模型性能度量——揭示自由观看行为背后注意力与记忆过程的动态相互作用。

## Abstract
Understanding how the brain supports visual search in naturalistic environments, where attention and memory must work together to find targets among distractors, requires analysing neural signals where responses overlap in time and multiple environmental variables simultaneously interact. Conventional event-related methods cannot disentangle these overlapping signals, creating a fundamental bottleneck for studying cognition in ecologically valid settings. Here, we seek to isolate activation patterns during a hybrid visual and memory search task in naturalistic scenarios. We show that our deconvolution-based approach applied to coregistered EEG and eye-tracking data resolves this problem, capturing fine grained activation patterns in the temporal response functions (TRFs) for main effects and their interactions. Starting from hypothesis driven models, we replicated established components for visual processing and target detection in a Hybrid Search task with unrestricted eye movements. Moreover, extending our approach to hierarchically larger data-driven models enabled us to explore interactions between the effects that have otherwise been studied separately. We showed that the TRF estimates remained stable with increasing model complexity, supported by improved model performance (Pearson s correlation coefficient) and controlled by the variance inflation factor (VIF). We identified a late activation consistent with the P300 component for target detection, and revealed that missed detections elicited similar but weaker responses, suggesting a more nuanced role than simple detection. These findings demonstrate how deconvolution methods, complemented with robust measures of model performance that support its expansion in features space, can uncover the dynamic interplay of attention and memory processes underlying free-viewing behavior.