---
title: Effect of Large Language Models on P300 Speller Performance with Cross-Subject Training
title_zh: 大语言模型对跨被试训练下 P300 拼写器性能的影响
authors: "Parthasarathy, N., Soetedjo, J., Panchavati, S., Lee, D., Arnold, C., Pouratian, N., Speier, W."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.28.685216v2.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 大语言模型辅助的脑机接口通信意图预测
tldr: 本研究针对P300拼写器速度慢且需个体校准的局限，提出了一种结合大语言模型（LLM）与跨被试训练的系统性分析框架。通过对78名受试者的EEG数据进行仿真，评估了多种LLM及理想化模型的性能上限。研究发现，LLM能显著提升打字速度，且多种模型性能已接近理论极限，表明未来BCI性能提升的关键将从语言建模转向神经信号解码。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决P300拼写器打字速度慢和对特定受试者校准依赖性强的问题，并探索LLM提升性能的理论上限。
method: 采用多模型理论分析框架，结合多种LLM、理想化模型及跨被试分类器训练，在78名受试者的数据集上进行仿真实验。
result: "LLM辅助使跨被试和被试内训练的打字速度分别提升约40%和75%，且现有模型性能已达到理论上限的5%以内。"
conclusion: 研究证明LLM能显著优化BCI通信，并指出当前性能瓶颈已从语言模型建模转移到了神经信号解码环节。
---

## 摘要
肌萎缩侧索硬化症（ALS）是一种进行性神经退行性疾病，严重损害沟通能力，需要辅助技术来恢复交互。P300 拼写器脑机接口（BCI）通过将脑电图（EEG）响应转化为文本来实现通信；然而，由于打字速度慢和需要针对特定被试进行校准，其实际应用受到了限制。最近的研究表明，大语言模型（LLMs）（如 GPT-2）可以通过预测单词显著提高 P300 拼写器的性能。然而，目前尚不清楚这些增益是特定于模型的，还是代表了语言模型中的一种普遍趋势。此外，在统一的解码框架内，LLM 辅助的 P300 拼写器的基本性能极限尚未得到系统表征。在本研究中，我们通过一个系统的多模型理论分析框架解决了这些空白。我们评估了广泛的语言模型，并引入了一个理想化的 LLM 以建立可实现性能的上限。此外，我们结合了跨被试分类器训练以减少校准需求，并评估了跨被试的泛化能力。通过对 78 名被试的 EEG 数据进行广泛模拟，我们证明了所评估的模型在打字速度上一致实现了实质性提升，与传统方法相比，增益分别高达约 40%（跨被试训练）和约 75%（被试内训练）。更重要的是，我们表明尽管架构存在差异，多个模型在理论性能极限的 5% 以内运行，这表明进一步扩大模型规模带来的收益正在递减。这些改进在被试内和跨被试分类器中均具有泛化性。我们的结果表明，在所考虑的解码框架内，LLM 辅助的 P300 拼写器正接近其基本性能极限，主要瓶颈已从语言建模转向神经信号解码。这项工作既为改进 BCI 通信提供了一个实用框架，也为其可实现的极限提供了理论视角。

## Abstract
Amyotrophic lateral sclerosis (ALS), a progressive neurodegenerative disease, severely impairs communication, requiring assistive technologies that restore interaction. The P300 speller brain-computer interface (BCI) enables communication by translating EEG responses into text; however, its practical adoption is limited by slow typing speed and the need for subject-specific calibration. Recent work has demonstrated that large language models (LLMs), such as GPT-2, can significantly improve the performance of the P300 speller by predicting words. However, it remains unclear whether these gains are model-specific or represent a broader trend across language models. Furthermore, the fundamental performance limits of LLM-assisted P300 spellers have not been systematically characterized within a unified decoding framework. In this study, we address these gaps through a systematic multi-model theoretical analysis framework. We evaluate a wide range of language models and introduce an idealized LLM to establish upper bounds on achievable performance. In addition, we incorporate cross-subject classifier training to reduce calibration requirements and assess generalization across subjects. Using extensive simulations on EEG data from 78 subjects, we demonstrate that the evaluated models consistently achieve substantial improvements in typing speed, with gains of up to [~]40% (across-subject training) and [~]75% (within-subject training) over conventional approaches. More importantly, we show that multiple models, despite architectural differences, operate within 5% of the theoretical performance bound, indicating diminishing returns from further model scaling. These improvements generalize across both within-subject and across-subject classifiers. Our results suggest that LLM-assisted P300 spellers are approaching their fundamental performance limits within the considered decoding framework, shifting the primary bottleneck from language modeling to neural signal decoding. This work provides both a practical framework for improving BCI communication and a theoretical perspective on its achievable limits.