---
name: cancellation-save-strategy
description: 设计会员取消订阅拦截与挽回策略，覆盖退出问卷、降档、暂停、优惠和 save offer。适用于自动续费和会员订阅业务。
intent: >-
  当订阅用户在到期前主动取消自动续费时，使用这个 skill 设计解约干预方案。重点是分清谁值得挽回、用什么动作挽回、什么人群不该强拦，以及如何设置护栏指标和实验节奏。
type: workflow
best_for:
  - 取消率上升
  - 设计 save offer
  - 取消流程改版
scenarios:
  - 用户大量提前关闭自动续费
  - 需要设计降档、暂停订阅和优惠挽回方案
---

# Cancellation Save Strategy

## Purpose

这个 skill 专门处理“用户还没到期，但已经决定不再续费”的场景。

它要解决的不是粗暴拦截，而是：

- 找出可挽回人群
- 设计合理的 save offer
- 避免因为过度打扰或过度优惠伤害长期价值

## Key Concepts

### 1. 不是所有取消都该挽回

优先考虑：

- 最近仍有使用
- 历史价值高
- 取消原因可逆

谨慎挽回：

- 几乎无使用
- 明显价格敏感且高退款风险
- 因合规、信任或严重体验问题取消

### 2. save offer 不只等于打折

常见动作：

- 暂停订阅
- 降档或换周期
- 补充权益说明
- 短期优惠
- 退出问卷后定向动作

### 3. 取消页是策略页，不只是表单页

至少要回答：

- 用户为什么取消
- 是否还存在剩余价值
- 该给什么动作
- 什么情况下直接放行

## Application

### Phase 1: 做取消原因分层

常见原因：

- 价格高
- 当前没需求
- 已找到替代品
- 使用体验差
- 支付原因

### Phase 2: 定义可挽回人群

建议看：

- 最近 30 天使用频次
- 当前套餐与价值层级
- 历史续费表现
- 取消原因

### Phase 3: 设计 save offer 梯度

可选动作：

1. 价值提醒
2. 降档或换周期
3. 暂停订阅
4. 小额优惠
5. 直接放行

### Phase 4: 设置护栏和实验

至少跟踪：

- 挽回率
- 次周期续费
- 退款率
- 投诉率
- 优惠渗透率

## Output Format

1. 取消原因分层
2. 可挽回人群定义
3. save offer 设计表
4. 实验方案
5. 风险与放量边界

## Examples

### 示例：价格敏感型取消用户

推荐动作不是“一刀切 5 折”，而是：

- 对高价值用户给换周期或短暂停订
- 对低价值用户更多直接放行
- 对价格敏感但高使用用户，再试小额优惠

## Common Pitfalls

- 所有人都给同一优惠
- 不看取消原因直接强拦
- 只看当下挽回率，不看次周期表现
- 没有直接放行路径

## References

- `skills/subscription-renewal-diagnostic/SKILL.md`
- `skills/retention-revenue-playbook/SKILL.md`
- `skills/commercial-prioritization-advisor/SKILL.md`
