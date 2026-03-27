# 会员 / 订阅专项库说明

这个仓库原本是“商业产品技能库”。这一层专项补充的目标，是把其中与会员、订阅、续费、解约干预、过期召回和支付失败恢复强相关的能力单独做厚。

## 为什么要单独做专项层

会员订阅业务有几个和通用商业化不同的特点：

1. 长期收入主要来自续费，不是只看首购
2. 生命周期动作高度依赖时机和频控
3. 同一个动作对不同国家、SKU、生命周期状态的效果差异很大
4. 很多“续费提升”其实是试用转付费、支付失败恢复、解约挽回和过期召回的混合结果

如果没有专项层，容易把这些问题混在一起分析，最后策略不稳定。

## 专项层覆盖的关键环节

1. 在期续费诊断
2. 解约干预与 save offer
3. 过期召回
4. 支付失败恢复
5. 生命周期节奏与实验设计

## 推荐使用路径

### 场景 1：续费率下滑，但不知道掉在哪

先用：

- `skills/subscription-renewal-diagnostic/SKILL.md`

再按问题进入：

- 已解约用户多：`skills/cancellation-save-strategy/SKILL.md`
- 过期召回弱：`skills/expired-member-winback-playbook/SKILL.md`
- 非自愿流失高：`skills/payment-failure-recovery-playbook/SKILL.md`

### 场景 2：要做会员生命周期专项

直接跑：

- `commands/plan-membership-lifecycle.md`

### 场景 3：要做续费专项复盘

直接跑：

- `commands/run-renewal-audit.md`

## 和通用商业产品技能的关系

- 通用技能负责经营全局和跨模型复用
- 专项技能负责会员 / 订阅问题的深挖
- 两者并存，不互相替代
