# Platform Strategy & Risk Control

**互联网平台策略与风险控制知识库**

Advertising Strategy · Content Strategy · Risk Control · Decision Systems · Experimentation

本项目围绕互联网平台的三类策略问题展开：**如何分配有限流量、如何维持内容生态质量、如何识别并处置风险**。在共同的方法论层面，讨论策略产品、规则引擎、模型评分、策略决策、实验验证与产品落地。

本仓库主要讨论**策略如何被设计、执行、评估和迭代**，不以广告投放知识或平台特定后台操作为核心。

> 适用方向：广告策略产品、推荐/内容策略产品、内容治理策略、反欺诈与交易风控策略产品，以及策略中台与决策系统产品。

## 从哪里开始

| 学习模块 | 核心问题 | 资料 |
| --- | --- | --- |
| **01 · Strategy Product Fundamentals** | 策略与普通功能产品有什么不同？如何定义目标、约束与决策？ | [策略产品基础](01-strategy-fundamentals/README.md) · [策略设计方法](01-strategy-fundamentals/strategy-design-framework.md) |
| **02 · Advertising & Traffic Strategy** | 广告、自然内容和商业目标如何争夺并分享流量？ | [广告与流量策略](02-advertising-and-traffic/README.md) |
| **03 · Content Strategy & Governance** | 内容供给、分发、质量与生态治理如何关联？ | [内容策略与治理](03-content-strategy/README.md) |
| **04 · Risk Control & Anti-Fraud** | 如何建立欺诈识别、风险分层与处置策略？ | [风控与反作弊](04-risk-control/README.md) · [风控指标完整演算](04-risk-control/risk-metrics-and-thresholds.md) |
| **05 · Risk Decision Systems** | 模型、规则、实时特征与人工审核如何协同？ | [策略决策系统](05-decision-systems/README.md) |
| **06 · Experimentation & Optimization** | 如何证明策略有效，同时避免误杀与生态损伤？ | [实验与策略优化](06-experimentation/README.md) |
| **07 · Strategy Product Cases** | 广告收入下降、内容质量波动、异常交易如何诊断？ | [综合案例与面试训练](07-cases-and-interviews/README.md) |

## 一条统一的策略工作流

~~~mermaid
flowchart LR
  A["业务目标与风险定义"] --> B["数据与状态感知"]
  B --> C["模型评分 / 规则判断"]
  C --> D{"策略决策"}
  D --> E["分发 / 放行 / 限流 / 审核 / 拦截"]
  E --> F["业务结果与护栏指标"]
  F --> G["实验评估与复盘"]
  G --> B
~~~

这是通用的**设计框架**，不是任何公司内部系统结构。真实项目中，规则、模型与人工流程可能有不同顺序，并受到数据隐私、法律、延迟预算和工程稳定性约束。

## 三条业务主线

**广告与流量策略**：在内容消费和用户体验约束下，研究流量供给、分发机会、广告请求、商业收益、广告相关性和长期用户价值。

**内容策略与治理**：研究内容供给、分发效率、创作者激励、多样性、低质内容识别、负反馈和生态健康，避免将“流量最大化”误认为“内容生态最优”。

**风控与反作弊**：研究风险事件、损失函数、规则与模型、误杀成本、灰度处置、人机协同，以及攻防双方行为变化造成的策略失效。

## 与另一个广告仓库的区别

[Advertising-Monetization-Learning](https://github.com/ZeyuYu713/Advertising-Monetization-Learning) 主要讲广告生态、品牌/效果广告、KPI、预算、购买机制、广告样式与商业化经济学；**本仓库则专注于平台上的决策机制和策略产品实践**。

例如，学习 CPM、Reach & Frequency 的定义去广告仓库；研究广告负载控制如何影响内容体验、用户留存与平台收益，在本仓库讨论。两边只保留必要的交叉引用，避免复制内容。

## 内容标准

每节优先包含：**业务背景、指标及口径、形式化模型或判定逻辑、可复算示例、产品方案、验证方法与常见错误**。

所有案例数据为虚构教学数据，不代表 ByteDance、TikTok 或其他公司的内部指标、系统实现或阈值。公式只在所陈述假设下成立；没有实验或可核查证据时，不将相关性解释成因果关系。

不收录真实的非公开风控绕过手法、内部阈值、敏感账户数据或可用于规避检测的操作细节。内容侧重防御、治理与可审计决策。

## 学习入口

推荐先读 [01 基础框架](01-strategy-fundamentals/README.md)，再根据岗位选择 [02 广告](02-advertising-and-traffic/README.md)、[03 内容](03-content-strategy/README.md) 或 [04 风控](04-risk-control/README.md)，最后通过 [06 实验](06-experimentation/README.md) 和 [07 综合案例](07-cases-and-interviews/README.md) 练习。

*Independent learning notes; not an official document of any platform.*
