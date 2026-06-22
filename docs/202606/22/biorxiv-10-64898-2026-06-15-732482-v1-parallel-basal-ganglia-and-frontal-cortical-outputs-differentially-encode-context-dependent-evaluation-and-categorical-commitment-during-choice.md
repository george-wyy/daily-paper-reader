---
title: Parallel basal ganglia and frontal cortical outputs differentially encode context-dependent evaluation and categorical commitment during choice
title_zh: 基底神经节和额叶皮层并行输出在抉择过程中差异编码情境依赖评估与分类承诺
authors: "Yoshida, A., Krauzlis, R., Hikosaka, O."
date: 2026-06-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732482v1.full.pdf"
tags: ["query:gaze-intent"]
score: 8.0
evidence: 决策任务中眼动选择的神经编码
tldr: 决策需要将选项评估转化为具体行动承诺。本研究通过记录猴子执行顺序选择任务时黑质网状部（SNr）和额叶眼动区（FEF）的神经元活动，发现SNr编码基于顺序等级的上下文依赖评估，而FEF编码接受/拒绝的分类承诺。多变量分析表明，SNr活动最佳解释变量为顺序等级，FEF为分类承诺。结果揭示了平行基底节和额叶输出通路在决策中的分工。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究评估选项到行动承诺的神经转换机制是否在基底节和额叶通路中分工。
method: 猴子执行部分分离顺序等级与分类承诺的任务，记录SNr和FEF神经元活动并多变量建模。
result: SNr活动由顺序等级主导，FEF由分类承诺主导，且跨猴子一致。
conclusion: 平行基底节和额叶输出分别处理上下文评估与分类承诺，协同指导选择。
---

## 摘要
适应性选择需要将可用选项的评估转化为对特定行动的承诺，但理解这种转化如何在神经回路中实现仍是一个核心挑战。我们记录了黑质网状部（SNr）和额叶眼动区（FEF）中分离良好的神经元，这两个区域向丘上体发送并行投射以驱动眼动选择，同时猴子执行顺序提议选择任务，该任务旨在部分分离场景定义的顺序排名与分类承诺。在目标出现前，SNr显示出比FEF更强的场景相关调制。在目标评估期间，SNr活动在行为结果间显示出以顺序排名为主的有序调制，而FEF活动则分类地区分接受与拒绝，并强烈编码目标方向。行为模型分解揭示，仅顺序排名就能最好地解释SNr活动，其表现优于奖励幅度甚至一个结合了排名、奖励、场景背景和等待成本的复合可接受性度量，而FEF活动则最好地由分类承诺解释。这种分离在多变量建模、单神经元响应模式以及所有三只猴子中一致。总之，这些发现支持了一种分工，即情境依赖评估和分类承诺分布在并行基底神经节和额叶皮层输出通路中，以有效指导自主选择。

## Abstract
Adaptive choice requires transforming the evaluation of available options into commitment to a specific action but understanding how this transformation is implemented across neural circuits remains a central challenge. Here we recorded well-isolated neurons in the substantia nigra pars reticulata (SNr) and frontal eye field (FEF), which send parallel projections to the superior colliculus for driving the eye movement choice, while monkeys performed a sequential-offer choice task designed to partially dissociate scene-defined ordinal rank from the categorical commitment. Before target onset, SNr displayed stronger scene-related modulation than FEF. During target evaluation, SNr activity showed ordered modulation across behavioral outcomes dominated by ordinal rank, whereas FEF activity categorically separated acceptance from rejection and strongly encoded target direction. Behavioral model decomposition revealed that ordinal rank alone best explained SNr activity, outperforming both reward magnitude and even a composite acceptability measure that incorporated rank together with reward, scene context, and waiting cost, whereas FEF activity was best explained by categorical commitment. This dissociation was consistent across multivariable modeling, single-neuron response patterns, and all three monkeys. Together, these findings support a division of labor in which context-dependent evaluation and categorical commitment are distributed across parallel basal ganglia and frontal cortical output pathways to efficiently guide voluntary choices.

---

## 论文详细总结（自动生成）

好的，遵照您的要求，以下是基于您提供的论文详细内容，以 Markdown 格式生成的详细中文总结。

### 论文核心总结：情境依赖评估与分类承诺在基底神经节和额叶皮层输出通路中的差异编码

#### 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：适应性决策需要将“对选项的评估”（Evaluation）转化为“对特定行动的承诺”（Commitment）。然而，这种转换的神经机制尚不明确。本研究旨在探究负责将信息传递到下游运动中枢（上丘, SC）的两条并行通路——基底神经节（黑质网状部, SNr）和额叶皮层（额叶眼动区, FEF），是否在此过程中扮演不同的计算角色。
- **背景与动机**：以往研究认为SNr主要参与运动门控（通过去抑制），而FEF与目标选择和运动发起有关。但“评估”和“行动”在很多任务中难以区分（例如，接受好的选项，拒绝坏的选项）。本研究利用一个巧妙的实验范式，将场景定义的“顺序等级”（Rank）和“分类承诺”（Commitment）部分解耦，从而首次直接在输出结构层面检验这两个区域的编码差异。
- **整体含义**：该研究揭示了决策过程中的一种“劳动分工”：**SNr主要传递情境依赖的、基于顺序等级（好/坏）的评估信号，而FEF主要传递分类性的（接受/拒绝）承诺信号以及运动方向信号**。这两种信号在SC中汇合，共同指导最终的行动。

#### 2. 方法论

- **核心思想**：设计一个行为任务，能够将“选项在情境中的相对价值（顺序等级）”与“最终的行动承诺（接受/拒绝）”分离开来，然后分析SNr和FEF的神经元活动编码的是哪个方面的信息。
- **关键技术细节与流程**：
    1.  **任务设计**：猴子执行一个“顺序提议选择任务”。背景场景定义了当前可选的对象对（例如，场景1：A vs. B），从而定义了对象在该场景下的“好坏”（顺序排名，Rank）。
    2.  **解耦的关键**：
        - 接受坏选项（Accept Bad）：在奖励差异小的场景中，猴子有时会接受低排名的对象，这实现了“接受承诺”但“低排名”的解耦。
        - 拒绝坏选项（Reject Bad）：猴子通过主动的“回归扫视”（Return Saccade）来拒绝，而非简单的不动，这定义了“拒绝承诺”也是一种主动行动。
    3.  **神经记录**：在三只猴子执行任务时，同时记录来自黑质网状部（SNr）和额叶眼动区（FEF）的单个神经元活动。
    4.  **数据分析模型**：
        - **线性混合效应模型**：对任务期（场景期、目标期）的神经元活动进行统计分析，分离不同变量的贡献。
        - **多变量线性混合效应模型**：将神经元活动建模为行动（Action，接受/拒绝）、排名（Rank，高/低）、奖励量（Reward amount）和方向（Direction）的函数，量化各变量的独立贡献。
        - **行为模型分解**：先拟合一个逻辑回归模型，找出影响猴子决定接受/拒绝的四个因素（奖励量、场景价值差、先前拒绝次数、顺序排名）。然后从这个最佳行为模型中提取出“可接受性评分”（Margin）。最后，用AIC（Akaike信息准则）等模型比较方法，检验SNr和FEF的神经元活动更能由“排名”还是“可接受性评分”来解释。
- **核心指标**：AIC值（用于模型选择，越小越好）、偏η²（效应大小）、偏R²（方差解释率）、回归系数β。

#### 3. 实验设计

- **数据集**：来自3只雄性恒河猴在行为任务中的神经元发放数据。
- **场景设置**：
    - **选择场景** (Scenes 1-6): 每个场景对应一个对象对，定义了高低排名。猴子可以自由接受或拒绝。
    - **强制选择场景** (Scenes 7-10): 作为控制条件，每次只提供一个对象，猴子只能接受。
- **基准对比**：
    - **区域对比**：主要对比黑质网状部（SNr）和额叶眼动区（FEF）两个脑区。
    - **变量对比**：对比“行动（Action）”、“排名（Rank）”、“奖励量（Reward）”和“可接受性评分（Margin）”等不同变量解释神经元活动的优劣。
- **对比方法**：通过多变量线性混合效应模型和行为模型分解，系统地比较了不同任务变量对神经元活动的解释力。

#### 4. 资源与算力

- 论文中**未明确提及**使用的GPU型号、数量或训练时长。
- 分析方法主要基于R和Python的统计建模（如线性混合模型、逻辑回归），这些计算通常在标准CPU上即可完成，对高性能GPU算力依赖不高。

#### 5. 实验数量与充分性

- **实验数量**：
    - 记录了**91个SNr神经元**和**99个FEF神经元**。
    - 行为数据包含了三只猴子在所有10个场景下数以万计的试验（trials）。
    - 分析层面包括：群体水平、单神经元水平、以及三只猴子的个体水平。
- **充分性评估**：
    - **非常充分和公平**：
        1.  **多维度验证**：结论在群体水平（图2、3）、模型水平（图4、5）和单神经元水平（图6）得到一致性验证。
        2.  **跨个体一致性**：三只猴子的结果均支持相同的结论，有力地排除了个体差异的干扰（图5E）。
        3.  **控制实验**：设置了强制选择任务作为控制条件，排除了视觉输入或运动执行差异对结果的干扰（图S6, S7）。
        4.  **严格的统计检验**：使用了线性混合效应模型、多重比较校正（Bonferroni, Holm）、排列检验和AIC模型选择等严谨的统计方法。
        5.  **模拟恢复分析**：通过模拟数据验证了AIC模型比较方法能够可靠区分“分级”和“分类”编码，证明了分析方法的有效性（方法与结果部分）。

#### 6. 主要结论与发现

- **功能分离的基本格局**：SNr和FEF编码了不同的决策变量。
- **SNr主要编码情境依赖的顺序排名**：
    - 目标出现前，SNr对场景（即当前的选择集合）有更强的敏感性。
    - 目标评估期间，SNr的活动在不同行为结果间呈现有序变化（接受好选项<接受坏选项<拒绝坏选项），“排名”是其主导编码变量（β = -0.64），其解释力远超“行动”、“奖励量”甚至整合了多因素的“可接受性评分”。这表明SNr传递的是一个简化的、情境相关的“好/坏”比较信号。
- **FEF主要编码分类性的行动承诺和运动方向**：
    - FEF的活动在接受好选项和接受坏选项时相似，但与拒绝坏选项截然分开，清晰地编码了“接受 vs. 拒绝”这一分类承诺。
    - 多变量模型显示，“方向”（β = 0.66）和“行动”（β = 0.35）是FEF活动的两大主导变量，而“排名”的贡献几乎为零。
- **层级化的神经计算模型**：研究结果支持一个三层次框架：（1）**行为层面**，决策整合了多种因素（由“可接受性评分”反映）；（2）**基底节输出**，SNr主要提取并传递“顺序排名”这一单一关键评估信号；（3）**额叶皮层输出**，FEF则将评估结果兑现为“行动承诺”和“空间方向”信号。两者在运动执行中枢（上丘）汇合。

#### 7. 优点

1.  **精妙的实验范式**：成功设计了能够将评估与承诺部分分离的任务（通过接受低排名选项和主动拒绝扫视），这是整个研究的基石。
2.  **直接比较并行输出通路**：直接在SNr和FEF这两个向共同目标（上丘）发送直接输出信号的脑区进行记录和比较，为该领域的劳动分工假说提供了直接证据。
3.  **严谨的多层次分析**：综合运用多变量建模、行为模型分解、单神经元分类等多种分析方法，从不同角度交叉验证了核心结论，增加了结果的可信度。
4.  **跨个体一致性**：在全部三只猴子中均观察到一致的分离模式，极大地提升了结论的普适性。
5.  **控制实验和模拟验证**：通过强制选择任务和模拟恢复分析，严谨地排除了混淆变量，并验证了自己分析方法的可靠性。

#### 8. 不足与局限

1.  **相关性，非因果性**：研究基于相关性记录，无法证明SNr/FEF的特定编码模式是否为决策的必要或充分条件。
2.  **缺乏同时记录**：没有同时记录上丘（SC）的神经元活动，因此关于两种信号如何在最终共同靶标（SC）中整合的结论仍是一种推测。
3.  **“排名”信号的来源**：研究表明SNr编码“排名”，但该信号的上游来源（如尾状核）及具体机制（直路/间接通路）尚待后续因果实验（如光遗传或药理抑制）来验证。
4.  **场景期分析的局限性**：对场景期的调制分析，未能完全区分场景身份（视觉特征）和其定义的奖励结构（价值背景），因此被保守地解释为“场景相关”调制。
5.  **单神经元分类的局限性**：单神经元分类基于对平滑的时域系数的时间点配对t检验，非独立样本，因此该方法被作者自己界定为“描述性总结”而非“正式统计推断”，其分类比例不应被过度解读。
6.  **任务范式的局限**：“排名”指代的是在该任务设置的特定场景下的顺序位置，其范围窄于经济学中一般的“价值”。研究结论是否适用于更广泛的、价值连续变化的决策情境，仍有待检验。

（完）
