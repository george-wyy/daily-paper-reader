---
title: "When feedback backfires: investigating neurofeedback effects in a closed-loop auditory attention decoding paradigm"
title_zh: 当反馈适得其反：在闭环听觉注意力解码范式中研究神经反馈效应
authors: "Rotaru, I., Geirnaert, S., Heintz, N., Bertrand, A., Francart, T."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721343v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 用于实时人机交互的闭环听觉注意力解码
tldr: 本研究探讨了实时神经反馈（NFB）对听觉注意力解码（AAD）的影响。通过对19名受试者在开环、听觉增益反馈、视觉反馈及伪听觉反馈四种条件下的实验，发现听觉神经反馈在短期内不仅未能提升解码准确率，反而因增加认知负荷和分心导致性能下降。研究结果表明，不稳定的反馈可能阻碍而非促进学习，强调了在闭环听觉注意力系统中使用更稳定解码器和长期训练协议的必要性。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究闭环系统中的实时神经反馈是否能通过人类与机器的交互及神经适应来提高听觉注意力解码的性能。
method: 对19名受试者进行单次实验，对比开环、听觉反馈、视觉反馈和伪听觉反馈四种条件下使用线性解码器进行注意力解码的效果。
result: 离线分析显示听觉反馈条件的解码准确率显著低于开环基准，且受试者主观感受该反馈更易分心并增加了注意力切换的难度。
conclusion: 单次实验中快速变化的听觉反馈可能因增加认知负荷而降低解码性能，未来需通过更精确的解码器和长期训练来实现神经反馈的正面效应。
---

## 摘要
选择性听觉注意力解码（AAD）能够追踪听者在多个并发说话者中关注的对象，是神经控制助听设备的关键构建模块。虽然假设将 AAD 集成到具有实时神经反馈（NFB）的闭环系统中可以通过神经适应和纠错行为提高解码效果，但这种双向人机交互的短期行为和算法影响仍不清楚。在本研究中，我们评估了在包含 19 名参与者的单次 AAD 范式中，在线 NFB 对 AAD 准确率和用户体验的影响。参与者在四种条件下执行了带有强制注意力切换的选择性听音任务：开环（OL）、带有听觉增益反馈的闭环（CLA）、带有视觉反馈的闭环（CLV），以及一种与参与者个体神经活动脱钩的伪听觉增益控制（psCLA）条件。AAD 在线执行，在 5 秒滑动窗口上使用受试者特定和受试者无关的线性解码器，随后进行隐马尔可夫模型后处理。在线分析显示，所有条件下的解码性能相当。然而，使用受试者无关解码器的离线事后分析显示，CLA 条件下的 AAD 准确率显著低于 OL 基准。在主观上，参与者报告 CLA 明显更分散注意力，且需要更高的切换努力。至关重要的是，对 psCLA 条件的因果分析发现，没有确凿证据表明更高的音频增益本身能提高解码准确率。我们的结果表明，在具有快速变化反馈线索的单次实验范式中，听觉神经反馈可能会通过增加认知负荷和干扰来降低 AAD 性能。这些发现表明，次优的反馈可能会阻碍而非促进学习。我们得出结论，更准确、稳定的解码器以及纵向、多阶段的训练方案可能是闭环听觉注意力系统中实现有益神经反馈效应的必要前提。

## Abstract
Selective auditory attention decoding (AAD) enables tracking which of multiple concurrent speakers a listener attends to and is a key building block for neuro-steered hearing devices. While AAD integrated in a closed-loop system with real-time neurofeedback (NFB) is hypothesized to improve decoding through neural adaptation and error-correction behaviour, the short-term behavioral and algorithmic impact of such a bilateral human-machine interaction remains poorly understood. Here we evaluated the effects of NFB on AAD accuracy and user experience in a single-session AAD paradigm with online NFB involving nineteen participants. They performed a selective listening task with enforced attention switches across four conditions: open-loop (OL), closed-loop with auditory gain feedback (CLA), closed-loop with visual feedback (CLV), and a condition with pseudo-auditory gain control (psCLA) decoupled from the participants individual neural activity. AAD was performed online using both subject-specific and subject-independent linear decoders on 5 s sliding windows, followed by Hidden Markov Model post-processing. Online analysis showed comparable decoding performance across all conditions. However, offline posthoc analysis using subject-independent decoders revealed that AAD accuracy in the CLA condition was significantly lower than in the OL baseline. Subjectively, participants reported that CLA was significantly more distracting and required higher switching effort. Crucially, a causal analysis of the psCLA condition found no robust evidence that higher audio gains inherently improve decoding accuracy. Our results demonstrate that within a single-session paradigm with rapidly varying feedback cues, auditory neurofeedback may degrade AAD performance by increasing cognitive load and distraction. These findings suggest that suboptimal feedback can impede rather than facilitate learning. We conclude that more accurate and stable decoders and longitudinal, multi-session training protocols are likely essential prerequisites for achieving beneficial neurofeedback effects in closed-loop auditory attention systems.