---
title: "Spectral envelopes of facial movements predict intention, cortical representations, and neural prosthetic control"
title_zh: 面部运动的频谱包络可预测意图、皮层表征和神经假体控制
authors: "Hakim, R., Jaggi, A., Heo, G., Matsumoto, H., Uchida, N., Watabe-Uchida, M., Datta, S. R., Musall, S., Sabatini, B. L."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.1101/2025.09.10.675423v3.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 面部运动通过无监督流程预测意图和神经假体控制
tldr: 本研究开发了名为 face-rhythm 的无监督分析框架，通过结合标记点追踪、频谱分析和非负张量分解，将小鼠复杂的面部运动分解为可解释的低维组件。该方法能有效解码任务变量和内部状态，并揭示了初级运动皮层（M1）对不同频率面部运动的独特编码模式，为理解面部行为与神经活动之间的联系提供了高效且可解释的工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决精确测量啮齿动物节律性面部运动并将其与复杂神经活动相关联的挑战。
method: 提出 face-rhythm 框架，利用无监督学习、频谱分析和张量分解将面部视频转化为可解释的行为组件。
result: 该方法成功识别了嗅探、理毛等行为，能高效解码任务状态，并发现 M1 神经元对高频运动具有相位不变的频谱表征。
conclusion: face-rhythm 在保持高性能解码的同时，提供了一种与皮层活动紧密相关的低维、可解释的面部行为描述方式。
---

## 摘要
包括人类在内的动物利用协调的面部运动来采样环境、摄取营养和进行交流。啮齿动物尤其在自发行为和认知任务中产生节律性的面部运动。精确测量这些运动并将其与神经活动联系起来仍然具有挑战性。我们介绍了 face-rhythm，这是一个无监督流水线，它结合了无标记点追踪、频谱分析和非负张量分量分析，将面部视频分解为一小组可解释的分量。将 face-rhythm 应用于小鼠在巴甫洛夫气味奖励任务、脑机接口（BMI）任务和自由行为期间的视频，可以恢复人类可解释的行为，如拨须、嗅探、舔舐以及更细微的行为。所得的分量在不同动物之间具有一致性，足以解码任务变量或内部信念状态，并使用低秩表征解释皮层活动。我们还发现，面部相关初级运动皮层（M1）中的神经元活动可以通过约 0.5 Hz 以上面部运动的相位不变频谱变换得到很好的预测，而较慢的运动则保留了相位可变的表征，能更好地通过面部的瞬时位置进行预测；单个神经元可以表现出其中一种或两种调谐形式。与深度学习点追踪模型、对比学习嵌入和视觉 Transformer 特征的系统比较表明，face-rhythm 在各项任务中都具有竞争力，同时也实现了生成与皮层活动密切相关的啮齿动物面部行为的低维、可解释描述的目标。

## Abstract
Animals, including humans, use coordinated facial movements to sample the environment, ingest nutrients, and communicate. Rodents, in particular, produce rhythmic facial movements during spontaneous behavior and cognitive tasks. Measuring these movements precisely and linking them to neural activity remains challenging. We introduce face-rhythm, an unsupervised pipeline that combines markerless point tracking, spectral analysis, and non-negative tensor component analysis to decompose facial video into a small set of interpretable components. Applied to videos of mice during a Pavlovian odor-reward task, a brain-machine interface (BMI) task, and free behavior, face-rhythm recovers human-interpretable behaviors such as whisking, sniffing, licking, and more subtle behaviors. The resulting components are consistent across animals, are sufficient to decode task variables or internal belief states, and explain cortical activity using a low-rank representation. We also find that the activity of neurons in face-associated primary motor cortex (M1) is predicted well by a phase-invariant spectral transformation of facial movements above ~ 0.5 Hz, while slower movements retain a phase-variant representation better predicted by the instantaneous position of the face; individual neurons can show either or both forms of tuning. A systematic comparison against deep-learning point-tracking models, contrastive-learning embeddings, and vision-transformer features places face-rhythm competitively across tasks while also achieving the goal of producing a low-dimensional, interpretable description of rodent facial behavior that is closely linked to cortical activity.