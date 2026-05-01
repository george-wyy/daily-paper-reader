---
title: "When feedback backfires: investigating neurofeedback effects in a closed-loop auditory attention decoding paradigm"
authors: "Rotaru, I., Geirnaert, S., Heintz, N., Bertrand, A., Francart, T."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721343v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 闭环人机交互与实时神经反馈
tldr: 本研究探讨了神经反馈（NFB）在闭环听觉注意解码（AAD）系统中的作用。通过对19名受试者进行四种实验条件（开环、听觉闭环、视觉闭环及伪听觉闭环）的对比测试，发现听觉神经反馈在短期内不仅未能提升解码准确率，反而因增加认知负荷和分心导致性能下降。研究结果挑战了反馈必然提升性能的假设，强调了稳定解码器和长期训练对实现闭环AAD系统增益的重要性。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究实时神经反馈在闭环听觉注意解码系统中对解码准确率和用户体验的具体影响。
method: 招募19名受试者在开环、听觉闭环、视觉闭环及伪听觉反馈四种条件下执行选择性听力任务，并结合线性解码器进行在线与离线分析。
result: 离线分析显示听觉闭环反馈下的解码准确率显著低于开环基准，且受试者主观反馈该模式更易分心并增加切换负担。
conclusion: 在单次实验中，不稳定的听觉反馈会因增加认知负担而损害解码性能，未来需更稳定的解码器和多阶段训练。
---

## Abstract
Selective auditory attention decoding (AAD) enables tracking which of multiple concurrent speakers a listener attends to and is a key building block for neuro-steered hearing devices. While AAD integrated in a closed-loop system with real-time neurofeedback (NFB) is hypothesized to improve decoding through neural adaptation and error-correction behaviour, the short-term behavioral and algorithmic impact of such a bilateral human-machine interaction remains poorly understood. Here we evaluated the effects of NFB on AAD accuracy and user experience in a single-session AAD paradigm with online NFB involving nineteen participants. They performed a selective listening task with enforced attention switches across four conditions: open-loop (OL), closed-loop with auditory gain feedback (CLA), closed-loop with visual feedback (CLV), and a condition with pseudo-auditory gain control (psCLA) decoupled from the participants' individual neural activity. AAD was performed online using both subject-specific and subject-independent linear decoders on 5 s sliding windows, followed by Hidden Markov Model post-processing. Online analysis showed comparable decoding performance across all conditions. However, offline posthoc analysis using subject-independent decoders revealed that AAD accuracy in the CLA condition was significantly lower than in the OL baseline. Subjectively, participants reported that CLA was significantly more distracting and required higher switching effort. Crucially, a causal analysis of the psCLA condition found no robust evidence that higher audio gains inherently improve decoding accuracy. Our results demonstrate that within a single-session paradigm with rapidly varying feedback cues, auditory neurofeedback may degrade AAD performance by increasing cognitive load and distraction. These findings suggest that suboptimal feedback can impede rather than facilitate learning. We conclude that more accurate and stable decoders and longitudinal, multi-session training protocols are likely essential prerequisites for achieving beneficial neurofeedback effects in closed-loop auditory attention systems.