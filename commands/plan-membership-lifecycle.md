---
name: plan-membership-lifecycle
description: 为会员订阅业务规划生命周期经营方案，串联续费诊断、解约挽回、过期召回和长期路线图。
argument-hint: "<业务背景、生命周期问题、目标周期>"
uses:
  - subscription-renewal-diagnostic
  - cancellation-save-strategy
  - expired-member-winback-playbook
  - payment-failure-recovery-playbook
  - retention-revenue-playbook
  - commercial-prioritization-advisor
outputs:
  - 生命周期经营路线图
  - 短期与长期动作清单
  - 数据与实验需求
---

# Plan Membership Lifecycle

按下面顺序执行：

1. 使用 `skills/subscription-renewal-diagnostic/SKILL.md` 做现状分层诊断。
2. 针对在期已解约问题，使用 `skills/cancellation-save-strategy/SKILL.md`。
3. 针对过期回流问题，使用 `skills/expired-member-winback-playbook/SKILL.md`。
4. 针对非自愿流失问题，使用 `skills/payment-failure-recovery-playbook/SKILL.md`。
5. 用 `skills/retention-revenue-playbook/SKILL.md` 把动作收敛为完整生命周期经营方案。
6. 最后用 `skills/commercial-prioritization-advisor/SKILL.md` 排出短期和中期优先级。

最终输出：

- 生命周期分层结论
- 30 天止血动作
- 90 天系统化动作
- 待补的数据、埋点和实验能力
