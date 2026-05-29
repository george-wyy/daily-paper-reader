---
title: Quantifying uncertainty in drift diffusion models of decision making under temporal dependence and parameter variability
title_zh: 量化时间依赖与参数变异性下决策漂移扩散模型的不确定性
authors: "Riegner, G., Schwartzman, A., Reinagel, P."
date: 2026-05-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.17.722295v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 决策的概率建模，不确定性量化
tldr: 决策行为存在时间相关性和非平稳性，现有漂移扩散模型（DDM）拟合方法忽视不确定性或假设独立常参数。本文提出一种计算高效的解析不确定性估计方法，对时间依赖和参数变化鲁棒，并通过协变量显式建模非平稳性。在大鼠二选一视觉任务中，该方法揭示了多时间尺度的动态决策状态。本研究为DDM参数估计提供了可靠的不确定性量化，并附有Python实现。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有DDM估计方法忽视时间依赖和参数变化，导致不确定性被低估。
method: 提出解析不确定性估计方法，鲁棒处理时间依赖和未建模参数变化，协变量建模非平稳性。
result: 应用于大鼠视觉任务，揭示多时间尺度动态决策状态。
conclusion: 该方法提供可靠的不确定性量化，提升决策模型推断的准确性。
---

## 摘要
决策行为随时间变化，表现出时间相关性和非平稳性。现有的漂移扩散模型（DDM）拟合方法要么无法为参数估计提供不确定性量化，要么依赖于决策独立且参数随时间恒定不变的 restrictive 假设，这可能低估不确定性。为解决这些局限，我们提出了一种计算高效的方法，用于估计DDM参数的分析不确定性，该方法对时间依赖和未建模的参数变异性具有鲁棒性，同时通过协变量显式建模非平稳变异性。我们将该方法应用于大鼠在二选一强制选择（2AFC）视觉任务中的决策，揭示了多个时间尺度上的动态决策状态。提供了该方法的Python实现。

## Abstract
Decision-making behavior changes over time, exhibiting temporal correlation and nonstationarity. Existing drift diffusion model (DDM) fitting methods either do not provide uncertainty quantification for parameter estimates, or rely on restrictive assumptions that decisions are independent and that parameters remain constant over time, potentially underestimating uncertainty. To address these limitations, we propose a computationally efficient method for estimating analytic uncertainties in DDM parameters that are robust to temporal dependence and unmodeled parameter variability, while explicitly modeling nonstationary variability through covariates. We apply this method to rat decision-making in a two-alternative forced-choice (2AFC) visual task, revealing dynamic decision-making states across multiple timescales. A Python implementation of the method is provided.