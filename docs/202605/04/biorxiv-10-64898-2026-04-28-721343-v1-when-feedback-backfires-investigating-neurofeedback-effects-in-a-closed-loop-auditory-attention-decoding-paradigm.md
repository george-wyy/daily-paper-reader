---
title: "When feedback backfires: investigating neurofeedback effects in a closed-loop auditory attention decoding paradigm"
title_zh: 当反馈适得其反：在闭环听觉注意力解码范式中研究神经反馈效应
authors: "Rotaru, I., Geirnaert, S., Heintz, N., Bertrand, A., Francart, T."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721343v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 闭环听觉注意力解码与实时神经反馈
tldr: 本研究探讨了实时神经反馈对听觉注意力解码（AAD）的影响。通过对19名受试者在开环、闭环听觉/视觉反馈及伪反馈四种条件下的实验，发现听觉神经反馈在单次实验中不仅未提升解码准确率，反而因增加认知负荷导致性能下降。研究揭示了不当反馈的负面效应，强调了开发稳定解码器和长期训练方案的必要性。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究闭环系统中的实时神经反馈是否能通过神经适应提高听觉注意力解码的准确性。
method: 对19名受试者在开环、听觉反馈、视觉反馈和伪听觉反馈四种条件下进行选择性听力任务实验。
result: 离线分析显示听觉反馈条件的解码准确率显著低于开环基准，且受试者主观感到更易分心。
conclusion: 单次实验中的不稳定听觉反馈会因增加认知负担而损害解码性能，需更精确的解码器和长期训练。
---

## 摘要
选择性听觉注意力解码（AAD）能够追踪听者在多个并发说话者中关注的对象，是神经控制助听设备的关键构建模块。虽然假设将 AAD 集成到具有实时神经反馈（NFB）的闭环系统中可以通过神经适应和纠错行为提高解码效果，但这种双向人机交互的短期行为和算法影响仍知之甚少。本研究在涉及 19 名参与者的在线 NFB 单次 AAD 范式中，评估了 NFB 对 AAD 准确率和用户体验的影响。参与者在四种条件下执行了带有强制注意力切换的选择性听音任务：开环（OL）、带听觉增益反馈的闭环（CLA）、带视觉反馈的闭环（CLV），以及与参与者个体神经活动脱钩的伪听觉增益控制（psCLA）条件。AAD 在线执行，在 5 秒滑动窗口上使用受试者特异性和受试者无关的线性解码器，随后进行隐马尔可夫模型后处理。在线分析显示所有条件下的解码性能相当。然而，使用受试者无关解码器的离线事后分析显示，CLA 条件下的 AAD 准确率显著低于 OL 基准。主观上，参与者报告 CLA 显著更易分心，且需要更高的切换努力。至关重要的是，对 psCLA 条件的因果分析发现，没有确凿证据表明更高的音频增益能本质上提高解码准确率。我们的结果表明，在具有快速变化反馈线索的单次实验范式中，听觉神经反馈可能会因增加认知负荷和分心而降低 AAD 性能。这些发现表明，次优反馈可能会阻碍而非促进学习。我们得出结论，更准确、稳定的解码器以及纵向、多阶段的训练方案可能是闭环听觉注意力系统中实现有益神经反馈效应的必要前提。

## Abstract
Selective auditory attention decoding (AAD) enables tracking which of multiple concurrent speakers a listener attends to and is a key building block for neuro-steered hearing devices. While AAD integrated in a closed-loop system with real-time neurofeedback (NFB) is hypothesized to improve decoding through neural adaptation and error-correction behaviour, the short-term behavioral and algorithmic impact of such a bilateral human-machine interaction remains poorly understood. Here we evaluated the effects of NFB on AAD accuracy and user experience in a single-session AAD paradigm with online NFB involving nineteen participants. They performed a selective listening task with enforced attention switches across four conditions: open-loop (OL), closed-loop with auditory gain feedback (CLA), closed-loop with visual feedback (CLV), and a condition with pseudo-auditory gain control (psCLA) decoupled from the participants' individual neural activity. AAD was performed online using both subject-specific and subject-independent linear decoders on 5 s sliding windows, followed by Hidden Markov Model post-processing. Online analysis showed comparable decoding performance across all conditions. However, offline posthoc analysis using subject-independent decoders revealed that AAD accuracy in the CLA condition was significantly lower than in the OL baseline. Subjectively, participants reported that CLA was significantly more distracting and required higher switching effort. Crucially, a causal analysis of the psCLA condition found no robust evidence that higher audio gains inherently improve decoding accuracy. Our results demonstrate that within a single-session paradigm with rapidly varying feedback cues, auditory neurofeedback may degrade AAD performance by increasing cognitive load and distraction. These findings suggest that suboptimal feedback can impede rather than facilitate learning. We conclude that more accurate and stable decoders and longitudinal, multi-session training protocols are likely essential prerequisites for achieving beneficial neurofeedback effects in closed-loop auditory attention systems.