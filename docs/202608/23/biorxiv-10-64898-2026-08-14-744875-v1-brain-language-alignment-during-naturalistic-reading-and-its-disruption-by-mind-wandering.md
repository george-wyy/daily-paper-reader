---
title: Brain-Language Alignment During Naturalistic Reading and Its Disruption by Mind-Wandering
title_zh: 自然阅读过程中的大脑-语言对齐及其走神干扰
authors: "Sun, H., Jangraw, D. C."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.14.744875v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 同时使用脑电和眼动追踪预测走神状态，可迁移至多模态意图预测
tldr: 以往脑-语言对齐的EEG证据多来自受控逐词阅读，自然阅读下是否可检测以及注意波动的影响未知。本研究基于ROAMM数据集，用岭回归编码模型预测注视对齐的EEG谱功率与FRP，比较五种词嵌入。结果表明上下文嵌入优于静态，谱对齐主要在alpha/低beta频段，FRP对齐在200-300ms，而心智游移期间对齐显著降低，对振荡特征影响更明显。这证明自然阅读中语言模型表征可被EEG可靠反映，注意波动是编码研究的重要变异来源。
source: biorxiv
selection_source: fresh_fetch
motivation: 先前EEG脑-语言对齐证据多来自受控逐词范式，自然阅读下可检测性及受心智游移影响未知。
method: 利用ROAMM多模态数据，训练岭回归编码模型预测注视对齐EEG谱功率与FRPs，比较静态与上下文嵌入。
result: 可靠对齐出现，上下文嵌入更优；谱对齐在alpha/低beta，FRP在200-300ms；心智游移降低对齐，振荡特征更明显。
conclusion: 自然阅读EEG可编码语言模型表征，注意波动构成脑-语言编码研究的重要变异源。
---

## 摘要
编码模型为将语言的计算表征与神经活动联系起来提供了一个原则性框架，但大多数关于大脑-语言对齐的脑电图（EEG）证据来自严格控制、逐词阅读的范式。这种对齐在自然阅读过程中是否可检测，以及它如何受到注意力缺失的影响，仍不清楚。我们利用ROAMM数据集解决了这些问题，该多模态数据集包含44名参与者阅读自然文本时的同步EEG和眼动记录，以及时间分辨的走神（MW）注释。我们使用岭回归编码模型，从五种词嵌入模型（GloVe、word2vec、BERT、GPT-2和Llama 3）预测注视对齐的EEG频谱功率和注视相关电位（FRP）。通过置换检验并进行错误发现率校正，我们发现两种特征类型均存在统计上可靠的大脑-语言对齐，且上下文嵌入优于静态嵌入。频谱对齐在顶叶电极的alpha和低beta频段最强，而基于FRP的对齐在注视开始后200–300毫秒于中央和顶枕区域达到峰值。利用ROAMM的跨度级MW注释，我们进一步表明，大脑-语言对齐在走神期间系统性减弱，且这种效应在振荡（PSD）特征上远大于事件相关（FRP）特征。这些发现表明，尽管该模态存在固有噪声，现代语言模型表征仍可反映在自然阅读过程中的EEG活动中，且注意力波动构成了大脑-语言编码研究中一个未被充分认识的变异来源。

## Abstract
Encoding models offer a principled framework for linking computational representations of language to neural activity, but most electroencephalography (EEG) evidence for brain--language alignment comes from tightly controlled, word-by-word reading paradigms. Whether such alignment is detectable during naturalistic reading, and how it is affected by lapses in attention, remains unclear. We addressed these questions using ROAMM, a multimodal dataset containing simultaneous EEG and eye-tracking recordings with time-resolved mind-wandering (MW) annotations from 44 participants reading naturalistic texts. Ridge regression encoding models were trained to predict fixation-aligned EEG spectral power and fixation-related potentials (FRPs) from five word-embedding models (GloVe, word2vec, BERT, GPT-2, and Llama 3). Using permutation testing with false discovery rate correction, we found statistically reliable brain--language alignment across both feature types, with contextual embeddings outperforming static embeddings. Spectral alignment was strongest in the alpha and low-beta bands over parietal electrodes, while FRP-based alignment peaked 200--300 ms after fixation onset over central and parietal-occipital regions. Leveraging ROAMM's span-level MW annotations, we further show that brain--language alignment is systematically reduced during MW, an effect that was substantially larger for oscillatory (PSD) than for event-related (FRP) features. These findings demonstrate that modern language-model representations are reflected in EEG activity during naturalistic reading despite the modality's inherent noise, and that fluctuations in attention constitute an underappreciated source of variability in brain--language encoding studies.