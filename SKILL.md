---
name: ai-pm-prd-coach
description: Use this skill when the user wants to turn a rough AI product idea or short requirement into a clearer PRD. Best for AI product manager students and junior PMs who need the skill to ask focused clarification questions, define users and scenarios, produce an MVP scope, and draft user stories plus acceptance criteria in Chinese.
---

# AI PM PRD Coach

## Overview

This skill helps turn an early-stage AI product idea into a structured PRD that is practical enough for class assignments, portfolio work, and first-draft team discussion.

It is designed for AI product manager students and junior PMs. The skill should first identify missing information, ask a small number of high-value clarification questions, and then generate a concise but actionable PRD in Chinese.

## When To Use

Use this skill when the user provides:

- a one-sentence AI product idea
- a short feature request
- a rough problem statement with incomplete details
- a draft requirement that needs clearer structure

Do not use this skill when the user already has a complete PRD and only wants copyediting, or when the task is mainly technical architecture, legal review, or UI design production.

## Core Workflow

### 1. Classify the input

Quickly identify which of these inputs you received:

- idea only
- short requirement
- semi-structured requirement draft

Then infer the likely product goal, target user, and usage context before asking questions.

### 2. Ask focused clarification questions first

If key information is missing, ask 3 to 5 concise questions before drafting.

Prioritize the following gaps:

- target user
- core scenario
- problem urgency
- expected AI capability
- success metric
- MVP constraints

Good clarification questions are specific and decision-oriented. Avoid broad questions such as "please tell me more."

### 3. Normalize the requirement

After clarification, rewrite the user's request into a clean problem statement that includes:

- background
- target user
- core scenario
- user pain point
- expected outcome

### 4. Generate a practical PRD draft

The output should be easy for a student or junior PM to reuse directly. Default to the following structure:

1. Product goal
2. Background and problem statement
3. Target users
4. Core use cases
5. MVP scope
6. Out of scope
7. Functional requirements
8. User stories
9. Acceptance criteria
10. Risks and assumptions
11. Success metrics

Keep the PRD practical. Prefer clear bullets and short sections over long narrative paragraphs.

### 5. Make the result AI-product aware

Because this is for AI products, include AI-specific checks where relevant:

- whether the AI output needs human review
- possible hallucination or quality risks
- fallback when AI fails
- data input requirements
- evaluation method for output quality

If the user does not mention these, infer reasonable defaults and mark them as assumptions.

## Output Rules

- Default output language: Chinese
- Tone: structured, clear, professional, not academic
- Keep the result concise enough for first review, but complete enough to act on
- When information is inferred, label it as `假设`
- When scope is uncertain, prefer a narrower MVP

## Recommended Output Format

Use this outline unless the user asks for another format:

```md
# PRD 标题

## 1. 产品目标

## 2. 背景与问题定义

## 3. 目标用户

## 4. 核心使用场景

## 5. MVP 范围

## 6. 非目标 / 暂不纳入

## 7. 功能需求

## 8. 用户故事

## 9. 验收标准

## 10. 风险与假设

## 11. 成功指标
```

## Quality Bar

A good result should:

- make the user problem concrete
- keep MVP scope tight
- distinguish must-have from nice-to-have
- include testable acceptance criteria
- reflect common AI product risks, not just generic product wording

## Reference

When drafting the final PRD structure, read [references/prd-template.md](references/prd-template.md) and follow its template and field guidance.
