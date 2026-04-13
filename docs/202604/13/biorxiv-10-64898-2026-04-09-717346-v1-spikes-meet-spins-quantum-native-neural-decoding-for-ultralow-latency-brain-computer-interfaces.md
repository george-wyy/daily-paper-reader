---
title: "Spikes meet Spins: Quantum-Native Neural Decoding for Ultra_Low-Latency Brain-Computer Interfaces"
title_zh: 脉冲遇上自旋：用于超低延迟脑机接口的量子原生神经解码
authors: "Li, G., Ye, Y., Su, H., Tian, Y., Jiang, L., Yang, Y., Huang, Y., Gao, Q., Wen, K., Sun, L."
date: 2026-04-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.09.717346v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.5
evidence: 使用量子原生架构的脑机接口超低延迟神经解码
tldr: "针对脑机接口在神经信号规模扩大时面临的延迟挑战，本研究提出一种基于1000位相干光子伊辛机的量子原生神经解码方法。通过将神经脉冲模式映射到伊辛哈密顿量，利用硬件能量弛豫实现推理。该方法在多物种数据集上达到96.2%的准确率，延迟仅为0.075毫秒，比GPU快十倍，为超低延迟BCI系统提供了新途径。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-09-717346-v1/fig-001.webp\", \"caption\": \"Fig. 1. Spikes-to-spins workflow for neural decoding via physical energy relaxation. (A, B) Schematic of the \\\"spikes-to-spins\\\" interface, where multi-channel neural spike trains are\", \"page\": 20, \"index\": 1, \"width\": 976, \"height\": 521}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-09-717346-v1/fig-002.webp\", \"caption\": \"Fig. 2. Multi-modal spike quantization and task validation.\", \"page\": 21, \"index\": 2, \"width\": 882, \"height\": 1314}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-09-717346-v1/fig-003.webp\", \"caption\": \"Fig. 3. Performance comparison against state-of-the-art classical decoders. (A, B) Head-to-head decoding accuracy comparison of the quantum-native QSRBM against GPU-accelerated classical architectures (Transformer, Conformer, LSTM, and CNN) across four\", \"page\": 23, \"index\": 3, \"width\": 750, \"height\": 664}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-09-717346-v1/fig-004.webp\", \"caption\": \"Fig. 4. Hardware-validated latency, scaling, and energy efficiency. (A) Distribution of the number of \\\"shots\\\" (iterations) required to reach the ground state during physical relaxation, derived from 36,333 hardware decoding trials; inset shows the mapping of\", \"page\": 24, \"index\": 4, \"width\": 976, \"height\": 391}]"
motivation: 传统计算架构在处理大规模神经记录时存在严重的延迟瓶颈，难以满足实时脑机接口的高性能需求。
method: 提出量子半受限玻尔兹曼机（QSRBM），利用1000量子比特相干光子伊辛机的硬件能量弛豫特性进行神经解码。
result: "在多种体内数据集中实现高达96.2%的准确率，硬件验证的延迟仅为0.075毫秒，较GPU提升了十倍且具有复杂度不变的扩展性。"
conclusion: 量子计算在超低延迟神经解码方面展现出巨大潜力，是未来高性能脑机接口系统实现实时交互的可行演进方向。
---

## 摘要
脑机接口 (BCI) 需要对神经活动进行快速且准确的解码，然而随着神经记录规模的扩大，传统计算架构面临着日益增长的延迟。我们展示了一种利用物理 1000 量子比特相干光子伊辛机 (Ising machine) 实现的量子计算增强型神经解码方法，其中推理是通过硬件能量弛豫而非数值计算完成的。通过将稀疏神经脉冲模式映射到伊辛哈密顿量 (Ising Hamiltonians) 上，我们的硬件原生量子半受限玻尔兹曼机 (Quantum Semi-Restricted Boltzmann Machine) 在涵盖多个物种和模态的公开体内 (in vivo) 数据集上实现了高达 96.2% 的准确率。我们报告了经硬件验证的中值延迟为 0.075 毫秒——比 GPU 快十倍——且具有复杂度不变的扩展特性。这些结果确立了量子计算作为实现未来脑机接口系统超低延迟神经解码的可行路径。

## Abstract
Brain-computer interfaces (BCIs) require rapid and accurate decoding of neural activity, yet conventional computing architectures face growing latency as neural recording scales. We demonstrate a quantum computing-enabled neural decoding approach using a physical 1000-qubit coherent photonic Ising machine, in which inference is performed through hardware energy relaxation rather than numerical computation. By mapping sparse neural spike patterns onto Ising Hamiltonians, our hardware-native Quantum Semi-Restricted Boltzmann Machine achieves up to 96.2% accuracy across public in vivo datasets spanning multiple species and modalities. We report hardware-verified median latencies of 0.075 ms-a tenfold speedup over GPUs-with complexity-invariant scaling. These results establish quantum computing as a viable pathway toward ultra-low-latency neural decoding for future BCI systems.