---
title: Task-optimized models of sensory uncertainty reproduce human confidence judgments
title_zh: 任务优化的感官不确定性模型再现人类置信判断
authors: "Govindarajan, L. N., Alavilli, S., McDermott, J. H."
date: 2026-06-24
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.31.685933v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 任务优化模型生成概率分布
tldr: 感官输入常含不确定性，人类如何表征并利用不确定性尚不明确。本研究开发任务优化模型，生成感知估计的概率分布以量化不确定性。通过对比人类信心判断与模型信心，发现在声音定位和音高感知中，人类信心随刺激变异性增加而降低，且与模型信心高度一致。这表明人类准确表征了感知不确定性，该框架可扩展至其他感知领域。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究人类是否及如何准确表征感官不确定性，并构建可计算模型以检验其规范性。
method: 开发任务优化模型输出概率分布，提取模型信心，并与人类信心判断进行跨条件比较。
result: 人类信心在声音定位和音高感知中随刺激变异性降低，且与模型信心高度相关。
conclusion: 人类不确定性判断反映实际感知不确定性，该建模框架可推广至多感知域。
---

## 摘要
感官输入通常具有模糊性，导致对外部世界的解释存在不确定性。对感知不确定性的估计可能有助于指导行为，但目前尚不清楚人类是否在自然情境中明确表示不确定性，以及任何此类表示是否符合规范正确性。由于缺乏估计不确定性的可计算刺激模型，进展受到阻碍。我们开发了一类任务优化模型，生成感知估计上的概率分布。为了评估人类不确定性表示是否与模型一致，我们将人类置信判断（可能间接反映不确定性表示）与从模型不确定性中提取的置信判断进行比较。在声音定位和音高感知中，人类置信度系统性地变化，对于产生更可变试验间估计的刺激，置信度更低。人类置信度在不同条件下跟踪模型置信度，表明人类不确定性表示准确反映了感知估计的实际不确定性。该建模框架可扩展到其他感知领域。

## Abstract
Sensory input is often ambiguous, leading to uncertain interpretations of the external world. Estimates of perceptual uncertainty might be useful in guiding behavior, but it remains unclear whether humans explicitly represent uncertainty in naturalistic settings, and whether any such representations are normatively correct. Progress has been hindered by the absence of stimulus-computable models that estimate uncertainty. We developed a class of task-optimized models that generate probability distributions over perceptual estimates. To assess whether human uncertainty representations align with the models, we compared human confidence judgments, which might indirectly reflect uncertainty representations, to confidence judgments extracted from the models uncertainty. In both sound localization and pitch perception, human confidence varied systematically, being lower for stimuli that produced more variable estimates across trials. Human confidence tracked model confidence across conditions, suggesting that human uncertainty representations accurately reflect the actual uncertainty of perceptual estimation. The modeling framework is extensible to other perceptual domains.