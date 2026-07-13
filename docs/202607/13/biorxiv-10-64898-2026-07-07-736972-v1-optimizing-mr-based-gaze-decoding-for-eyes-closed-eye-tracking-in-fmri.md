---
title: Optimizing MR-based gaze-decoding for eyes-closed eye-tracking in fMRI
title_zh: 优化基于磁共振的注视解码技术以实现fMRI中闭眼状态的眼动追踪
authors: "Kling, S. M., Lascombes, U., Nau, M., Masson, G. S., Szinte, M."
date: 2026-07-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.07.736972v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 基于MR信号的眼动解码提升眼动追踪
tldr: fMRI研究中闭眼时无法使用摄像头追踪眼动，阻碍了对闭眼状态认知的探索。本文利用深度学习框架DeepMReye从眼部MR信号解码注视行为，通过开眼时的视动校准数据微调显著提升解码性能，并发现模型能泛化到闭眼状态。进一步加入闭眼时注视已知位置的微调数据，性能继续提升。研究表明闭眼期间可实现可靠注视监测，为fMRI眼动研究提供新途径。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-07-736972-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1752, \"height\": 752, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-07-736972-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1719, \"height\": 699, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-07-736972-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1737, \"height\": 734, \"label\": \"Figure\"}]"
motivation: 解决fMRI中闭眼时摄像头无法追踪眼动的问题，实现闭眼状态下的注视解码。
method: 使用DeepMReye模型，通过开眼和闭眼时的视动校准数据微调，从眼部MR信号解码注视位置。
result: 开眼数据微调显著提升解码性能，模型泛化到闭眼；加入闭眼数据微调后性能进一步提高。
conclusion: 闭眼期间可基于MR信号实现可靠注视监测，有助于将眼动追踪更好整合到fMRI研究。
---

## 摘要
眼动为人类认知提供了宝贵的见解，并且是许多功能磁共振成像（fMRI）研究中的关键变量。然而，当闭眼时，基于摄像头的眼动追踪不可用，使得闭眼状态的研究充满挑战。在这里，我们通过基于磁共振的注视解码技术，使用DeepMReye（一种从眼部MR信号中无摄像头重建注视行为的深度学习框架）来填补这一空白。我们首先证明，使用睁眼时获取的视觉运动校准数据对DeepMReye进行微调，能显著改善注视解码效果，并且这种微调不需要同时获取基于摄像头的数据。接着，我们评估了将参与者在睁眼和闭眼状态下注视已知位置时获取的数据纳入模型是否能进一步提升性能。值得注意的是，尽管DeepMReye最初仅在睁眼数据上训练，但网络成功推广到了闭眼时段，并且通过在闭眼数据上微调，性能显著提升。这些发现表明，在闭眼期间进行可靠的注视监测是可行的，从而能更有效地将眼动追踪整合到fMRI研究中，进而增进我们对人类认知的理解。

## Abstract
Eye movements provide valuable insights into human cognition and are a critical variable in numerous functional magnetic resonance imaging (fMRI) studies. Yet, when the eyes are closed, camera-based eye-tracking is unavailable, making studies of eyes-closed states challenging. Here, we address this gap through MR-based gaze decoding with DeepMReye, a deep learning framework for camera-free reconstruction of gaze behavior from the MR-signal of the eyes. We first show that fine-tuning DeepMReye using visuomotor calibration data acquired when the eyes were open significantly improves gaze decoding, and that this fine-tuning does not require simultaneous camera-based data. We next assessed whether model performance could be further improved by incorporating data acquired while participants gazed at known positions with both eyes open and closed. Notably, while DeepMReye was originally trained exclusively on eyes-open data, the network successfully generalized eyes-closed periods, with performance improving significantly through fine-tuning on the eyes-closed data. These findings demonstrate that reliable gaze monitoring during eyes-closed periods is feasible, enabling a more effective integration of eye-tracking in fMRI research and, consequently, advancing our understanding of human cognition.