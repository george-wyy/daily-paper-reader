---
title: "HSSM: A Widely Applicable Toolbox for Hierarchical Bayesian Neuro-cognitive Modeling"
title_zh: HSSM：一个广泛适用的分层贝叶斯神经认知建模工具箱
authors: "Fengler, A., Xu, Y., Bera, K., Paniagua, C., Omar, A., Frank, M. J."
date: 2026-06-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730398v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 层级贝叶斯工具箱可应用于眼动数据的概率建模，支持前瞻性系统开发
tldr: 认知神经科学的计算模型分析常局限于少数解析可解的规范模型。HSSM工具箱基于层次贝叶斯推理，通过似然替代的模拟推理实现任意过程模型的参数估计。用户可使用类似公式的语法指定混合效应回归，并纳入神经协变量。该工具加速模型开发到实证检验的循环，促进社区共享。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有方法限制了可应用的模型种类，阻碍了复杂认知模型的实证验证。
method: 采用模拟推理和层次贝叶斯框架，利用PyMC与Bambi构建似然替代网络。
result: 支持快速参数估计、混合效应回归及神经协变量，并通过HuggingFace部署模型。
conclusion: HSSM桥接计算理论与实验研究，推动认知神经科学建模的民主化与可重复性。
---

## 摘要
计算模型是认知神经科学的核心，但其在实验数据集中的严谨应用往往受限于少数能够进行易处理分析计算的经典模型。我们介绍了HSSM（分层序列抽样模型）生态系统，这是一个Python工具箱，通过分层贝叶斯推断，使广泛、可扩展的神经认知过程模型变得易于使用。通过似然代理自然地利用基于模拟的推断，HSSM能够为缺乏封闭形式似然的模型进行快速参数估计。HSSM基于PyMC和Bambi构建，提供用户友好的公式语法，用于指定模型参数上的分层混合效应回归，并可纳入逐试次的神经或生理协变量。该生态系统支持快速模型模拟和训练数据生成，以及用于通过HuggingFace部署代理似然网络的神经网络训练工具。本工作的贡献旨在不仅惠及从事特定问题的单一研究者，而且自然地惠及整个研究社区。HSSM生态系统中的工具共同弥合了计算理论家和实验者的兴趣，加速了从模型开发到严格实证测试的循环。

## Abstract
Computational models are central to cognitive neuroscience, but their rigorous application to experimental datasets is often constrained to a narrow set of canonical models that afford tractable analytical computations. We introduce the HSSM (Hierarchical Sequential Sampling Model) ecosystem, a Python toolbox that democratizes access to a broad, extensible array of neuro-cognitive process models through hierarchical Bayesian inference. Naturally leveraging simulation-based inference via likelihood surrogates, HSSM enables fast parameter estimation for models lacking closed-form likelihoods. Built atop PyMC and Bambi, HSSM provides a user-friendly formula syntax for specifying hierarchical mixed-effects regressions on model parameters, incorporating trial-by-trial neural or physiological covariates. The ecosystem allows fast model simulation and training data generation, as well as the neural network training utilities to deploy surrogate likelihood networks via HuggingFace. Contributions are designed to benefit not only the single researcher working on a problem, but organically, the entire research community. Together, the tools in the HSSM ecosystem bridge the interests of computational theorists as well as experimentalists, accelerating the cycle from model development to rigorous empirical testing.