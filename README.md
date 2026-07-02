# AI PM PRD Coach

`ai-pm-prd-coach` is a reusable skill for AI product manager students and junior PMs.

It turns a rough AI product idea or short requirement into a clearer Chinese PRD by:

- asking focused clarification questions first
- narrowing the MVP scope
- generating user stories
- drafting testable acceptance criteria
- surfacing AI-specific risks and assumptions

This project is designed for:

- class assignments
- PM portfolio projects
- first-draft requirement discussions

## Why this skill

Many beginner PMs can describe an idea, but struggle to turn it into a requirement document that is structured, scoped, and actionable.

This skill is built to close that gap. It behaves more like a PRD coach than a simple template filler.

## What it does

Input:

- a one-sentence AI product idea
- a short feature request
- a rough problem statement

Output:

- structured PRD draft in Chinese
- MVP scope
- user stories
- acceptance criteria
- risks and assumptions
- success metrics

## Key design choices

- `Clarify first`: asks 3 to 5 high-value questions before drafting when key information is missing
- `MVP focused`: prefers a narrower and more realistic first version
- `AI-aware`: includes hallucination risk, fallback logic, and output quality concerns when relevant
- `Student friendly`: keeps the output practical instead of overly formal

## Repository structure

```text
ai-pm-prd-coach/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
├── references/
│   └── prd-template.md
└── examples/
    ├── example-prompts.md
    ├── example-output.md
    └── full-demo-prd.md
```

## Example use cases

- turn an AI feature idea into a PRD for a class assignment
- structure an early product concept for a portfolio case study
- convert a vague requirement into user stories and acceptance criteria
- train beginner PMs to think about AI risks, fallback, and quality evaluation

## Example prompt

```text
Use $ai-pm-prd-coach to turn this rough idea into a Chinese PRD:
I want to build an AI interview practice assistant for college students.
Please ask me key clarification questions first, then generate the PRD,
MVP scope, user stories, and acceptance criteria.
```

## Output structure

The skill defaults to this structure:

1. 产品目标
2. 背景与问题定义
3. 目标用户
4. 核心使用场景
5. MVP 范围
6. 非目标 / 暂不纳入
7. 功能需求
8. 用户故事
9. 验收标准
10. 风险与假设
11. 成功指标

## Files to check

- Core skill instructions: [SKILL.md](./SKILL.md)
- PRD template reference: [references/prd-template.md](./references/prd-template.md)
- Prompt examples: [examples/example-prompts.md](./examples/example-prompts.md)
- Output expectation: [examples/example-output.md](./examples/example-output.md)
- Full demo: [examples/full-demo-prd.md](./examples/full-demo-prd.md)

## Suggested next steps

- add more domain-specific PRD examples
- create separate references for education, productivity, and e-commerce use cases
- add an English output mode if needed

## License

You can add the license that matches your course or public GitHub publishing preference.
