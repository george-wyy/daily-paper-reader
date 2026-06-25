---
title: "ResXR: validated infrastructure for reproducible studies of human behavior in Extended Reality"
title_zh: ResXR：用于增强现实中可重复人类行为研究的经过验证的基础设施
authors: "Bergstein, Y., Barel, N., Shai Basson, G., Bromberg, O., Schonberg, T."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.17.732869v1.full.pdf"
tags: ["query:gaze-intent"]
score: 7.0
evidence: 开源XR工具包，同步眼动追踪；支持基于注视的人机交互研究
tldr: XR行为研究缺乏共享基础设施，定制工具导致数据格式不统一，难以复现。ResXR开源工具包包含Unity模板记录头、手、眼、面同步追踪数据，Python管线验证质量并输出标准Motion-BIDS格式。基于应力测试验证传感器行为，提供三个现成范式。旨在为可复现XR实验建立透明、社区可扩展的基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 克服XR行为研究中共享基础设施缺失导致的数据格式混乱和实验结果难以复现的问题。
method: 开发ResXR工具包：Unity模板记录同步追踪数据，Python管线验证质量并输出Motion-BIDS格式数据集与质量报告。
result: 提供三个现成范式，验证了传感器数据的可靠性，生成了包含质量标志的标准化数据集和自包含报告。
conclusion: 为可复现的XR实验奠定透明、社区可扩展的基础设施，推动标准化数据共享与复现研究。
---

## 摘要
扩展现实（XR）结合了实验控制和生态效度，但行为XR研究缺乏共享基础设施：构建沉浸式实验需要专门的工程知识，而定制工具生成的自定义格式数据其他实验室难以重新分析。我们提出ResXR（Research with XR），这是一个开源工具包，提供从沉浸式实验到标准化数据集和质量报告的路径，可在独立头显上运行。一个Unity模板记录同步的头、手、眼和面部追踪数据，并带有每个样本的硬件时间戳；一个独立的Python管道验证质量、标记被屏蔽的时间段，并以Motion-BIDS格式导出原始和衍生数据集，附带自包含的质量报告。三个即用型范式涵盖了常见的行为设计。ResXR是XR研究中的一个新理念：消费者头显的传感器数据必须经过实证验证，而不是直接取自供应商文档，其模式和质量标记基于经过压力测试的传感器行为。其目标是为可重复的XR实验提供一个透明、社区可扩展的基础。

## Abstract
Extended Reality (XR) combines experimental control and ecological validity, yet behavioral XR research lacks shared infrastructure: building immersive experiments demands specialized engineering, and custom tools yield data in custom formats that other laboratories cannot readily reanalyze. We present ResXR (Research with XR), an open-source toolkit providing a path from immersive experiment to standardized dataset and quality report, running on standalone headsets. A Unity template records synchronized head, hand, eye, and face tracking with per-sample hardware timestamps; an independent Python pipeline validates quality, masks flagged intervals, and exports raw and derivative datasets in Motion-BIDS format with self-contained quality reports. Three ready-to-run paradigms span common behavioral designs. ResXR is an idea new to XR research: sensor data from consumer headsets must be empirically validated rather than taken from vendor documentation, grounding its schema and quality flags in stress-tested sensor behavior. Its aim is a transparent, community-extensible foundation for reproducible XR experimentation.