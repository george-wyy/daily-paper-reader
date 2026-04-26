---
title: Pupil and Neural Dynamics Reveal Belief-Dependent Decision Making Under Ambiguity
title_zh: 瞳孔与神经动力学揭示模糊情境下依赖信念的决策过程
authors: "Qin, Y., Rungratsameetaweemana, N., Lauharatanahirun, N., Sajda, P."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719818v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 结合瞳孔测量和EEG数据的多模态方法，揭示决策信念
tldr: 本研究探讨了人类在概率不明的模糊情境下如何进行决策。通过结合行为学、瞳孔测量和脑电图（EEG）的多模态方法，研究发现个体对模糊结果持有不同的内部信念模型。这些信念差异不仅体现在选择行为上，还通过瞳孔唤醒水平反映出来。研究表明，模糊规避并非单一的认知偏差，而是由异质性的主观信念驱动的，生理指标能有效追踪这些主观表征。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在揭示个体在模糊决策中如何内部表征未知结果，以及这些表征如何塑造其行为和生理反应。
method: 采用多模态研究方法，整合了行为实验、瞳孔测量和脑电图数据，分析风险与模糊条件下的决策过程。
result: 发现个体的决策策略反映了不同的内部信念，且瞳孔唤醒水平与主观信念而非客观任务结构紧密相关。
conclusion: 模糊规避源于异质性的内部信念模型，多模态生理数据为理解信念引导的价值决策提供了关键机制证据。
---

## 摘要
人类每天在模糊情境下做出数以千计的决策，在这些情境中，获得有利结果的概率往往并非完全已知。尽管模糊规避（ambiguity aversion）在群体层面已得到很好的刻画，但个体如何在内部表征模糊结果，以及这些表征如何塑造行为和生理反应，目前仍不清楚。为了解决这些问题，我们采用结合了行为、瞳孔测量和脑电图（EEG）数据的多模态方法，研究了风险和模糊情境下基于价值的决策。我们发现，个体采取了不同的决策策略，反映了对未知结果的不同内部信念。这些信念差异不仅体现在选择中，还体现在决策形成过程中的瞳孔关联唤醒（pupil-linked arousal）中。至关重要的是，不同策略之间的生理差异在模糊选项的客观估值规则下依然存在，但当使用每个个体的主观信念计算估值时，这些差异便消失了，这表明唤醒追踪的是主观信念而非客观任务结构。总之，我们的研究结果表明，模糊规避并非一种统一的偏差，而是反映了异质性的内部信念模型，且多模态生理学为理解这些信念引导基于价值的选择的机制提供了一个窗口。

## Abstract
Humans make thousands of decisions under ambiguity every day, where most times the probabilities of getting beneficial outcomes are not fully known. Although ambiguity aversion is well characterized at the aggregate level, it remains unclear how individuals internally represent ambiguous outcomes and how these representations shape behavior and physiology. To address these questions, we investigate value-based decision-making under risk and ambiguity using a multimodal approach that combines behavioral, pupillometric, and electroencephalographic (EEG) data. We show that individuals adopt distinct decision strategies that reflect different internal beliefs about unknown outcomes. These belief differences are expressed not only in choice but also in pupil-linked arousal during decision formation. Crucially, physiological differences across strategies persist under an objective valuation rule for ambiguous options but disappear when valuation is computed using each individuals subjective beliefs, indicating that arousal tracks subjective belief rather than objective task structure. Together, our findings show that ambiguity aversion is not a uniform bias but reflects heterogeneous internal belief models, and that multimodal physiology provides a window into the mechanisms through which these beliefs guide value-based choice.

---

## 论文详细总结（自动生成）

这是一份关于论文《Pupil and Neural Dynamics Reveal Belief-Dependent Decision Making Under Ambiguity》（瞳孔与神经动力学揭示模糊情境下依赖信念的决策过程）的深度结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：在现实生活中，决策往往面临“模糊性”（Ambiguity，即结果概率未知），而非单纯的“风险”（Risk，即概率已知）。虽然群体层面普遍存在“模糊规避”现象，但个体如何内部表征这些未知概率，以及这种表征如何影响生理和神经活动，尚不明确。
*   **核心问题**：模糊规避是一个统一的心理偏差，还是反映了不同个体之间异质性的内部信念模型？生理信号（瞳孔和脑电）能否揭示这些潜藏的信念？

### 2. 方法论：核心思想与技术细节
*   **多模态整合**：结合行为实验、瞳孔测量（Pupillometry）和脑电图（EEG）数据，通过计算建模（漂移扩散模型 DDM）将生理信号与决策过程关联。
*   **决策任务设计（LCT）**：参与者在“确定收益”和“博弈投资”之间选择。博弈包含三种模糊水平：0%（纯风险）、30%（低模糊）和60%（高模糊）。
*   **个体策略分层**：根据参与者在无模糊（纯风险）条件下的表现，将其分为三类：
    *   **理想型（Ideal）**：决策最符合期望价值（EV）最大化。
    *   **激进型（Aggressive）**：即使期望价值低也倾向于投资。
    *   **保守型（Conservative）**：即使期望价值高也倾向于保留现金。
*   **主观信念推断**：引入参数 $k$，代表个体对模糊区域中出现“高回报”概率的主观估计。
*   **漂移扩散模型（DDM）**：将瞳孔大小、EEG 频谱特征（额叶-顶叶差异）作为协变量，模拟证据积累过程中的漂移率（Drift Rate）。

### 3. 实验设计
*   **场景与数据集**：
    *   实验在沉浸式虚拟现实（VR）环境中进行（HTC VIVE Pro Eye）。
    *   包含两个阶段：首先是三人协作的航天器控制任务（用于评估领导力等社交特质），随后是个人决策任务（LCT）。
*   **样本量**：招募 57 名健康成年人，共 108 个实验 Session。最终分析包含 96 组行为数据、95 组瞳孔数据和 79 组 EEG 数据。
*   **对比基准**：以“客观等概率模型”（假设模糊区域高低回报概率各占 50%）作为基准，对比“主观信念模型”。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号或大规模算力消耗。由于主要涉及传统的信号处理（Butterworth 滤波、ICA、小波变换）和计算建模（PyDDM 框架），此类分析通常在标准工作站或高性能 CPU 服务器上即可完成。

### 5. 实验数量与充分性
*   **实验规模**：每位参与者完成 132 次有效决策试验。
*   **充分性评价**：
    *   **多维度验证**：实验不仅分析了行为选择，还通过瞳孔动力学和 EEG 频域特征进行了交叉验证。
    *   **统计严谨性**：采用了线性混合效应模型、Wilcoxon 符号秩检验（带 FDR 校正）以及 DDM 参数估计，确保了结果的统计可靠性。
    *   **客观性**：通过将个人决策策略与之前的协作任务（领导力评分）挂钩，证明了这种决策风格具有跨情境的稳定性，增加了研究的客观说服力。

### 6. 主要结论与发现
*   **信念驱动的异质性**：模糊规避并非统一偏差。激进型投资者持有“乐观”信念（主观 $k$ 值高），保守型持有“悲观”信念（主观 $k$ 值低）。
*   **生理信号追踪主观信念**：瞳孔唤醒水平（Arousal）并不直接追踪客观的模糊程度，而是追踪基于主观信念计算出的价值。当使用主观信念重新校准时，不同策略组间的生理差异消失了。
*   **神经动力学差异**：
    *   **理想型**：表现出强烈的后期额叶 β 波调制，反映了对决策冲突的控制。
    *   **激进型**：在决策前就表现出广泛的神经分化，具有更强的预备性状态。
    *   **保守型**：神经反应相对迟钝，主要表现为后部顶叶的 α/β 波调制。
*   **社交关联**：在个人决策中表现激进的人，在团队协作任务中往往获得更高的领导力评分。

### 7. 优点与亮点
*   **主观化建模**：成功将“模糊性”这一抽象概念量化为个体的主观信念参数 $k$，并证明了生理信号对该参数的敏感性。
*   **多模态闭环**：从行为分层到生理验证，再到计算模型模拟，形成了一个完整的解释链条。
*   **跨任务一致性**：将实验室内的博弈决策与复杂的团队协作特质（领导力）联系起来，提升了研究的生态效度。

### 8. 不足与局限
*   **模糊水平有限**：仅设置了 30% 和 60% 两个模糊梯度，可能无法完全覆盖现实中连续变化的模糊情境。
*   **EEG 空间分辨率**：受限于 EEG 的物理特性，无法精确定位参与模糊处理的具体深层脑区（如杏仁核或纹状体）。
*   **因果关系**：虽然建立了生理信号与信念的关联，但尚不能完全确定是生理状态决定了信念，还是信念产生了生理反应。
*   **VR 环境限制**：虽然 VR 增加了沉浸感，但头戴设备的重量和佩戴舒适度可能对长时间的 EEG 和瞳孔记录产生微小干扰。

（完）
