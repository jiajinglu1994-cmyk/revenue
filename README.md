# revenue

商业产品技能库。目标是把上游的 Product Manager Skills 中与营收、增长、定价、渠道、商业化决策相关的能力，泛化成更适合商业产品团队日常使用的一套 skills。

## 项目内容

- `skills/`：面向商业产品的核心技能
- `commands/`：多 skill 串联的工作流
- `Product-Manager-Skills/`：上游参考仓库的本地克隆，仅用于学习和对照，不纳入当前仓库版本管理

## 泛化原则

上游仓库很多能力是按 SaaS PM 视角写的。我在这个项目里做了三层泛化：

1. 从 SaaS 指标扩展到更广的商业化模型
   包括订阅、电商、内容付费、平台抽佣、广告、服务型营收。
2. 从“产品经理方法论”转成“商业产品决策框架”
   输出更强调收入影响、毛利、回本、实验设计和经营动作。
3. 从单点框架升级为可串联工作流
   让诊断、定价、功能投入、渠道评估和优先级排序能组合起来跑。

## 当前 skills

1. `revenue-health-diagnostic`
   全局诊断收入、转化、留存、渠道效率和单位经济。
2. `pricing-change-evaluator`
   评估涨价、降价、折扣、套餐重构、抽佣调整、包月包年等变化。
3. `feature-investment-evaluator`
   评估功能是否值得做，重点看营收贡献、留存提升、成本和实验路径。
4. `acquisition-channel-evaluator`
   评估渠道的获客成本、后链路质量、规模化能力和回本周期。
5. `commercial-prioritization-advisor`
   为商业化需求选择优先级逻辑，避免只看主观价值或只看短期收入。
6. `commercial-growth-strategy-workflow`
   从经营诊断到假设、实验、路线图的完整增长工作流。

## 当前 commands

- `run-commercial-review`
- `plan-commercial-roadmap`

## 在 Codex 中的用法

直接引用具体 skill 文件即可。

```text
使用 /Users/gdnpc-658/Documents/pmcodex/revenue/skills/revenue-health-diagnostic/SKILL.md，
帮我诊断这个商业化产品最近一个季度的收入、转化、留存和单位经济问题。
先问最多 3 个澄清问题，再给出问题优先级、关键假设和 30 天动作。
```

```text
运行 /Users/gdnpc-658/Documents/pmcodex/revenue/commands/plan-commercial-roadmap.md，
目标是提升订阅业务未来两个季度的续费率和 ARPU。
```

## 来源说明

本项目参考了本地克隆的上游仓库：

- 上游地址：`https://github.com/deanpeters/Product-Manager-Skills`
- 本地参考目录：`/Users/gdnpc-658/Documents/pmcodex/revenue/Product-Manager-Skills`

当前仓库不复制上游源码，只沉淀泛化后的自有 skills。
