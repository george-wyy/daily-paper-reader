---
title: Modality-specific predictive templates in pre-stimulus EEG activity
authors: "Hoxha, I., Chevallier, S., Delorme, A., Amorim, M.-A."
date: 2026-04-18
pdf: "https://www.biorxiv.org/content/10.1101/2023.09.27.559806v3.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 预刺激活动中用于预测事件的预测模板
tldr: 解码预刺激 EEG 活动，以识别用于预测视觉或听觉事件的特定模态模板。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2023-09-27-559806-v3/fig-001.webp\", \"caption\": \"\", \"page\": 4, \"index\": 1, \"width\": 1387, \"height\": 568}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2023-09-27-559806-v3/fig-002.webp\", \"caption\": \"\", \"page\": 8, \"index\": 2, \"width\": 1360, \"height\": 1295}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2023-09-27-559806-v3/fig-003.webp\", \"caption\": \"\", \"page\": 10, \"index\": 3, \"width\": 1383, \"height\": 1138}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2023-09-27-559806-v3/fig-004.webp\", \"caption\": \"\", \"page\": 11, \"index\": 4, \"width\": 1371, \"height\": 430}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2023-09-27-559806-v3/fig-005.webp\", \"caption\": \"\", \"page\": 14, \"index\": 5, \"width\": 1385, \"height\": 770}]"
motivation: 预刺激活动中用于预测事件的预测模板。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
Perceptual decision-making is a combination of sensory information and prior beliefs. In order to perform actions in a timely fashion, it is necessary to anticipate the timing at which events occur, but also what event is more likely than the other. While EEG signatures of anticipation have been identified it is less clear whether classifiers trained on informative (cued) trials generalize to uncued trials and whether such decoded templates predict trial-by-trial shifts in decision strategy (e.g., drift-rate or starting-point changes in a Diffusion Decision Model). This study aimed to determine whether human participants anticipated a visual or auditory stimulus at the single-trial level in both cued and uncued trials. We found that pre-stimulus brain activity contains information about the expected upcoming stimulus and that this information can be successfully extracted from single-trial brain activity. Behavioral analyses revealed a connection between correct anticipation and shifts in decision strategy, while also validating the classification of uncued trials. Importantly, the classification of uncued trials confirms that expectations build even in the absence of triggers. These findings highlight the presence of single-trial, stimulus-specific neural signatures of anticipation, offering new insights into trial-to-trial variability in decision-making and advancing our understanding of cognitive processes.