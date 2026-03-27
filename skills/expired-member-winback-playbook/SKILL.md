---
name: expired-member-winback-playbook
description: 设计过期会员的短过期与长过期召回方案，覆盖触达节奏、权益设计、价格动作和放弃阈值。适用于会员和订阅业务。
intent: >-
  当会员已过期，需要判断哪些用户值得继续召回、用什么时机和动作召回、何时停止投入时，使用这个 skill。重点是区分短过期高意向用户和长过期低意向用户，避免统一策略浪费成本。
type: workflow
best_for:
  - 过期会员召回
  - 召回节奏设计
  - 过期分层经营
scenarios:
  - 到期后 D7 内召回弱
  - 长过期用户触达成本高但回收差
---

# Expired Member Winback Playbook

## Purpose

这个 skill 用于过期会员召回，不处理在期挽回，也不处理支付失败恢复。

重点是把：

- 短过期
- 中过期
- 长过期

三类人群分开经营。

## Key Concepts

### 1. 短过期和长过期不是同一问题

- 短过期更接近“意愿未完全消失”
- 长过期更接近“需求衰退或替代完成”

### 2. 召回动作优先顺序

先做：

- 价值提醒
- 场景唤醒
- 核心权益回顾

再做：

- 轻度价格动作
- 定向权益包

### 3. 召回一定要有放弃阈值

如果用户长期不响应、历史价值低、触达成本高，就不应该无限打扰。

## Application

### Phase 1: 做过期分窗

推荐至少拆：

- D1-D7
- D8-D30
- D31+

### Phase 2: 定义优先召回人群

优先级通常更高的人群：

- 过期前仍有使用
- 历史价值高
- 关键权益使用深
- 短期内有明显需求场景

### Phase 3: 设计召回动作

常见动作：

- 到期后价值提醒
- 关键权益回顾
- 限时回归包
- 场景化内容召回

### Phase 4: 定义放弃规则

至少明确：

- 最多触达几次
- 超过什么窗口不再主推
- 哪类用户不再投入优惠

## Output Format

1. 过期分窗结论
2. 优先召回人群
3. 动作节奏表
4. 放弃阈值
5. 实验与护栏

## Examples

### 示例：D1-D7 与 D30+ 不同打法

- D1-D7：更适合强调未完成价值和轻度激励
- D30+：更适合低频测试，不适合持续重补贴

## Common Pitfalls

- 所有过期用户一个节奏
- 只有优惠，没有价值回顾
- 没有放弃阈值
- 不看召回后次周期续费

## References

- `skills/subscription-renewal-diagnostic/SKILL.md`
- `skills/retention-revenue-playbook/SKILL.md`
- `skills/pricing-change-evaluator/SKILL.md`
