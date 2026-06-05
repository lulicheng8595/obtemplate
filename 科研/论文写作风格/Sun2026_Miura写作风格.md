# Sun 2026 Miura-ori 论文叙事风格档案

适用场景：后续撰写 4D 打印、连续纤维增强、折纸/可重构吸波、承载-吸波一体化、RCS 调控相关 SCI 论文时，优先采用这种叙事风格。这里保存的不是某几句表达，而是整篇文章的组织方式：如何安排图、如何解释结果、如何写每个 Results 小节、如何讨论贡献边界。

## 1. 整篇文章的叙事节奏

这类文章的叙事不是“材料制备-性能测试-应用展示”的流水账，而是把结构设计写成一个逐步展开的功能系统。每一节都回答一个明确问题，并自然引出下一节。

推荐节奏：

1. 先用概念图建立系统：这个结构为什么存在，它同时处理哪些需求。
2. 再讲结构如何实现：材料、几何、铰链/纤维路径、制造工艺和可调参数。
3. 再讲基础性能：材料是否能耗散电磁波，结构是否能承载，形态是否能稳定。
4. 再讲核心功能：折叠角或锁定形态如何改变吸波响应。
5. 再讲阵列或应用级功能：单元状态如何扩展到 RCS 或散射调控。
6. 最后讨论边界：它不是万能结构，而是在特定材料-结构-几何耦合下建立了一个可扩展设计策略。

写作时应始终让读者感觉：每一步不是为了多放一个测试，而是为了证明“结构形态可以成为电磁功能变量”。

## 2. 每个 Results 小节的长度与内部结构

Sun 这类文章的小节通常不宜过短。每个 Results 小节应围绕一张主图展开，正文长度建议为 4-7 个自然段；如果图很复杂，可以 6-8 段，但不能变成逐 panel 清单。

推荐小节结构：

- 第 1 段：提出本小节主问题或主 claim。长度约 120-180 中文字，或英文 80-120 words。
- 第 2 段：解释结构/实验/图中设计。说明为什么这些 panel 能回答该问题。
- 第 3-4 段：描述关键结果。每段围绕一类证据，不要一段塞满所有 panel。
- 第 5 段：解释机制。把现象连接到材料、几何、载荷路径、局域场或散射行为。
- 第 6 段：收束并引出下一节。说明这个结果为下一张图或下一功能验证提供了基础。

一个小节最好只有一个中心句。例如：

- Fig. 2 小节：打印结构同时提供力学、电热和电磁基础。
- Fig. 3 小节：折叠角状态可以被激活、设定并锁定。
- Fig. 4 小节：锁定折叠角改变吸波峰位和带宽。
- Fig. 5 小节：角度状态可组织为空间编码阵列来调控后向散射。

## 3. 图片解读风格

图的解读顺序应为：先讲整张图的 scientific job，再讲关键 panel，最后讲图中证据支撑的机制。不要从 “Fig. 2a shows..., Fig. 2b shows...” 开始堆面板。

推荐写法：

1. 先定义整张图的作用：
   “To establish the structural basis for load-bearing and electromagnetic modulation, we first examined ...”

2. 再把 panel 分组，而不是逐个报账：
   - 结构/工艺 panel：说明样品如何制造、结构如何形成。
   - 参数/几何 panel：说明哪些变量可调。
   - 性能 panel：说明它能承载、吸波或重构。
   - 机制 panel：说明为什么会出现这些性能。

3. 每张图保留 1-2 个主数字在正文中，其余数字放图注或补充材料。

4. 对图的解释必须从可见证据出发，不把图没有证明的机制写成定论。

例如，读结构设计图时，不仅要说“展示了 Miura-ori 结构”，还要说：

- 结构：刚性面板、柔性铰链、折纸单元如何构成。
- 参数：折叠角、厚度、周期、面板尺度中哪些是可调变量。
- 工艺：FDM 或 4D 打印如何把二维展开结构转为三维形态。
- 应用价值：这些结构特征如何服务吸波、承载或可编程散射。

这是用户已经明确喜欢的结构图判断：一张好的设计图必须同时交代 **结构、参数、应用价值、工艺**。

## 4. 结果解释风格

结果解释要分三层，不能停在现象描述。

第一层：观察到什么。

- 反射损耗曲线发生峰位迁移。
- 折叠角改变有效吸收带宽。
- 压缩载荷下结构保持稳定。
- 编码阵列降低后向 RCS。

第二层：这说明什么直接结论。

- 折叠角可以作为电磁响应调节参数。
- 结构几何不仅影响形状，也影响等效厚度和局域耦合。
- 承载路径与吸波结构没有完全分离，而是在同一构型中协同存在。

第三层：机制解释是什么。

- 材料损耗提供能量耗散基础。
- 折纸几何改变入射波传播路径、多重反射和局域场分布。
- 形态锁定使响应不依赖持续外场维持。
- 阵列中不同折叠角单元改变局部反射幅度/相位，从而重排远场散射。

写结果解释时，优先使用这种链条：

**measured/simulated phenomenon -> structural variable -> physical mechanism -> design implication**

不要只写“the structure shows excellent absorption”。应写：

“The shift of the absorption peak with folding angle indicates that the electromagnetic response is governed not only by the lossy composite but also by the reconfigured propagation path and effective thickness. Therefore, the folding morphology can be treated as a programmable design variable rather than a passive deployment state.”

## 5. Discussion 写法

Discussion 不要重新复述所有结果，而要完成三个任务：

1. 把核心推进说清楚：本文把什么从材料属性转化成了结构变量。
2. 和最接近文献比较：不是简单说性能更好，而是说设计逻辑不同。
3. 主动承认边界：驱动方式、可逆性、角度精度、大面积阵列、循环稳定性、RCS 实验验证等。

推荐 Discussion 顺序：

- 第一段：一句话总结设计策略和主要发现。
- 第二段：与固定吸波材料、传统可重构吸波器、已有折纸吸波器对比。
- 第三段：强调本文的机制贡献，例如形态锁定、连续纤维路径、形态编码。
- 第四段：讨论工程意义，例如可展开电磁防护、低可探测外壳、多频段吸波构件。
- 第五段：诚实写局限和未来工作。

Discussion 的语气要稳，不要像宣传稿。强 claim 必须接证据；弱 claim 用 “suggests”, “indicates”, “provides a route”, “may enable”。

## 6. 引言叙事逻辑

推荐顺序：

1. 从工程需求进入：吸波结构正在从附加涂层转向承载型、可部署、可适应动态电磁环境的结构单元。
2. 指出现有固定吸波体系的不足：频段固定、形态固定、承载贡献有限、难以适应复杂姿态/入射角/频率捷变环境。
3. 引入可重构超材料/折纸结构作为解决路径：几何重构可以改变等效厚度、传播路径、局域场和散射分布。
4. 继续收窄 gap：已有可重构吸波器依赖电子元件、液晶、外部驱动或薄膜折纸，往往在承载、形态保持、制造稳定性和工程集成方面不足。
5. 引出自己的方案：连续纤维增强 4D 打印折纸结构，把载荷传递、电热激活、形态锁定和微波耗散放进同一结构体系。
6. 贡献句不要泛泛说“提出了一种新材料”，而应说“将折叠角/锁定形态转化为承载型吸波结构中的可编程电磁设计变量”。

## 7. 句式偏好

优先使用这类句式：

- “This design converts ... into ...”
- “The folding angle therefore serves as ... rather than ...”
- “Unlike ... that rely on ..., the present strategy ...”
- “This result indicates that ... is not merely ..., but also ...”
- “The comparison highlights that the key advance is not ..., but ...”
- “By locking the programmed morphology, the structure maintains ... without continuous external input.”
- “The observed response can be attributed to ..., which modifies ... and consequently ...”
- “This section establishes the structural basis for the subsequent electromagnetic modulation.”

中文草稿中可对应写成：

- “该设计将……转化为……”
- “因此，折叠角不再只是结构外形参数，而是……”
- “不同于依赖……的可调吸波器，本文策略通过……”
- “该结果说明，连续纤维并非仅作为增强相，而是……”
- “这一比较表明，本文的关键推进不在于单一吸收峰值，而在于……”
- “该响应可归因于……，其改变了……并进一步导致……”
- “本节为后续电磁调控验证建立了结构基础。”

## 8. 需要避免的写法

- 避免一上来写“随着科技发展……”这类泛泛开头。
- 避免把“多功能”当作自明优点，必须拆成承载、吸波、形态锁定、电热激活、RCS 调控等具体功能。
- 避免用 “excellent/remarkable/superior” 替代证据。
- 避免把仿真 RCS 写成实验事实。
- 避免把有限离散角度状态过度写成连续可编程。
- 避免让引言承诺强于 Results 证据。
- 避免每段都以 Fig. xa, Fig. xb 开头，读起来会像图注扩写。
- 避免一个小节过短，导致结果缺少机制解释；也避免一个小节过长，混入多个 claim。

## 9. 用于当前 SCI 稿件的核心表述

推荐贡献句：

“Here, we develop a continuous-fiber-reinforced 4D-printed origami metastructure in which the locked folding morphology serves as a programmable electromagnetic design variable. The continuous fibers provide both load-transfer pathways and Joule-heating channels, while the rGO/FCI/PLA matrix enables microwave loss and shape-memory fixation. This coupling allows load-bearing origami structures to switch microwave absorption across radar-relevant bands and to organize morphology-coded arrays for scattering suppression.”

中文对应：

“本文提出一种连续纤维增强的 4D 打印折纸电磁超结构，将锁定折叠形态作为可编程电磁设计变量。连续纤维同时提供载荷传递路径和焦耳热激活通道，rGO/FCI/PLA 复合基体则提供微波损耗和形状记忆固定能力。该材料-结构耦合使承载型折纸结构能够在多个雷达相关频段之间调节吸波响应，并进一步组织为形态编码阵列以实现后向散射抑制。”

## 10. 后续使用规则

当用户要求撰写或改写 4D 打印吸波/折纸/连续纤维相关论文时，先调用本档案。除非用户明确要求换风格，否则默认采用这种叙事方式：

**工程需求 -> 现有方案限制 -> 结构策略 -> 图中证据 -> 机制解释 -> 设计意义 -> 边界讨论**

对于 Results，每个小节默认控制在 4-7 段，每段围绕一个功能或证据层级展开。对于图片解读，默认先问用户这张图承担什么 claim，再共同确定哪些 panel 支撑 claim，最后再写入正文或笔记。