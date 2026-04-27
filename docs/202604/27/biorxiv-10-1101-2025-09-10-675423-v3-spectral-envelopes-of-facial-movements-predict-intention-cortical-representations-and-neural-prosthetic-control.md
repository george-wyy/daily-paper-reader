---
title: "Spectral envelopes of facial movements predict intention, cortical representations, and neural prosthetic control"
title_zh: 面部运动的光谱包络可预测意图、皮层表征和神经假体控制
authors: "Hakim, R., Jaggi, A., Heo, G., Matsumoto, H., Uchida, N., Watabe-Uchida, M., Datta, S. R., Musall, S., Sabatini, B. L."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.1101/2025.09.10.675423v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 通过频谱分析从面部运动中预测意图
tldr: 本研究针对啮齿类动物面部运动与神经活动关联分析的难题，开发了名为 face-rhythm 的无监督分析框架。该框架结合了无标记点追踪、频谱分析和非负张量分量分析，能将复杂的面部视频分解为如胡须摆动、嗅闻和舔舐等可解释的低维组件。实验证明，这些组件不仅能跨个体稳定预测任务变量和内部状态，还能有效解释初级运动皮层的神经活动，揭示了不同频率运动在皮层中的差异化表征方式。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决精确测量啮齿类动物节律性面部运动并将其与复杂神经活动相关联的挑战。
method: 提出 face-rhythm 框架，通过结合点追踪、频谱分析和非负张量分解，将面部视频转化为可解释的运动分量。
result: 该方法能准确识别多种面部行为，解码任务变量，并发现运动皮层对高频运动采用相位不变的频谱表征，对低频运动采用相位可变的表征。
conclusion: face-rhythm 为研究面部行为及其神经机制提供了一个低维、可解释且极具竞争力的计算工具。
---

## 摘要
包括人类在内的动物利用协调的面部运动来采样环境、摄取营养和进行交流。啮齿动物尤其在自发行为和认知任务中产生节律性的面部运动。精确测量这些运动并将其与神经活动联系起来仍然具有挑战性。我们介绍了 face-rhythm，这是一个无监督流程，它结合了无标记点追踪、光谱分析和非负张量分量分析，将面部视频分解为一小组可解释的分量。将其应用于巴甫洛夫气味奖励任务、脑机接口（BMI）任务和自由行为期间的小鼠视频，face-rhythm 恢复了人类可解释的行为，如拂须、嗅探、舔舐以及更细微的行为。所产生的分量在不同动物之间具有一致性，足以解码任务变量或内部信念状态，并使用低秩表征解释皮层活动。我们还发现，面部相关初级运动皮层（M1）的神经元活动可以通过约 0.5 Hz 以上面部运动的相位不变光谱变换得到很好的预测，而较慢的运动则保留了相位可变的表征，能更好地通过面部的瞬时位置来预测；单个神经元可以表现出其中一种或两种调谐形式。与深度学习点追踪模型、对比学习嵌入和视觉 Transformer 特征的系统比较表明，face-rhythm 在各项任务中都具有竞争力，同时也实现了生成与皮层活动密切相关的啮齿动物面部行为的低维、可解释描述的目标。

## Abstract
Animals, including humans, use coordinated facial movements to sample the environment, ingest nutrients, and communicate. Rodents, in particular, produce rhythmic facial movements during spontaneous behavior and cognitive tasks. Measuring these movements precisely and linking them to neural activity remains challenging. We introduce face-rhythm, an unsupervised pipeline that combines markerless point tracking, spectral analysis, and non-negative tensor component analysis to decompose facial video into a small set of interpretable components. Applied to videos of mice during a Pavlovian odor-reward task, a brain-machine interface (BMI) task, and free behavior, face-rhythm recovers human-interpretable behaviors such as whisking, sniffing, licking, and more subtle behaviors. The resulting components are consistent across animals, are sufficient to decode task variables or internal belief states, and explain cortical activity using a low-rank representation. We also find that the activity of neurons in face-associated primary motor cortex (M1) is predicted well by a phase-invariant spectral transformation of facial movements above ~ 0.5 Hz, while slower movements retain a phase-variant representation better predicted by the instantaneous position of the face; individual neurons can show either or both forms of tuning. A systematic comparison against deep-learning point-tracking models, contrastive-learning embeddings, and vision-transformer features places face-rhythm competitively across tasks while also achieving the goal of producing a low-dimensional, interpretable description of rodent facial behavior that is closely linked to cortical activity.