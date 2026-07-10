---
title: Humans integrate gaze and decision cues for inferring preferences in social interactions
title_zh: 人类在社交互动中整合注视和决策线索来推断偏好
authors: "Gopnarayan, M. N., Bavard, S., Stuchly, E., Gluth, S."
date: 2026-07-10
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737460v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 使用眼动追踪和层次推理模型，从注视和决策线索推断人类偏好
tldr: 社交互动中，推断他人隐藏偏好依赖行为线索。本研究通过多属性讨价还价任务和眼动追踪，发现买家接受率反映效用、拒绝速度体现信心、首注视指向高权重属性。卖家整合选择、反应时和注视信息调整出价，层次模型揭示其贝叶斯更新信念。注视虽未提升整体表现，但改变了注意策略。该工作揭示了人类从决策动态推断偏好的认知机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737460-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1660, \"height\": 693, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737460-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1493, \"height\": 1220, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737460-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1315, \"height\": 1758, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737460-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1333, \"height\": 934, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737460-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1717, \"height\": 714, \"label\": \"Figure\"}]"
motivation: 探究人类在实时社交中如何结合选择、反应时和注视等过程线索推断他人隐藏偏好。
method: 设计多属性讨价还价任务，采集75对买卖双方的决策、反应时和眼动数据，构建层次贝叶斯推断模型。
result: 买家接受率对应效用，拒绝速度指示决策信心，首注视偏向最高权重属性；卖家利用这些线索调整出价，但注视访问未改善整体收益。
conclusion: 人类通过贝叶斯方式整合多重决策过程线索推断偏好，注视信息改变了注意的使用方式，而非直接提升推断准确性。
---

## 摘要
社会决策依赖于从可观察行为中推断他人隐藏的偏好。然而，在实时互动中学习他人时，人类如何将选择与反应时间和注视等过程线索结合起来，仍不清楚。在这里，我们结合了一项新颖的多属性讨价还价任务与眼动追踪，并表明多个决策过程线索支持偏好推断。在75组买方-卖方配对中，买方的接受率追踪了报价效用，拒绝速度反映了决策信心，首次注视优先指向权重最高的属性。卖方利用选择、反应时间以及可用的注视线索调整后续报价。一个层级推断与选择模型表明，卖方在期望效用与期望信息获取之间取得平衡，并以贝叶斯方式更新其信念。尽管注视访问并未提高整体表现，但它改变了卖方使用注意信息的方式。这些发现揭示了人类如何在实时社交互动中从决策动态推断他人隐藏的偏好。

## Abstract
Social decision-making depends on inferring others' hidden preferences from observable behavior. Yet it remains unclear how humans combine choices with process cues such as response times and gaze when learning about others in real-time interaction. Here, we combine a novel multi-attribute bargaining task with eye-tracking and show that multiple decision-process cues support preference inference. Across 75 buyer-seller dyads, buyers' acceptance rates tracked offer utility, rejection speed reflected decision confidence, and first fixations preferentially targeted the highest-weighted attribute. Sellers adapted subsequent offers using choices, response times, and, when available, gaze cues. A hierarchical inference and choice model suggested that sellers balanced expected utility with expected information gain and updated their beliefs in a Bayesian manner. Although gaze access did not improve overall performance, it changed how sellers used attentional information. These findings shed light on how humans infer others' hidden preferences from decision dynamics in real-time social interaction.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：在实时社交互动中，人类如何整合选择行为、反应时间（RTs）和注视（gaze）等决策过程线索，来推断他人隐藏的偏好？  
- **研究动机**：以往研究已表明可以从选择中学习，但决策动态（反应时间、眼动）同样蕴含丰富信息。然而，在交互式、多轮次的社会情境中，人们如何动态地利用这些线索进行偏好推断尚不明确。  
- **整体含义**：揭示人类具有从决策过程信号“读心”的能力，对理解社会认知、设计人机交互系统具有启发意义。

## 2. 论文提出的方法论

### 核心思想
- 设计一个多属性讨价还价任务（multi-attribute bargaining task），让卖方通过观察买方的接受/拒绝决定、反应时间以及实时注视（注视组）来推断买方的属性权重，并据此调整后续报价。  
- 买方决策建模为漂移扩散模型（DDM），将效用映射为漂移率。  
- 卖方推理建模为**贝叶斯学习**：在离散权重网格上维持后验信念，每次观察后更新，并采用**信息-效用权衡**选择报价。

### 关键技术细节
- **买方模型（gaze-DDM）**：  
  效用 \( u = \mathbf{w}^\top \mathbf{x}_o \)，漂移率 \( v = v_{\text{coef}} (u - \mu) \)。边界分离 \( a \)，起始偏向 \( z_{\text{rel}} \)，非决策时间 \( t_{\text{er}} \)。注视序列用软max建模：\( P(a_\ell = i) \propto \exp(\alpha_\ell w_i + \nu \cdot I[\text{未注视}] ) \)，其中 \( \alpha_\ell = \alpha / (1 + \beta_\alpha (\ell-1)) \)。

- **卖方推理模型**：  
  后验更新：\( \tilde{p}_{t+1}(m) = p_t(m) L_t(m) / \sum p_t(m') L_t(m') \)，其中 \( L_t(m) = L_{\text{DDM},t}(m) \cdot [L_{\text{gaze},t}(m)]^\rho \)。  
  \(\rho\) 控制注视证据权重。  
  报价选择：\( V(o) = \lambda \cdot E[IG(o)] + (1-\lambda) \cdot E[U(o)] \)，\(\lambda\) 为信息-效用权衡参数。IG 基于拒绝后的熵减计算。

- **估计方法**：两阶段层次贝叶斯（NumPyro + NUTS采样），先估计买方参数，再固定其值估计卖方参数。

### 公式/算法流程（文字说明）
1. 买方根据隐藏权重计算报价效用，DDM产生接受/拒绝决策和RT。  
2. 在注视组，注视序列由基于权重的软max生成。  
3. 卖方观察到决策、RT和（可选）注视，通过贝叶斯公式更新对权重的后验。  
4. 卖方对每个候选报价计算期望效用和期望信息增益（基于假设拒绝后的熵减），加权得到综合价值，再由软max选择。

## 3. 实验设计

- **数据集/场景**：  
  - 75对买卖双方（共150名参与者），完成20个产品类别（如汽车、笔记本电脑），每个类别3个属性。  
  - 每个类别最多4轮报价，卖方从12个预定选项中选择。  
  - 买方权重分两种：**指导权重**（实验给出）和**自然权重**（买方自己报告）。  
- **基准/对比方法**：  
  - **注视组 vs 无注视组**：主要操纵变量，比较有无实时注视信息对卖方表现的影响。  
  - **自然权重 vs 指导权重**：比较权重来源对学习效率的影响。  
  - 卖方行为分析中，对比了基于仅选择 vs 结合RT和注视的学习效果。  
- 未使用其他外部方法（如AI模型）进行对比，仅对人类行为建模分析。

## 4. 资源与算力

- 论文中**未明确说明使用的GPU型号、数量、训练时长**等算力信息。  
- 所有计算基于层级贝叶斯估计，使用NumPyro的NUTS采样器（8条链，500热身+1000采样迭代），对个人计算机即可完成，未提及高性能计算资源。

## 5. 实验数量与充分性

- **实验数量**：主要实验75组配对，每组20个类别，每个类别最多4轮，总报价约6000次。眼动数据共7157个试次。  
- **统计检验**：多种回归模型（逻辑回归、线性混合模型）、t检验、效应量等，且有预注册（OSF）。  
- **充分性评价**：  
  - **覆盖全面**：分析了买方决策、RT、注视模式，卖方调整行为，以及分组差异。  
  - **模型验证**：层次贝叶斯提供了后验分布和可信区间，进行了后验预测检查。  
  - **缺点**：未做多重比较校正（但效应量较大），注视组和无注视组样本量接近（38 vs 37对），但个体的差异可能影响。总体上实验较充分、分析客观。

## 6. 主要结论与发现

1. **买方行为**：接受概率随效用递增（S形），拒绝速度反向反映效用；首次注视高度偏向最高权重属性（58% vs 33%随机），注视顺序比总注视时长更具诊断性。  
2. **卖方学习**：  
   - 成功利用选择结果：最终报价与卖方估计的相关性在接受后显著高于全部拒绝后。  
   - 利用RT：快速拒绝后卖方更大程度改变报价。  
   - 利用注视（注视组）：卖方将下一报价中首次注视属性的分数平均提高3.0分。  
3. **注视访问未提升整体收益**：注视组平均60.1分 vs 无注视组63.8分，差异不显著。  
4. **自然权重优势**：买方使用自然权重时，卖方报价效用显著高于指导权重。  
5. **计算建模**：卖方并非纯收益最大化，而是兼顾信息获取（λ > 0）；注视组中ρ显著大于零，表明卖家将注视作为证据。  

## 7. 优点

- **范式创新**：结合实时交互、多属性、动态信念更新和眼动追踪，生态效度高。  
- **多层次建模**：同时建模买方DDM和卖方贝叶斯推理，分离了信号产生和信宿理解过程。  
- **预注册**：明确假设和排除标准，增加可信度。  
- **分析全面**：既有人类行为统计，又有计算模型参数估计，提供机制理解。  
- **发现反直觉结论**：注视信息虽被策略使用但未提升最终收益，揭示了认知成本。

## 8. 不足与局限

- **实验覆盖**：仅3个属性、固定12个选项、最多4轮报价，限制了策略复杂性，可能低估信息寻求策略在长期互动中的价值。  
- **生态局限性**：无口头交流，真实谈判中语言信息可能压倒非言语线索。  
- **认知负荷**：注视组卖家可能因实时处理注视增加认知负担，导致收益未提升，但论文未独立测量认知负荷。  
- **样本量**：75对（150人）在个体差异研究中尚可，但对分组比较（注视 vs 无注视）可能偏小。  
- **偏差风险**：注视组中买卖双方可能意识到被观察，影响自然行为；但已通过“塑料手”程序降低身份识别。  
- **模型假设**：贝叶斯网格假设权重离散且固定，可能简化了真实权重分布的连续性。  
- **未与AI对比**：论文提到未来用于人机交互，但未提供与机器模型（如LLM）的对比实验。

（完）
