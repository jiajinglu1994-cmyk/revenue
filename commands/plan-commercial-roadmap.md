---
name: plan-commercial-roadmap
description: 为商业产品制定季度路线图，串联经营诊断、方案评估和优先级排序。
argument-hint: "<业务目标、时间范围、现状问题>"
uses:
  - commercial-growth-strategy-workflow
  - feature-investment-evaluator
  - pricing-change-evaluator
  - commercial-prioritization-advisor
outputs:
  - 季度增长路线图
  - 实验与能力建设列表
---

# Plan Commercial Roadmap

按下面顺序执行：

1. 运行 `skills/commercial-growth-strategy-workflow/SKILL.md` 搭建完整分析框架。
2. 对进入候选集的价格方案使用 `skills/pricing-change-evaluator/SKILL.md`。
3. 对进入候选集的功能方案使用 `skills/feature-investment-evaluator/SKILL.md`。
4. 使用 `skills/commercial-prioritization-advisor/SKILL.md` 把动作排成 P0 / P1 / P2。

最终输出：

- 30 天动作
- 90 天路线图
- 关键实验
- 需要补齐的数据和基础能力
