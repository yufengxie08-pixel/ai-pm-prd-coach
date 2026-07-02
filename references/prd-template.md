# AI PM PRD Template

Use this template when the user wants a first-draft PRD in Chinese.

## Writing principles

- Keep the document concise and practical.
- Prefer narrow MVP scope over broad wish lists.
- Label inferred content as `假设`.
- For AI features, include quality risk and fallback logic when relevant.

## Template

```md
# {产品名称或功能名称}

## 1. 产品目标
- 要解决什么问题：
- 希望带来什么结果：
- 为什么现在做：

## 2. 背景与问题定义
- 当前现状：
- 主要痛点：
- 问题影响：

## 3. 目标用户
- 核心用户：
- 次级用户：
- 用户特征：

## 4. 核心使用场景
- 场景 1：
- 场景 2：
- 场景 3：

## 5. MVP 范围
- 必须有：
- 可以延后：
- MVP 成功的最低标准：

## 6. 非目标 / 暂不纳入
- 本期不解决的问题：
- 暂不支持的人群或场景：

## 7. 功能需求
### 7.1 功能一
- 功能描述：
- 输入：
- 输出：
- 规则：

### 7.2 功能二
- 功能描述：
- 输入：
- 输出：
- 规则：

## 8. 用户故事
- 作为 {用户}，我希望 {动作}，以便 {结果}。
- 作为 {用户}，我希望 {动作}，以便 {结果}。

## 9. 验收标准
- Given ...
  When ...
  Then ...
- Given ...
  When ...
  Then ...

## 10. 风险与假设
- 假设：
- AI 输出风险：
- 数据或输入质量风险：
- 失败时 fallback：

## 11. 成功指标
- 使用率：
- 完成率：
- 满意度：
- AI 结果质量指标：
```

## Acceptance criteria guidance

Acceptance criteria should be:

- observable
- testable
- specific enough for design and engineering handoff

Weak example:

- 用户觉得好用

Better example:

- 用户输入一段不超过 500 字的需求后，系统可在 10 秒内生成包含目标用户、MVP 范围和验收标准的结构化 PRD 初稿。

## AI-specific checks

Add these only when relevant:

- Is manual review required before output is shown to end users?
- What happens when the model confidence is low?
- Can the user edit, retry, or regenerate?
- How will output quality be evaluated?
