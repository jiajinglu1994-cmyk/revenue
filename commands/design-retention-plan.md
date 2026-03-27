---
name: design-retention-plan
description: 为商业产品设计续费、复购、召回和挽回方案，串联诊断、定价和优先级能力。
argument-hint: "<业务模式、留存问题、目标指标>"
uses:
  - revenue-health-diagnostic
  - retention-revenue-playbook
  - pricing-change-evaluator
  - commercial-prioritization-advisor
outputs:
  - 留存策略方案
  - 实验设计摘要
  - 30 天动作建议
---

# Design Retention Plan

按下面顺序执行：

1. 先用 `skills/revenue-health-diagnostic/SKILL.md` 确认问题主要发生在续费、复购、召回、支付失败还是取消挽回。
2. 使用 `skills/retention-revenue-playbook/SKILL.md` 设计分阶段动作、人群分层、触发时机和验证方式。
3. 如果方案涉及价格、权益包或折扣，补跑 `skills/pricing-change-evaluator/SKILL.md` 检查收入与利润风险。
4. 最后用 `skills/commercial-prioritization-advisor/SKILL.md` 给出先做什么、后做什么和哪些动作只适合灰度。

最终输出：

- 留存问题分层结论
- 建议上线的 1 到 3 个动作
- 对照组与实验组设计
- 需要补齐的数据和能力
