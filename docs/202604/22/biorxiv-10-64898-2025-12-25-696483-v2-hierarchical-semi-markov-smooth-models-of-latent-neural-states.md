---
title: Hierarchical Semi-Markov Smooth Models of Latent Neural States
title_zh: 潜神经状态的分层半马尔可夫平滑模型
authors: "Krause, J., van Rij, J., Borst, J. P."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.25.696483v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 基于神经生理信号的潜在认知过程概率建模
tldr: 本研究针对隐半马尔可夫模型（HsMM）在处理神经生理信号时无法兼顾个体差异和实验协变量非线性影响的问题，提出了一种层次化半马尔可夫平滑模型框架。该框架通过混合加法模型替代传统参数，引入平滑函数和随机效应，并支持经验贝叶斯和全贝叶斯推断。在词汇决策数据集上的应用表明，该模型能更准确地捕捉个体差异并重新评估认知过程的划分，为认知神经科学提供了更灵活的建模工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的隐半马尔可夫模型难以处理受试者间的异质性以及实验协变量对认知过程产生的非线性影响。
method: 提出一种将HsMM参数替换为包含平滑函数和随机效应的混合加法模型的层次化建模框架，并实现贝叶斯推断算法。
result: 在词汇决策任务的应用中发现，不同受试者对认知过程的依赖程度不同，且两个预设的半马尔可夫状态可能对应同一认知过程。
conclusion: 该层次化平滑模型框架显著提升了神经信号建模的灵活性和准确性，有助于更深入地理解复杂的认知动态。
---

## 摘要
隐（半）马尔可夫模型（HsMMs）正越来越多地被用于将神经生理信号分割成潜在认知过程的序列。其核心思想是：不同的过程会在（多变量）神经生理信号的试次级记录中留下独特的痕迹。配备了这些痕迹的发射模型以及描述任务中涉及的不同潜在过程进展的潜在过程模型后，马尔可夫模型可用于推断任何时间点和试次中最可能的过程。然而，目前使用的 HsMMs 在两个重要方面仍存在局限。首先，它们无法解释潜在过程和发射过程中的受试者间异质性；相反，通常假设一个单一的群体级模型来解释所有数据。其次，它们无法解释实验协变量对潜在过程和发射过程可能产生的非线性影响。为了解决这些问题，我们提出了一个建模框架，其中发射和潜在过程的 HsMM 参数被替换为混合加性模型，包括实验协变量的平滑函数和随机效应。我们推导了所有参数的经验贝叶斯和全贝叶斯推理所需的所有量，并提供了所有估计算法的 Python 实现。为了展示该框架的优势，我们将这种多层模型应用于现有的词汇决策数据集。我们表明，即使在这样一个简单的任务中，并非所有受试者都同等地依赖相同的过程，而且至少有两个以前被认为反映不同过程的半马尔可夫状态，实际上可能与同一个认知过程相关。

## Abstract
Hidden (semi-) Markov Models (HsMMs) are increasingly being used to segment neurophysiological signals into sequences of latent cognitive processes. The idea: different processes will leave distinct traces in trial-level recordings of (multivariate) neuro-physiological signals. Markov models, equipped with an emission model of these traces and a latent process model describing the progression through the different latent processes involved in a task, can then be used to infer the most likely process for any time-point and trial. However, the currently used HsMMs remain limited in two important ways. First, they cannot account for subject-level heterogeneity in the latent and emission process. Instead, a single group-level model is assumed to explain the entire data. Second, they cannot account for the potentially nonlinear effects of experimental covariates on the latent and emission process. To address these problems, we present a modeling framework in which the HsMM parameters of the emission and latent process are replaced with mixed additive models, including smooth functions of experimental covariates and random effects. We derive all necessary quantities for empirical Bayes and fully Bayesian inference for all parameters and provide a Python implementation of all estimation algorithms. To demonstrate the advantages offered by this framework, we apply such a multi-level model to an existing lexical decision dataset. We show that, even in such a simple task, not all subjects rely on the same processes equally and that at least two semi-Markov states, previously believed to reflect distinct processes, might actually relate to the same cognitive process.