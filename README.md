# revenue

商业产品技能库。

目标不是复刻通用 PM 方法论，而是把上游 `Product Manager Skills` 中与营收、增长、定价、渠道、留存和商业化决策强相关的能力，重组为一套更适合商业产品团队日常使用的技能体系。

这套库默认面向以下业务模型：

- 订阅与会员
- 电商与增值包
- 内容付费与工具付费
- 平台抽佣与撮合
- 广告与流量变现
- 需要兼顾收入、毛利、回本和经营动作的商业化产品

## 目录结构

- `skills/`：核心技能定义
- `commands/`：多技能串联工作流
- `docs/`：设计原则与上游映射
- `Product-Manager-Skills/`：上游参考仓库的本地克隆，仅用于学习和对照，不纳入版本管理

## 设计原则

这里的泛化主要做了四件事：

1. 从 SaaS PM 视角扩展到多种商业模型
   不只讨论 MRR、NRR，也覆盖 GMV、抽佣、复购、退款、广告 ARPU、订单毛利和回本。
2. 从“写文档框架”转成“经营决策框架”
   输出不止停在分析结论，更强调分层、测算、灰度、实验和动作优先级。
3. 从单点工具升级为可组合工作流
   让机会识别、经营诊断、定价评估、功能投入、渠道判断和路线图规划能串起来用。
4. 从产品语言泛化成商业产品语言
   减少纯 PM 术语，增加经营目标、收入影响、风险暴露和组织落地语境。

更细的映射见 [docs/upstream-derivation-map.md](/Users/gdnpc-658/Documents/pmcodex/revenue/docs/upstream-derivation-map.md)。

## 技能矩阵

1. `commercial-opportunity-canvas`
   用统一框架判断一个商业机会值不值得做，适合新方向、专项机会和年度规划输入。
2. `revenue-health-diagnostic`
   诊断收入、转化、留存、渠道效率和单位经济问题，适合季度复盘和异常排查。
3. `pricing-change-evaluator`
   评估涨价、降价、折扣、套餐重构、抽佣变化、包月包年和附加包设计。
4. `feature-investment-evaluator`
   评估商业化功能是否值得投入，重点看收入路径、成本、风险和验证方式。
5. `acquisition-channel-evaluator`
   判断渠道该加预算、限额试验、保持优化还是停掉。
6. `retention-revenue-playbook`
   设计续费、复购、召回、挽回和 dunning 动作，解决“有首购没长期价值”的问题。
7. `commercial-prioritization-advisor`
   为商业化需求选择合适的排序逻辑，避免只看想象中的收入空间。
8. `commercial-growth-strategy-workflow`
   从诊断到假设、评估、排序和路线图的完整商业增长工作流。

## Commands

- `run-commercial-review`
- `plan-commercial-roadmap`
- `design-retention-plan`

## 推荐使用方式

直接引用具体 skill 文件：

```text
使用 /Users/gdnpc-658/Documents/pmcodex/revenue/skills/revenue-health-diagnostic/SKILL.md
帮我诊断这个商业化产品最近一个季度的收入、转化、留存和单位经济问题。
先问最多 3 个澄清问题，再给出问题优先级、关键假设和 30 天动作。
```

```text
运行 /Users/gdnpc-658/Documents/pmcodex/revenue/commands/plan-commercial-roadmap.md
目标是提升订阅业务未来两个季度的续费率和 ARPU。
```

如果是一个新方向而不是已有业务复盘，先从 `commercial-opportunity-canvas` 开始，再进入评估和路线图。

## 来源说明

- 上游仓库：`https://github.com/deanpeters/Product-Manager-Skills`
- 本地参考目录：`/Users/gdnpc-658/Documents/pmcodex/revenue/Product-Manager-Skills`

当前仓库不复制上游源码，只沉淀泛化后的自有 skills 和 workflows。
