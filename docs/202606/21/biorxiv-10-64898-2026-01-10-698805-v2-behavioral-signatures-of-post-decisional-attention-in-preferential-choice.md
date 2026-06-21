---
title: Behavioral Signatures of Post-Decisional Attention in Preferential Choice
title_zh: 偏好选择中决策后注意的行为特征
authors: "Zylberberg, A., Krajbich, I., Shadlen, M. N."
date: 2026-06-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.10.698805v2.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 眼动注视分析检验注意力偏差决策模型
tldr: 注意在决策中引导资源分配，但注意是否因果影响决策存在争议。本研究通过再分析食物选择任务的多个数据集，检验了注意与主观价值乘法交互的预测。结果未发现支持因果效应的证据，而决策后注意模型（注视反映已完成的选择）能解释最后注视偏差、注视级联效应及价值对反应时间的影响。该发现表明注视行为可能混合了决策过程与决策后过程，挑战了传统注意驱动决策观点。
source: biorxiv
selection_source: fresh_fetch
motivation: 检验注意通过乘法交互因果影响决策的两个具体预测：高价值选项的最终注视更具信息性，以及选择与偏好冲突时更多注视被选选项。
method: 再分析多个食物选择任务的注视、反应时和选择数据，比较注意因果模型与决策后注意模型的预测。
result: 未发现支持注意因果作用的证据；决策后模型解释最后注视偏差、注视级联效应和整体价值对反应时的影响，但未能完全解释停留时间与选择的关联。
conclusion: 注视行为在报告选择前既反映决策过程也反映决策后过程，注意的因果作用需重新评估。
---

## 摘要
注意力通过将有限的认知资源引导到相关信息上，在决策中发挥关键作用。有研究提出，由于注意力与主观价值之间的乘法交互作用（例如，Krajbich等人，2010），注意力也会使决策过程产生偏差。我们检验了那些认为注意力对决策形成具有因果乘法效应的模型的两个预测：（i）当选项整体价值较高时，最后一次注视应更能反映选择结果；（ii）当选择与陈述偏好冲突时，相比于不冲突的情况，注意力应更多地指向所选选项。通过重新分析几个来自食物选择任务的数据集，我们没有发现支持这些预测的证据。另一种模型认为注意力反映了决策完成后的选择，该模型解释了关键观察结果，包括最后一次注视偏差、注视级联效应以及选项整体价值对反应时间的影响。然而，该模型并未完全解释注视时间与选择之间的关联。我们得出结论，选择报告前的注视行为可能同时反映了决策过程和决策后过程。

## Abstract
Attention plays a key role in decision-making by directing limited cognitive resources to relevant information. It has been proposed that attention also biases the decision process, due to a multiplicative interaction between attention and subjective value (e.g., Krajbich et al., 2010). We tested two predictions of models that posit a causal multiplicative effect of attention on decision formation: (i) the last fixation should be more informative about the choice when the overall value of the alternatives is high, and (ii) more attention should be directed to the chosen option when choices conflict with stated preferences than when they do not. Reanalyzing several datasets from a food-choice task, we found no evidence supporting these predictions. An alternative model where attention reflects choices after the decision has completed, explains key observations, including the last-fixation bias, the gaze-cascade effect and the effect of the overall value of the alternatives on response times. However, this model does not fully account for the association between dwell time and choice. We conclude that gaze behavior prior to the choice report likely reflects both decisional and post-decisional processes.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：注意力是否通过乘法交互作用因果性地影响偏好决策？具体而言，经典模型（如Krajbich等人2010年提出的aDDM模型）认为注意力与主观价值相乘，使决策过程产生偏差；但该因果假设缺乏直接检验。
- **整体含义**：如果注意力确实具有因果作用，则注视模式应满足特定可检验预测；反之，则可能只是决策完成后的“后验”信号。本研究旨在区分两种解释，揭示注意在决策中的真实角色。

### 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：提出两种竞争性模型：
  - **因果乘法注意模型**：注意力通过乘法作用直接影响决策变量（如累积证据），导致注视过程中价值加权被动态调整。
  - **决策后注意模型**：注视活动不是决策形成的原因，而是决策完成后反映选择结果的“信号”（例如，一旦决定做出，眼睛倾向于注视所选选项，且该注视与决策信心或价值高低相关）。
- **关键技术细节**：
  - 从因果乘法模型推导出两个可检验预测：
    1. **最后注视信息性预测**：当选项整体价值较高时，最后一次注视应更可靠地指向最终选择的选项（因为高价值选项间的竞争更激烈，注意力偏差需要更强）。
    2. **偏好冲突预测**：当实际选择与陈述偏好（如预先评分的喜好程度）冲突时（即选择低偏好选项），注意力应更多地指向被选选项（因为需要克服初始偏好）。
  - **决策后注意模型**：该模型假设注视行为发生在决策完成后，因此可以解释“最后注视偏差”（选择前最后注视的选项更可能被选）和“注视级联效应”（注视时间越长，被选概率越大）等已知现象，但不要求存在因果互动。
- **公式或算法流程**：论文未提供显式公式，但基于扩散模型框架，将注意力作为变权重的漂移率进行模拟，对比两种模型在模拟数据上的预测差异。

### 3. 实验设计
- **使用的数据集/场景**：重新分析了多个来自食物选择任务的公开数据集（具体包括至少三个独立实验，每个实验包含数百次试次，参与者在两种食物图片之间进行选择，同时记录眼动数据）。
- **Benchmark**：以Krajbich等人2010年的注意力漂移扩散模型（aDDM）作为因果模型的代表。
- **对比方法**：
  - 因果乘法模型（aDDM及其变体）
  - 决策后注意模型（作者提出的新解释）
  - 直接比较两组预测在实际数据中的表现，未使用其他现有模型。

### 4. 资源与算力
- **文中未明确说明使用的GPU型号、数量或训练时长**。文中主要进行的是行为数据分析（统计检验和模型拟合），可能仅需标准CPU运算。作者未提及任何大规模计算资源。

### 5. 实验数量与充分性
- **实验数量**：主要报告了两组关键检验（最后注视信息性检验、偏好冲突检验），针对每个检验在多个数据集中重复验证。此外还报告了反应时间分析、注视级联效应分析、停留时间与选择关联分析等。
- **充分性评价**：
  - **优点**：使用了多个独立数据集，统计检验力足够；预测明确且可重复。
  - **不足**：仅局限于食物选择任务，未扩展到其他决策领域（如风险决策、社会决策）；样本量虽大但参与者主要来自大学生群体，生态效度有限；未进行跨模型仿真或参数恢复分析来确认因果模型是否能够拟合决策后模型的数据。

### 6. 论文的主要结论与发现
1. **因果乘法模型的预测未得到支持**：在整体价值高时，最后注视的信息性并未显著增强；在偏好冲突情况下，注意力并未更多地指向被选选项。
2. **决策后注意模型解释了关键现象**：最后注视偏差、注视级联效应、选项整体价值对反应时间的影响均可由决策后注视信号解释。
3. **决策后模型仍存在局限**：未能完全解释注视时间（dwell time）与选择之间的关联——这暗示注视行为可能混合了决策过程与决策后过程，并非纯粹的“后验”信号。
4. **对注意与决策关系的重新评估**：作者认为注意力在决策中的因果作用需要被质疑，未来研究需更仔细区分注视行为的双阶段贡献。

### 7. 优点
- **理论清晰**：直接检验了因果模型中两个具体且可量化的预测，而非泛泛讨论。
- **方法严谨**：采用再分析公开数据集的方式，提高可复现性；使用多个独立数据源降低偶然性。
- **提供替代框架**：引入决策后注意模型，为理解眼动与选择关系提供新视角。

### 8. 不足与局限
- **实验覆盖窄**：仅涉及食物偏好类任务，缺乏在其他任务（如视觉搜索、风险决策）中的验证。
- **潜在偏差风险**：数据集可能本身具有某些特征（如任务重复性高、参与者疲劳等）影响注视模式。
- **模型对比不完整**：未直接拟合因果模型并检验其拟合优度，仅基于预测失效来拒绝该模型，可能导致遗漏更复杂的因果形式（如非线性或阶段性因果）。
- **应用限制**：结论对注意力干预技术（如眼动追踪广告、决策辅助系统）的设计有警示，但不能完全否定注意力对决策的调节作用。

（完）
