---
title: "Judging the reasons for fixations: A direct experimental method to assess the contribution of saliency and semantic factors to gaze control"
title_zh: 判断注视的原因：一种直接实验方法评估显著性和语义因素对注视控制的贡献
authors: "Faul, F., Nuthmann, A."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.01.735892v1.full.pdf"
tags: ["query:gaze-intent"]
score: 6.0
evidence: 评估注视控制中显著性vs语义因素，对计算眼动模型有用
tldr: 关于显著性与语义对注视控制贡献的争论常依赖间接全局比较，但注视由异质局部原因引发，全局方法存在局限。本文采用直接方法，让参与者在高注视密度簇上明确判断注视原因，区分低层显著性与语义类别。结果表明语义通常主导显著性，抽象语义类别（如“未知/不寻常”）尤为重要。作者提出框架区分“高亮感兴趣位置”与“采样策略”，经典模型仅为受限输入，而深度学习模型（如DeepGaze IIE）更通用，其预测性能随注视原因变化较小。该工作揭示注视控制的局部异质性，为模型评估提供新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有间接全局比较方法无法区分注视的异质局部原因，需直接方法评估显著性与语义的贡献。
method: 让参与者在高注视密度簇上直接判断注视原因，分类为低层显著性或各类语义因素，并选出最重要因素。
result: 语义因素普遍主导显著性，抽象语义类别（“未知/不寻常”）重要；DeepGaze IIE性能随原因变化小于经典模型。
conclusion: 提出注视控制框架区分高亮和采样过程，深度学习模型隐含编码采样策略，更符合实际注视行为。
---

## 摘要
当前关于显著性与语义对注视控制相对贡献的争论，往往依赖于比较显著性和意义地图的预测能力。我们认为这种间接的全局方法存在根本性局限，因为注视源于异质的局部原因，这些原因在全场景比较中被混淆。为了证实这一观点，我们采用一种直接方法，让参与者明确识别高注视密度特定聚类处的注视原因，区分低层显著性与多种语义类别，并指出最重要的一个。获得的判断显示，多个因素同时贡献于注视控制。尽管其影响在不同注视聚类中有所变化，但语义通常主导显著性。值得注意的是，抽象语义类别，特别是“未知/不寻常”，被证明是重要的，突显了先验知识和新颖性除了个人相关性之外在引导注意中的作用。为了在现有模型背景下解释这些发现，我们提出一个框架，区分突出图像中感兴趣位置的过程与将信息转化为扫描路径的采样策略。在此框架内，经典显著性和意义地图被视为策略的受限输入，而基于深度学习的模型（如DeepGaze IIE）更普遍，也可能隐含编码了策略本身的方面。与此一致，我们发现DeepGaze IIE的预测性能随着注视的具体原因而变化的程度小于经典显著性和意义地图方法。

## Abstract
Current debates regarding the relative contribution of saliency versus semantics to gaze control often rely on comparing the predictive power of saliency and meaning maps. We argue that such indirect, global approaches are fundamentally limited because fixations arise from heterogeneous, local causes that are conflated in whole-scene comparisons. To substantiate this claim, we used a direct method where participants explicitly identified the reasons for fixation at specific clusters of high fixation density, distinguishing between low-level saliency and various semantic categories, as well as the most important one. The obtained judgments revealed that multiple factors contribute simultaneously to gaze control. Although their influence varied across fixation clusters, semantics generally dominated saliency. Notably, abstract semantic categories, particularly "unknown/unusual," proved important, highlighting the role of prior knowledge and novelty besides personal relevance in guiding attention. To interpret these findings in the context of existing models, we propose a framework distinguishing between processes highlighting interesting locations in the image from a sampling strategy translating this information into scanpaths. Within this framework, classic saliency and meaning maps are viewed as restricted inputs to the strategy, whereas deep learning-based models (e.g., DeepGaze IIE) are more general and may also implicitly encode aspects of the strategy itself. Consistent with this, we found that the predictive performance of DeepGaze IIE varied less significantly with the specific reasons for fixation than that of classic saliency and meaning map approaches.