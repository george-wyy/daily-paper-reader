---
title: Luminance-corrected Pupillometry for Reliable Effort-tracking in Dynamic Environments
title_zh: 动态环境中用于可靠努力追踪的亮度校正瞳孔测量法
authors: "Cai, Y., Naber, M., Van der Stigchel, S., Strauch, C."
date: 2026-05-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728653v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 瞳孔测量可应用于眼动意图识别中的努力追踪
tldr: 瞳孔测量法虽能客观追踪努力程度，但动态环境中亮度变化严重干扰其可靠性。本文提出一种基于Open-DPSM模型的亮度校正方法，通过分解整体亮度和逐帧变化对视网膜照度的影响，显著恢复动态视觉输入下的努力区分度。经听觉n-back任务验证，校正后瞳孔数据在聚合和时间分辨率水平均优于原始数据，且与行为及主观指标互补，三者融合的AUC达0.98。该工作为复杂动态场景下的努力与唤醒研究提供了可行工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 瞳孔大小受亮度强烈干扰，限制了其在动态视觉环境中的应用，需要校正亮度效应以获得可靠的努力度量。
method: 参与者执行听觉n-back任务，同时观看恒定或动态驾驶视频；采用Open-DPSM模型整体和逐帧校正亮度对瞳孔尺寸的影响。
result: 亮度校正后瞳孔测量的努力区分度显著提升，聚合水平略优于准确性和NASA-TLX，三者结合AUC=0.98。
conclusion: 亮度校正的瞳孔测量法适用于动态环境，联合多模态指标可精准追踪努力和唤醒状态。
---

## 摘要
瞳孔测量法提供了一种跨领域索引努力的客观方法。然而，瞳孔大小受亮度变化影响强烈，这可能会掩盖与努力相关的影响，并限制其在大多数具有动态视觉输入的应用场景中的使用。我们在此介绍并验证了一种克服这一问题的方法。为此，参与者在观看恒定视觉输入或动态驾驶电影片段的同时，执行不同难度的听觉n-back任务。努力通过生理（瞳孔大小）、行为（准确性）和主观（NASA-TLX）指标进行评估。在实验阶段层面分析准确性、问卷评分和瞳孔大小，而瞳孔测量法还额外提供了连续的时间分辨信息。正如预期，瞳孔测量法追踪了努力的差异，但其区分度在动态视觉输入下显著降低。使用一种动态、可解释且开源的建模程序（Open-DPSM）校正整体亮度和逐时刻亮度变化的影响，在聚合和时间分辨两个层面上显著提高了努力的区分度。在聚合层面上，亮度校正的瞳孔测量法略优于准确性和NASA-TLX。将三者结合使用获得了最高的分类性能（AUC = 0.98），支持了努力是多维度的且最好通过多模态方式捕获的观点。这些发现为在基础和应用研究中利用复杂动态刺激进行努力和唤醒的精细生理追踪建立了实践基础。一篇教程部分引导研究人员使用这里验证的方法，在动态观察环境中对其自身的瞳孔测量数据进行亮度校正。

## Abstract
Pupillometry provides an objective way to index effort across domains. However, pupil size is strongly affected by luminance changes, which can obscure effort-related effects, and limit its use in most applied scenarios with dynamic visual input. We here introduce and validate a method to overcome this problem. To this end, participants performed an auditory n-back task of differing difficulty while viewing either constant visual input or dynamic driving movie clips. Effort was assessed physiologically (pupil size), behaviorally (accuracy), and subjectively (NASA-TLX). Accuracy, questionnaire scores, and pupil size were analyzed at the session level, while pupillometry additionally provided continuous time-resolved information. As expected, pupillometry tracked differences in effort, but its discriminability was substantially reduced under dynamic visual input. Correcting for the effects of overall luminance and moment-to-moment luminance changes using a dynamic, explainable, and open-source modeling procedure (Open-DPSM) considerably improved effort discriminability on both aggregate and time-resolved levels. At the aggregate level, luminance-corrected pupillometry slightly outperformed accuracy and NASA-TLX. Combining all three measures yielded the highest classification performance (AUC = 0.98), supporting the view that effort is multifaceted and best captured multimodally. These findings establish a practical basis for fine-grained physiological tracking of effort and arousal in both fundamental and applied research using complex, dynamic stimuli. A tutorial section guides researchers in applying luminance correction to their own pupillometric data in dynamic viewing environments using the here validated approach.