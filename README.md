[English](./README.en.md) | 简体中文

# consume-me

**让你的 Claude Code / Codex 把你的脑子吃到见底。**

`consume-me` 不是来温柔帮你整理思路的。它是来把你的 agent 变成一台认知压榨机，堵死你所有偷懒的出口，榨干每个模糊假设，把你脑子里最后一点像样的判断、洞察和灵感都逼出来。

这不是那种“帮你想一想”的 skill。  
这是那种会把你按在桌上，逼你把真正答案吐出来的 skill。

## 它会怎么消费你

- **纵向深挖**：顺着每个决策分支一路掘到底，直到它真的吐出明确判断。
- **横向扫荡**：把你懒得看、故意跳过、或者不敢碰的备选方案全揪出来。
- **全局复盘**：把整套系统拖到强光下，逼出结构性矛盾、隐藏依赖和自欺欺人的前提。

## 为什么它够疯

- 它不帮你显得聪明，它逼你真的想清楚。
- 它不接受“差不多”，只接受被压到见底之后剩下的硬决策。
- 它会让 Claude Code / Codex 像一头不肯松口的认知猎犬，一口一口咬掉你所有软塌塌的想法。
- 它适合规格、架构、路线图、产品赌注、prompt 设计，以及任何还有软肋的方案。

## 安装

如果你准备好了把脑子喂进去，就这样装。

这个仓库是单-skill 专仓，但采用了标准的 `skills/consume-me/` 目录结构，因此可以直接接入开放的 `skills` CLI 生态。

这也是一个纯文本 skill：没有脚本、没有二进制、没有额外可执行文件，从分发内容看非常安全。

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

### openclaw（龙虾）

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a openclaw
```

### 全局安装

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -g -y
```

### 安装前预览

```bash
npx skills@latest add hardydai-cell/consume-me --list
```

## 它能挂到哪些 Agent 身上

这个 skill 通过 `skills` CLI 工作流分发，可面向 Codex、Claude Code、openclaw（龙虾）、OpenCode、Cursor 以及更多 agent 环境安装。

## 示例触发语

- `用 $consume-me 把这份产品规格吃到只剩硬决策。`
- `用 $consume-me 把这份架构方案里所有偷懒假设都榨出来。`
- `用 $consume-me 继续往下掘，直到脑子里最后一颗有用的火星冒出来。`

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

如果你想要的是一个会顺着你、安慰你、帮你把模糊废话包装得更像答案的 skill，那这个仓库不适合你。  
如果你想让你的 agent 把你的脑子消费到见底，直到最后一点真东西被压出来，那就把它装上。
