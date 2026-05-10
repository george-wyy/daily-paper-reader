---
title: "spatiAlytica: Viewer-Grounded Multimodal Agentic System for Interactive Spatial Omics Analysis"
title_zh: spatiAlytica：用于交互式空间组学分析的基于查看器的多模态智能体系统
authors: "Das, A., Zhang, K., Song, J., Han, M., Chen, A., Meng, W., Galloway, H., Chen, P.-Y., Jo, S., Liu, Z., Hasib, M. M., Officer, A., Sinha, H., Chiu, Y.-C., Gao, S.-J., Li, L., Huang, Y."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.29.721735v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 以观察者为中心的多模态交互代理系统
tldr: 空间组学分析受限于编程门槛和现有AI工具缺乏视觉交互能力。本文提出spatiAlytica，一个嵌入Napari查看器的多模态智能体系统，支持非编程背景的生物学家通过自然语言进行交互式分析。该系统集成了状态序列化、代码生成、空间视觉问答等功能，并推出了包含多维度任务的基准测试集spatiAlyticaBench。实验证明其在效率和准确性上优于现有基准，并成功应用于多种癌症研究。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决空间组学分析中编程门槛高以及现有AI智能体缺乏视觉感知和跨轮对话上下文的问题。
method: 开发了嵌入Napari查看器的多模态智能体系统，结合了查看器状态序列化、智能体记忆、代码生成与调试以及空间视觉问答技术。
result: 在spatiAlyticaBench基准测试中表现优于强基线模型，且在癌症案例研究中成功复现了已知空间模式并发现了新的生物学现象。
conclusion: spatiAlytica为非编程生物学家提供了一个强大的探索性分析工具，显著提升了空间组学研究的效率和深度。
---

## 摘要
空间转录组学和蛋白质组学能够绘制组织架构和细胞相互作用图谱，但其分析仍受限于编程需求以及缺乏查看器关联和跨轮次上下文的以文本为中心的AI智能体。我们提出了spatiAlytica，这是一个嵌入在Napari查看器中的以查看器为中心的多模态交互式智能体系统，使非编程背景的生物学家能够通过自然语言进行迭代式、假设驱动的空间组学分析。spatiAlytica结合了查看器状态序列化、智能体记忆、生物学概念到数据字段的映射、代码生成与调试、空间视觉问答（Spatial VQA）以及关联解释，以支持探索性分析和解释性推理工作流。我们推出了spatiAlyticaBench，这是一个全面的基准测试，涵盖了222个单轮空间分析编码问题、178个多轮顺序工作流问题以及7,350个基于图像的推理问题。spatiAlytica的表现优于强大的智能体基准模型，同时消耗的时间和Token更少。针对卡波西肉瘤、结直肠癌和卵巢癌的案例研究重现了已知的空间模式，并揭示了卡波西肉瘤进展过程中CD8 T细胞的渐进性功能障碍。

## Abstract
Spatial transcriptomics and proteomics map tissue architecture and cellular interactions, but analysis remains limited by programming demands and text-centered AI agents that lack viewer grounding and cross-turn context. We present spatiAlytica, a viewer-centric multimodal interactive agentic system embedded in the Napari viewer that enables non-programmer biologists to perform iterative, hypothesis-driven spatial omics analysis via natural language. spatiAlytica couples viewer-state serialization, agentic memory, biological concept-to-data-field mapping, code generation and debugging, Spatial VQA, and grounded interpretation to support an exploratory analysis and interpretive reasoning workflow. We introduce spatiAlyticaBench, a comprehensive benchmark spanning 222 single-turn spatial analytical coding questions, 178 multi-turn sequential workflow questions, and 7,350 image-grounded reasoning questions. spatiAlytica outperformed strong agentic baselines, while using less time and tokens. Case studies across Kaposis sarcoma, colorectal cancer, and ovarian cancer recapitulated known spatial patterns and uncovered progressive CD8 T-cell dysfunction during KS progression.