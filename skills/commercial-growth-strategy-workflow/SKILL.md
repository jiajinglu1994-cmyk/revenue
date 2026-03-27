---
name: commercial-growth-strategy-workflow
description: 运行商业产品增长策略工作流，从经营诊断到人群、定价、渠道、功能和实验路线图。适用于季度规划、专项增长项目和商业化策略重构。
intent: >-
  把商业产品的增长讨论从“很多想法”推进到“有诊断、有结构拆分、有假设、有评估、有排序和有路线图”。适用于季度经营规划、专项增长攻坚和商业化策略重构。
type: workflow
best_for:
  - 季度经营规划
  - 商业化专项攻坚
  - 增长策略重构
scenarios:
  - 续费率和 ARPU 同时承压，需要系统性增长方案
  - 新季度要在渠道、定价和功能之间排优先级
---

# Commercial Growth Strategy Workflow

## Purpose

把商业产品策略从“有很多想法”推进到“有诊断、有假设、有实验、有路线图”。这是一个串联多个技能的工作流，适合做季度经营规划和专项增长方案。

## Key Concepts

### 1. 先诊断，再出动作

如果跳过诊断直接做动作，最常见的结果是：

- 把结构性问题当成流量问题
- 把留存问题当成价格问题
- 同时改太多变量，无法归因

### 2. 增长动作必须落到具体对象

建议至少按以下一层做结构拆分：

- 人群
- 渠道
- 国家
- 套餐或 SKU
- 生命周期阶段

### 3. 工作流的价值在于串联

单个 skill 给的是局部判断；workflow 要做的是把局部判断收敛成一个可执行路线图。

## Workflow Overview

整个工作流建议按 6 个阶段推进。

### Phase 1: 经营诊断

先运行：

- `skills/revenue-health-diagnostic/SKILL.md`

产出：

- 当前最核心的 3 个问题
- 问题所在环节
- 哪些问题要先止血

### Phase 2: 人群与结构拆分

把问题拆到关键结构层：

- 人群层
- 国家或渠道层
- SKU / 套餐层
- 新老用户层

目标是避免在总盘子里做平均优化。

### Phase 3: 生成增长假设

假设至少落到以下方向之一：

- 机会选择或人群选择
- 定价优化
- 渠道优化
- 付费漏斗优化
- 续费/复购提升
- 召回与挽回
- 商业化功能建设

### Phase 4: 逐项评估关键方案

按方案类型调用：

- 定价类：`skills/pricing-change-evaluator/SKILL.md`
- 功能类：`skills/feature-investment-evaluator/SKILL.md`
- 渠道类：`skills/acquisition-channel-evaluator/SKILL.md`
- 留存类：`skills/retention-revenue-playbook/SKILL.md`

### Phase 5: 做优先级排序

运行：

- `skills/commercial-prioritization-advisor/SKILL.md`

把方案分成：

- 立即执行
- 小流量验证
- 本季度储备
- 暂不投入

### Phase 6: 输出商业化路线图

路线图至少包括：

- 30 天止血动作
- 90 天增长动作
- 需要的埋点/报表/实验能力
- 负责人和关键指标

## Output Format

1. 经营结论
2. 关键结构洞察
3. 增长假设清单
4. 方案评估摘要
5. 优先级路线图
6. 风险和依赖

## Examples

### 示例：季度商业增长项目

问题背景：

- 新客投放还能买量，但回本变慢
- 续费率下滑
- 高价套餐占比下降

合理工作流输出应该包含：

1. 先止血：修支付失败恢复、砍掉低质量渠道
2. 再增长：做高价值人群的套餐迁移和临期续费动作
3. 最后建设：补齐 cohort 看板和价格灰度能力

## Common Pitfalls

- 跳过诊断，直接拍脑袋上增长动作
- 不做人群分层，导致策略平均化
- 一次同时改价格、渠道、权益，无法归因
- 没有埋点和实验设计就上全量

## References

- `skills/revenue-health-diagnostic/SKILL.md`
- `skills/pricing-change-evaluator/SKILL.md`
- `skills/feature-investment-evaluator/SKILL.md`
- `skills/acquisition-channel-evaluator/SKILL.md`
- `skills/retention-revenue-playbook/SKILL.md`
