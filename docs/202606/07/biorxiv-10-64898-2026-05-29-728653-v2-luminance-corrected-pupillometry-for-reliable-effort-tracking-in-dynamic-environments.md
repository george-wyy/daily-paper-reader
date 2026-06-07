---
title: Luminance-corrected Pupillometry for Reliable Effort-tracking in Dynamic Environments
title_zh: 用于动态环境中可靠努力追踪的亮度校正瞳孔测量法
authors: "Cai, Y., Naber, M., Van der Stigchel, S., Strauch, C."
date: 2026-05-31
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728653v2.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 瞳孔测量方法用于努力追踪，与眼动意图识别相关
tldr: 瞳孔测量可客观追踪努力程度，但动态环境中的亮度变化会干扰结果。本研究提出动态、可解释的开源建模程序Open-DPSM，校正整体和瞬时亮度影响，显著提升瞳孔测量在聚合和连续时间上的努力区分度。校正后瞳孔测量略优于准确率和NASA-TLX，三者联合AUC达0.98，支持努力的多维度性。该方法为复杂动态场景下的精细生理追踪提供了实用基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 动态视觉环境中亮度变化严重干扰瞳孔测量对努力程度的追踪，亟需有效校正方法。
method: 采用动态、可解释的开源建模程序Open-DPSM，校正总体亮度和瞬时亮度变化对瞳孔大小的影响。
result: 亮度校正后瞳孔测量在努力区分度上略优于准确率和NASA-TLX，三者联合分类AUC达0.98。
conclusion: 亮度校正瞳孔测量为动态刺激下努力和警觉的生理追踪建立了可靠实用基础。
---

## 摘要
瞳孔测量法提供了一种客观的方式来跨领域索引努力程度。然而，瞳孔大小受亮度变化强烈影响，这可能会掩盖与努力相关的效应，并限制其在大多数具有动态视觉输入的应用场景中的使用。我们在此介绍并验证了一种克服该问题的方法。为此，参与者在观看恒定视觉输入或动态驾驶电影片段的同时，执行不同难度的听觉n-back任务。努力程度通过生理指标（瞳孔大小）、行为指标（准确率）和主观指标（NASA-TLX）进行评估。在会话水平上分析了准确率、问卷得分和瞳孔大小，而瞳孔测量法还额外提供了连续的时间分辨信息。正如预期，瞳孔测量法追踪了努力程度的差异，但其区分度在动态视觉输入下显著降低。使用一种动态、可解释且开源的建模程序（Open-DPSM）校正整体亮度和逐帧亮度变化的影响后，在总体和时间分辨水平上显著提高了努力区分度。在总体水平上，亮度校正后的瞳孔测量法略优于准确率和NASA-TLX。将三项指标结合获得了最高的分类性能（AUC = 0.98），支持了努力是多维度的且最佳通过多模态捕捉的观点。这些发现为在基础和应用研究中使用复杂动态刺激进行精细的努力和唤醒生理追踪奠定了实践基础。一个教程部分指导研究人员如何使用本文验证的方法，对其在动态观看环境中的瞳孔测量数据应用亮度校正。

## Abstract
Pupillometry provides an objective way to index effort across domains. However, pupil size is strongly affected by luminance changes, which can obscure effort-related effects, and limit its use in most applied scenarios with dynamic visual input. We here introduce and validate a method to overcome this problem. To this end, participants performed an auditory n-back task of differing difficulty while viewing either constant visual input or dynamic driving movie clips. Effort was assessed physiologically (pupil size), behaviorally (accuracy), and subjectively (NASA-TLX). Accuracy, questionnaire scores, and pupil size were analyzed at the session level, while pupillometry additionally provided continuous time-resolved information. As expected, pupillometry tracked differences in effort, but its discriminability was substantially reduced under dynamic visual input. Correcting for the effects of overall luminance and moment-to-moment luminance changes using a dynamic, explainable, and open-source modeling procedure (Open-DPSM) considerably improved effort discriminability on both aggregate and time-resolved levels. At the aggregate level, luminance-corrected pupillometry slightly outperformed accuracy and NASA-TLX. Combining all three measures yielded the highest classification performance (AUC = 0.98), supporting the view that effort is multifaceted and best captured multimodally. These findings establish a practical basis for fine-grained physiological tracking of effort and arousal in both fundamental and applied research using complex, dynamic stimuli. A tutorial section guides researchers in applying luminance correction to their own pupillometric data in dynamic viewing environments using the here validated approach.