---
name: run-renewal-audit
description: 对会员订阅业务做续费专项复盘，串联续费诊断、解约挽回、过期召回和支付失败恢复。
argument-hint: "<地区、SKU、近期续费问题、当前策略>"
uses:
  - subscription-renewal-diagnostic
  - cancellation-save-strategy
  - expired-member-winback-playbook
  - payment-failure-recovery-playbook
  - commercial-prioritization-advisor
outputs:
  - 续费专项诊断
  - 高优先级修复动作
  - 实验建议
---

# Run Renewal Audit

按下面顺序执行：

1. 先用 `skills/subscription-renewal-diagnostic/SKILL.md` 明确问题发生在哪个环节。
2. 如果在期已解约占比高，调用 `skills/cancellation-save-strategy/SKILL.md`。
3. 如果过期后回流弱，调用 `skills/expired-member-winback-playbook/SKILL.md`。
4. 如果自动续费失败导致流失，调用 `skills/payment-failure-recovery-playbook/SKILL.md`。
5. 最后用 `skills/commercial-prioritization-advisor/SKILL.md` 给出先做什么、后做什么和哪些动作只适合灰度。

最终输出：

- 一句话续费结论
- 最值得先做的 3 个动作
- 每个动作的目标指标、护栏指标和验证窗口
