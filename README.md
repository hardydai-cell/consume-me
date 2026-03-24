# consume-me

**Turn vague plans into explicit decisions.**  
**把模糊计划压成可执行决策。**

`consume-me` is a pressure-testing skill for serious AI agents. It does not flatter the plan, summarize it politely, or let weak assumptions slide. It interrogates a plan or design from three angles until the real trade-offs, dependencies, and structural risks are explicit.

`consume-me` 是一个给严肃 AI Agent 使用的高压审问型 skill。它不会礼貌复述你的方案，也不会放过含糊假设。它会从三个视角持续追问，直到真正的权衡、依赖关系和结构性风险被彻底摊开。

## What It Does / 它做什么

- **Drill-down**: walk every branch of the decision tree to the leaves.
- **Lateral Scan**: challenge whether same-level alternatives were skipped.
- **Zoom-out**: step back and expose system-wide contradictions and hidden assumptions.

- **纵向深挖**：把每个决策分支追到叶子节点。
- **横向补漏**：追问同层备选方案是否被忽略。
- **全局复盘**：识别系统级矛盾、盲点和隐含前提。

## Why It Feels Different / 为什么它不一样

- It pushes until fuzzy language becomes decision-ready language.
- It is designed for planning, architecture, spec review, and product/design critique.
- It prefers asking the right next question instead of pretending consensus already exists.

- 它会把模糊表达压成可以执行的决策语言。
- 它适用于规划、架构评审、规格澄清、产品与设计质询。
- 它优先追问下一个真正关键的问题，而不是假装已经形成共识。

## Install / 安装

This repository is a dedicated single-skill repo, but it uses the standard `skills/consume-me/` layout so it works cleanly with the open `skills` CLI ecosystem.

这是一个单-skill 专仓，但采用了标准的 `skills/consume-me/` 目录结构，因此可以直接接入开放的 `skills` CLI 生态。

### Generic / 通用

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me
```

### Codex

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a codex
```

### Claude Code

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a claude-code
```

### Global install / 全局安装

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -g -y
```

## Works With Many Agents / 支持多类 Agent

This skill is distributed through the `skills` CLI workflow, which supports Codex, Claude Code, OpenCode, Cursor, and many other agent environments.

这个 skill 通过 `skills` CLI 工作流分发，可面向 Codex、Claude Code、OpenCode、Cursor 以及更多 agent 环境安装。

## Example Prompts / 示例触发语

- `Use $consume-me to stress-test this product spec.`
- `Use $consume-me to interrogate this architecture plan until every major trade-off is explicit.`
- `Use $consume-me to review this roadmap and surface hidden dependencies.`

- `用 $consume-me 审问这份产品规格，直到每个关键决策都明确。`
- `用 $consume-me 压测这份架构方案，把主要权衡全部摊开。`
- `用 $consume-me 复盘这份路线图，找出隐藏依赖和结构风险。`

## Repository Layout / 仓库结构

```text
consume-me/
├─ README.md
└─ skills/
   └─ consume-me/
      ├─ SKILL.md
      └─ agents/
         └─ openai.yaml
```

## Why Star This / 为什么值得 Star

If most planning skills stop at “good enough”, `consume-me` is the one that keeps pressing. It is built for teams and builders who would rather surface hard problems early than pay for them later.

如果大多数规划类 skill 都停在“差不多可以”，那 `consume-me` 就是那个会继续逼问下去的 skill。它适合那些宁愿在前期暴露难题、也不愿在后期付出代价的团队和开发者。
