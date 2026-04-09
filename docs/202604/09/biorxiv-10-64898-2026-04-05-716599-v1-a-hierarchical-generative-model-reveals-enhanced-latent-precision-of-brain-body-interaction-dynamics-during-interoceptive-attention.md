---
title: A hierarchical generative model reveals enhanced latent precision of brain-body interaction dynamics during interoceptive attention
authors: "Shinagawa, K., Idei, H., Umeda, S., Yamashita, Y."
date: 2026-04-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.05.716599v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 用于连续多模态动态和脑机交互的层次化生成模型
tldr: 本研究针对脑体相互作用（BBI）动态难以提取的问题，提出了一种基于预测编码的层次化生成模型（PV-RNN）。通过分析33名受试者在内感受注意任务下的EEG、ECG和呼吸数据，模型成功捕捉了多尺度、非线性的双向耦合动态。研究发现，内感受注意显著增强了多模态关联层的潜在精度，且该增强程度与个体的身体控制感及心理健康指标密切相关，为理解脑体交互提供了新的计算框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统的脑体相互作用研究多为观察性，缺乏能够整合多模态连续动态的生成式建模框架。
method: 采用受预测编码启发的变分循环神经网络（PV-RNN）对同步采集的EEG、ECG和呼吸序列进行层次化建模。
result: 模型中间关联层在内感受注意期间表现出显著增强的潜在精度，且该指标与主观身体控制感正相关，与焦虑等精神脆弱性负相关。
conclusion: 层次化生成模型为提取连续脑体交互动态提供了可解释的框架，并揭示了内感受注意的潜在生理特征及其临床意义。
---

## Abstract
Brain-body interactions (BBIs) are fundamental to cognition and mental health, but their continuous multimodal dynamics remain difficult to extract. Previous approaches have been largely observational, and few frameworks enable these interacting processes to be modeled within an integrated generative system. Here, we applied a Predictive-Coding-Inspired Variational RNN (PV-RNN) to simultaneous EEG, ECG, and respiration recordings obtained from 33 participants during exteroceptive and interoceptive attention. The model learned a temporal hierarchy spanning modality-specific dynamics, multimodal associative integration, and sequence-level global states, and accurately reconstructed unseen physiological sequences. Specifically, the intermediate associative layer successfully captured the core complexities of BBI by extracting multiscale, nonlinear, and bidirectional coupling dynamics with variable temporal lags. Furthermore, the estimated precision (inverse variance) of latent variables representing BBI dynamics within this multimodal associative layer increased significantly during interoceptive attention. The magnitude of this condition-dependent precision enhancement correlated positively with subjective adaptive body controllability and negatively with psychiatric vulnerabilities, including rumination and trait anxiety. These findings identify a latent physiological signature of interoceptive attention and establish hierarchical generative modeling as an interpretable framework for extracting continuous BBI dynamics and linking multimodal physiology to cognitive and clinical characteristics.