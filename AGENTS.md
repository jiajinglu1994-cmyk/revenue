# Repository Guidelines

## 目标

这个仓库沉淀的是“商业产品技能”，不是通用 PM 教材。

判断一个改动是否合格，优先看三件事：

1. 能不能帮助商业产品团队更快做经营决策
2. 能不能跨订阅、电商、平台、广告等模型复用
3. 能不能把分析结论落到动作、实验、路线图或数据需求

## 结构约定

- `skills/<skill-name>/SKILL.md`：单个技能
- `commands/*.md`：多技能串联工作流
- `docs/*.md`：设计原则、映射关系和辅助说明
- `Product-Manager-Skills/`：仅作上游参考，不纳入版本管理

## Skill 写作规范

每个 skill 尽量包含这些部分：

- Frontmatter：至少有 `name`、`description`
- `Purpose`
- `Key Concepts`
- `Application`
- `Examples`
- `Common Pitfalls`
- `References`

优先写“商业判断框架”和“动作输出方式”，不要堆太多泛 PM 背景知识。

## 内容风格

- 用中文写，文件名保持英文 kebab-case
- 先讲什么时候该用，再讲怎么用
- 例子尽量是商业产品语境，不要只用纯 SaaS B2B 例子
- 能分层就分层，不要只给总盘结论
- 能落到 go / no-go、灰度、止血、排期，就不要只停在抽象建议

## 编辑边界

- 不要提交 `Product-Manager-Skills/`
- 不要把上游整段照搬进来
- 如果复用了上游思路，在 `docs/upstream-derivation-map.md` 补映射说明

## 校验

提交前至少确认：

- `README.md` 中的技能清单与实际目录一致
- `commands/` 中引用的 skill 路径存在
- 新 skill 的输出格式足够稳定，能被后续 workflow 复用
