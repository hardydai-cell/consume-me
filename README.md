[English](./README.en.md) | 简体中文

# consume-me

**把模糊计划压成可执行决策。**

`consume-me` 是一个给严肃 AI Agent 使用的高压审问型 skill。它不会礼貌复述你的方案，也不会放过含糊假设。它会从三个视角持续追问，直到真正的权衡、依赖关系和结构性风险被彻底摊开。

## 它做什么

- **纵向深挖**：把每个决策分支追到叶子节点。
- **横向补漏**：追问同层备选方案是否被忽略。
- **全局复盘**：识别系统级矛盾、盲点和隐含前提。

## 为什么它不一样

- 它会把模糊表达压成可以执行的决策语言。
- 它适用于规划、架构评审、规格澄清、产品与设计质询。
- 它优先追问下一个真正关键的问题，而不是假装已经形成共识。

## 安装

这个仓库是单-skill 专仓，但采用了标准的 `skills/consume-me/` 目录结构，因此可以直接接入开放的 `skills` CLI 生态。

### 标准安装

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me
```

### 目录直装

如果你更喜欢 skill catalog 常见的 `owner/repo/path` 风格，这个仓库也支持直接从 skill 目录安装：

```bash
npx skills@latest add https://github.com/hardydai-cell/consume-me/tree/main/skills/consume-me
```

### Codex

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a codex
```

### Claude Code

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a claude-code
```

### 全局安装

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -g -y
```

### 安装前预览

```bash
npx skills@latest add hardydai-cell/consume-me --list
```

## 支持多类 Agent

这个 skill 通过 `skills` CLI 工作流分发，可面向 Codex、Claude Code、OpenCode、Cursor 以及更多 agent 环境安装。

## 示例触发语

- `用 $consume-me 审问这份产品规格，直到每个关键决策都明确。`
- `用 $consume-me 压测这份架构方案，把主要权衡全部摊开。`
- `用 $consume-me 复盘这份路线图，找出隐藏依赖和结构风险。`

## 仓库结构

```text
consume-me/
├─ README.md
├─ README.en.md
└─ skills/
   └─ consume-me/
      ├─ SKILL.md
      └─ agents/
         └─ openai.yaml
```

## 为什么值得 Star

如果大多数规划类 skill 都停在“差不多可以”，那 `consume-me` 就是那个会继续逼问下去的 skill。它适合那些宁愿在前期暴露难题、也不愿在后期付出代价的团队和开发者。
