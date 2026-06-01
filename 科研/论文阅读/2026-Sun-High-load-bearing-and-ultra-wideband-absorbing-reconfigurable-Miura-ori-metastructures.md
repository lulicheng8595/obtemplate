---
title: High-load-bearing and ultra-wideband absorbing reconfigurable Miura-ori metastructures
authors: Chengtao Sun; Dawei Li; Wenhe Liao; Tingting Liu; Changdong Zhang; Yingzhi Xiong
journal: Composites Science and Technology
year: 2026
volume: 281
pages: "111658"
doi: 10.1016/j.compscitech.2026.111658
url: https://doi.org/10.1016/j.compscitech.2026.111658
tags:
  - 文献精读
  - Miura-ori
  - 可重构吸波超材料
  - FDM
  - 承载吸波一体化
  - 4D打印博士论文
status: 公开信息已读-全文待补
created: 2026-06-01
---

# High-load-bearing and ultra-wideband absorbing reconfigurable Miura-ori metastructures

## 题录核验

- 题名：High-load-bearing and ultra-wideband absorbing reconfigurable Miura-ori metastructures
- 作者：Chengtao Sun, Dawei Li, Wenhe Liao, Tingting Liu, Changdong Zhang, Yingzhi Xiong
- 期刊：Composites Science and Technology, Volume 281, 7 July 2026, Article 111658
- DOI：https://doi.org/10.1016/j.compscitech.2026.111658
- 官方页：https://www.sciencedirect.com/science/article/pii/S0266353826001430
- 作者主页核验：https://www.metastructure.tech/
- 注意：先前周报中写成“Penglin He et al.”不准确；ScienceDirect、作者主页和 RSC forward links 显示首作者为 Chengtao Sun。

## 阅读状态与边界

本笔记基于 ScienceDirect 官方页面可访问的摘要、引言片段、方法片段、总结片段、CRediT 信息，以及 ResearchGate 可见的图表上下文片段整理。当前本地项目、Zotero 数据库和 Zotero 附件目录均未找到该论文 PDF；ScienceDirect 全文需要机构权限。因此，下面对总体设计逻辑、关键性能指标和可借鉴写法可以直接使用，但具体几何参数、完整图表编号、实验样品尺寸、材料电磁参数曲线和补充材料数据需要拿到全文后复核。

## 一句话结论

这篇文章把 Miura-ori 刚柔折纸机构、FDM 一体化平面打印、CB/PLA 介电损耗材料和金属背板吸波单元结合起来，形成一种可折叠部署、被动保持、超宽带吸波且具有高承载能力的可重构电磁功能超结构。

## 核心问题

传统吸波材料或吸波超表面通常在制造后功能固定，难以适应动态服役环境。已有可重构吸波方案包括变容二极管、材料调制、微流控、升降、旋转、拉伸和折叠等，但工程应用中常见问题是带宽受限、结构稳定性不足、制备复杂或承载能力差。折纸吸波结构具有几何可重构优势，但许多已有工作依赖纸基或柔性薄膜涂覆损耗层，再通过压痕和手工折叠获得三维构型，机械强度、部署精度、折叠耐久性和被动保持能力都不够。

本文的目标是把“可重构电磁响应”和“承载结构”从两个分离问题变成同一个结构设计问题：通过刚性面板和柔性铰链形成 Miura-ori 机构，用 FDM 一次打印二维展开结构，再折叠组装为三维电磁功能面板。

## 设计路线

1. 几何层面：采用 Miura-ori 折纸拓扑，使二维平面结构可快速转化为三维周期结构。折叠角改变会改变空间几何、等效阻抗和电磁耦合路径。
2. 材料层面：使用 CB/PLA 复合丝材作为 FDM 打印材料。炭黑填充带来介电损耗，是吸收电磁波的主要耗散介质。
3. 制造层面：使用 Bambu X1-Carbon Combo 进行 FDM 单次构建，实现平面一体化制造，避免传统纸基涂覆、切割、手工折叠的工艺不稳定。
4. 电磁层面：金属背板使透射近似为零，吸收主要取决于反射损耗。结构通过几何参数与材料损耗协同，实现 2-40 GHz 超宽频响应。
5. 力学层面：刚柔折纸机制让结构在面内低载荷驱动下可部署，同时在边界约束下具备较高面外承载能力。

## 关键性能指标

- 工作频段：2-40 GHz。
- 吸收表现：93.9% 的频段内反射损耗低于 -10 dB。
- 入射稳定性：官方摘要指出具有良好的角度稳定性。
- 极化稳定性：官方摘要指出具有极化不敏感行为。
- 承载能力：在特定约束条件下可承受超过自重 6360 倍的载荷。
- RCS 缩减：通过折叠-装配构建电磁功能面板，最大 RCS reduction 达 27.3 dB。
- 仿真方法：使用 CST Studio Suite 2022 频域求解器；+z 方向为 open/add space，x/y 方向设为 unit cell；因金属背板存在，不考虑透射。

## 论文结构推断与重点图表

- 图形摘要：应展示从二维打印、折叠部署到三维吸波/RCS 降低应用的整体路线。
- Fig. 2：ScienceDirect 片段显示该图讨论 RMM 的刚柔设计和 FDM 制造策略。重点看 CB/PLA 平面打印、铰链/面板分区、折叠后的周期结构，以及“2D fabrication to 3D function”的证据链。
- Supplementary Fig. S1：ScienceDirect 片段提到 CB/PLA 复合丝材中高密度炭黑颗粒使其成为介电损耗介质。需要全文补读其微观形貌、电导率/介电常数/损耗角正切数据。
- Fig. 5e：ResearchGate 图表上下文显示该图比较 phi = 90°, 105°, 120° 时的名义应力-应变曲线。重点看折叠角如何改变初始刚度、峰值载荷和压缩响应。
- Fig. 5f：ResearchGate 片段显示 phi = 90° 结构峰值载荷最高，达到 1159.3（单位需全文核验）。重点看承载性能与折叠角的关系。
- Table 1：ResearchGate 片段显示该表比较已有 origami-based structures，突出本文在低载部署与高面外承载之间的综合优势。适合用于博士论文综述表格。
- Supplementary Table S1：ResearchGate 片段提到不同折叠角下结构高度投影面积，用于名义应力计算。全文补读时要核验 F/(pw) 与 Delta H/H 的定义和样品尺寸。

## 与博士论文第三至第五章的关系

### 第三章：吸波复合材料与结构协同设计

可借鉴其“损耗材料 + 几何超结构 + 金属背板”的吸波解释框架。它不是单纯优化材料复介电常数，而是通过折纸几何改变路径长度、局部共振/多重反射、阻抗匹配和损耗耗散。第三章中可以引用它支撑一个观点：增材制造吸波超材料的核心不是把吸波粉末填进基体，而是让材料损耗参数与结构尺度共同决定有效吸收带宽。

### 第四章：连续纤维增强/承载-吸波一体化复合材料

本文没有使用连续纤维增强，但它对“承载-吸波一体化”的论证非常有价值。它把承载能力放到吸波超结构同等重要的位置，强调折纸结构不仅是调谐机制，也能承担机械载荷。第四章可以对比你的连续纤维增强形状记忆复合材料：本文依赖刚柔折纸几何和 CB/PLA，而你的工作可进一步引入连续纤维铰链或面板增强，实现更高承载、更可控驱动和形状记忆恢复。

### 第五章：可重构/折纸/可编程电磁超结构

这是最直接对应的章节。本文说明 Miura-ori 的折叠角可以作为可编程几何自由度，折叠状态对应不同空间形貌和电磁响应。第五章可借鉴其叙事：先指出传统可重构吸波依赖电控/液控/材料相变，存在环境适应和结构稳定问题；再提出机械可重构折纸结构，以低成本、可部署和被动保持为优势；最后把 4D 打印或连续纤维形状记忆驱动作为进一步升级。

## 对自己课题的启发

1. 把“折叠角”写成电磁设计变量，而不是机械后处理变量。折叠角改变的是单元空间周期、等效厚度、入射波多次散射路径和局部电流分布。
2. 把“高承载”作为吸波超结构的必要服役指标。博士论文中可避免只报 RLmin 和 EAB，而加入压缩、弯曲、循环折叠、部署保持等指标。
3. 4D 打印升级点清晰：本文需要外部折叠/装配；你的工作可用连续碳纤维增强形状记忆聚合物实现电热驱动、自折叠、自锁定或可逆重构。
4. 材料升级点清晰：CB/PLA 适合 FDM 和介电损耗，但性能空间有限；可对比 rGO、MXene、Fe3O4、羰基铁、连续碳纤维等多损耗机制。
5. 写作中可突出“快速二维制造到三维电磁功能”的路线，这与 4D 打印的形变制造逻辑一致。

## 可直接借鉴的写作角度

- 从“固定功能吸波体”转向“几何可编程吸波超结构”。
- 从“吸波性能优化”转向“吸波-承载-部署-保持一体化”。
- 从“材料损耗主导”转向“材料损耗与折纸拓扑协同”。
- 从“手工折叠纸基吸波器”转向“增材制造刚柔一体折纸吸波器”。
- 从“电控可调”转向“机械可重构 + 被动保持”的低复杂度调控路线。

## 可写进论文的中文表述草稿

受 Miura-ori 折纸拓扑启发，Sun 等提出了一种 FDM 一体化制造的刚柔可重构吸波超结构。该结构利用 CB/PLA 复合材料的介电损耗特性和折纸构型的空间重构能力，在 2-40 GHz 范围内实现了超宽带电磁耗散，并在大部分频段保持反射损耗低于 -10 dB。同时，刚性面板与柔性铰链构成的折纸机构赋予结构低载部署和高面外承载能力，最大可承受超过自重 6360 倍的载荷。该研究表明，折纸几何不仅可以作为吸波响应调控手段，也可以作为承载-吸波一体化超材料的重要结构基础。

## 局限与待复核问题

- 需要全文核验 CB/PLA 的介电参数、填充率、打印参数和样品尺寸。
- 需要确认 2-40 GHz 吸收结果中仿真与实验的对应关系，尤其是自由空间测试设置和样品尺寸是否足以支撑低频段结果。
- 需要补读不同折叠角下的吸收曲线，判断可重构是否主要体现为带宽变化、峰位偏移还是角稳定性变化。
- 需要确认 6360 倍自重载荷是在何种边界约束、折叠角和加载方向下得到，避免在论文中泛化为任意服役工况。
- 需要确认 RCS reduction 的测试/仿真场景：入射角、极化、参考目标、面板阵列规模和频段。
- 需要核验循环折叠耐久性。如果没有循环数据，不能把“可重构”直接等同于长期可逆重构。

## 与已有本地文献的连接

- 可与本地 Zotero 中的 “Miura-ori based reconfigurable multilayer absorber for high-efficiency wide-angle absorption” 对比：前者偏多层宽角吸收，本文更强调 FDM 一体制造和承载。
- 可与 “4D printed continuous fiber-reinforced self-locking Miura-ori composites with high energy absorption” 对比：该文偏力学/能量吸收，本文偏电磁吸波；两者结合可构成第五章中“4D 打印连续纤维 Miura-ori 吸波结构”的理论支撑。
- 可与 Sun 等 2024 年 “Design of functionally gradient metastructure with ultra-broadband and strong absorption” 对比：同一团队从功能梯度吸波超结构推进到可重构折纸吸波超结构，体现了从静态结构优化到可部署功能结构的研究脉络。

## 精读优先级

拿到全文后优先读 Fig. 2、吸收曲线与参数扫描、Fig. 5e/f、Table 1 和 RCS 面板构建部分。对博士论文最有价值的是它的设计逻辑和指标体系，而不是单个 RL 峰值。

## BibTeX

```bibtex
@article{Sun2026MiuraRMM,
  title = {High-load-bearing and ultra-wideband absorbing reconfigurable Miura-ori metastructures},
  author = {Sun, Chengtao and Li, Dawei and Liao, Wenhe and Liu, Tingting and Zhang, Changdong and Xiong, Yingzhi},
  journal = {Composites Science and Technology},
  volume = {281},
  pages = {111658},
  year = {2026},
  doi = {10.1016/j.compscitech.2026.111658},
  url = {https://doi.org/10.1016/j.compscitech.2026.111658}
}
```
