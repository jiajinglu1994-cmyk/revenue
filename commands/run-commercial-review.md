---
name: run-commercial-review
description: 对一个商业产品做完整经营复盘，串联诊断、渠道、定价和优先级能力。
argument-hint: "<业务背景、最近指标、当前问题>"
uses:
  - revenue-health-diagnostic
  - acquisition-channel-evaluator
  - pricing-change-evaluator
  - retention-revenue-playbook
  - commercial-prioritization-advisor
outputs:
  - 经营诊断摘要
  - 关键问题优先级
  - 30天动作建议
---

# Run Commercial Review

按下面顺序执行：

1. 先用 `skills/revenue-health-diagnostic/SKILL.md` 找出最关键的收入、转化、留存或单位经济问题。
2. 如果问题集中在拉新质量，调用 `skills/acquisition-channel-evaluator/SKILL.md` 深挖主要渠道。
3. 如果问题集中在客单价、ARPU、付费率或套餐结构，调用 `skills/pricing-change-evaluator/SKILL.md`。
4. 如果问题集中在续费、复购、召回、取消挽回或支付失败，调用 `skills/retention-revenue-playbook/SKILL.md`。
5. 最后用 `skills/commercial-prioritization-advisor/SKILL.md` 给出动作排序。

最终输出：

- 一句话经营判断
- 最值得先做的 3 件事
- 每件事的预期影响、风险和前置条件
