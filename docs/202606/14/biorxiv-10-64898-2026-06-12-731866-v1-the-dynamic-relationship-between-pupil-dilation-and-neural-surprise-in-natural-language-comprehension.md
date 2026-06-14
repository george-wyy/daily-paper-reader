---
title: The dynamic relationship between pupil dilation and neural surprise in natural language comprehension
title_zh: 自然语言理解中瞳孔扩张与神经惊奇的动态关系
authors: "Gehmacher, Q., Kaltenmaier, A., Schubert, J., Weisz, N., Press, C."
date: 2026-06-12
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.12.731866v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 使用瞳孔测量研究语言理解中的神经惊喜
tldr: 自然语言理解中，大脑如何区分持续预测与模型更新仍存争议。本研究结合MEG和瞳孔测量，用GPT-2量化词汇惊喜和语义误差，发现听觉皮层分级追踪词汇惊喜，而语义误差通过ReLU门控响应，仅当误差超过基线才触发。瞳孔和脑干主要反映门控响应，表明皮层与瞳孔-脑干系统在预测误差处理上存在功能分离，揭示了学习与感知的相互作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究大脑在自然语言理解中，预测误差的持续追踪与模型更新是否由不同计算机制实现。
method: 记录被试听自然语音时的MEG和瞳孔数据，用GPT-2逐词计算词汇惊喜和语义预测误差。
result: 听觉皮层分级编码词汇惊喜；语义误差通过门控响应驱动瞳孔和脑干，而非皮层。
conclusion: 皮层持续映射预测信息，而瞳孔-脑干系统选择性门控模型更新，两者计算解离。
---

## 摘要
预测处理理论认为，大脑会持续生成预测并根据误差信号更新内部模型，但目前尚不清楚预测表征和模型更新反映的是单一的分级计算，还是在可分离系统中实现的计算上不同的操作。我们记录了参与者在聆听连续自然语音时的脑磁图（MEG）和瞳孔测量数据，利用GPT-2模型逐词量化词汇惊奇和语义预测误差。总体而言，词汇惊奇主要以分级方式被追踪，而语义误差的反应则更好地由修正线性（ReLU）门控函数捕捉——即仅当误差超过近期上下文基线时才会响应。这些相对效应的强度也存在一些有趣的分离。听觉皮层以分级、连续的方式追踪词汇惊奇，而后的皮层阶段则反映语义误差。相比之下，强直性瞳孔直径和源定位的脑干反应主要由对语义误差的门控反应捕捉。瞳孔耦合分析证实，这种门控特征在瞳孔相关唤醒和脑干定位反应（而非皮层反应）之间具有统计共享性。这些发现共同揭示了一种分工模式：皮层维持着一个连续、高保真的预测信息地图，而瞳孔相关的模型更新系统则充当一个选择性门控，专门在跨越误差阈值的意义破坏事件中被激活。这种不对称性表明，服务于连续解析预测误差的信号和服务于模型修正的信号可能在计算上分离，这对我们理解服务于感知和学习的机制之间的内在互动具有一系列启示。

## Abstract
Predictive processing accounts hold that the brain continuously generates predictions and updates internal models from error signals, but it remains unclear whether prediction representation and model-updating reflect a single graded computation or computationally distinct operations implemented in dissociable systems. We recorded magnetoencephalography (MEG) and pupillometry while participants listened to continuous natural speech, quantifying word-by-word lexical surprise and semantic prediction error with a GPT-2 model. Broadly speaking, lexical surprise was tracked in a predominantly graded fashion, whereas the response to semantic error was better captured by a rectified linear (ReLU) gating function - i.e., that responds only when the error exceeds a recent contextual baseline. There were also some interesting dissociations in the strength of these relative effects. The auditory cortex tracked lexical surprise in a graded, continuous manner, with later cortical stages reflecting semantic error. By contrast, tonic pupil diameter and source-localised brainstem responses were predominantly captured by a gated response to semantic error. A pupil-coupling analysis confirmed that this gating signature was statistically shared between pupil-linked arousal and brainstem-localised, but not cortical, responses. Together, these findings reveal a division of labour in which the cortex maintains a continuous, high-fidelity map of predictive information while a pupil-linked model-update system acts as a selective gate, engaged specifically by meaning-disrupting events that have crossed a threshold level of error. This asymmetry suggests that signals serving continuous parsing of prediction error and signals serving model revision may be computationally dissociated, with a range of implications for our understanding of the intrinsic interactions between mechanisms serving perception and learning.