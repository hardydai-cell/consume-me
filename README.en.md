English | [简体中文](./README.md)

# consume-me

**Turn vague plans into explicit decisions.**

`consume-me` is a pressure-testing skill for serious AI agents. It does not flatter the plan, summarize it politely, or let weak assumptions slide. It interrogates a plan or design from three angles until the real trade-offs, dependencies, and structural risks are explicit.

## What It Does

- **Drill-down**: walk every branch of the decision tree to the leaves.
- **Lateral Scan**: challenge whether same-level alternatives were skipped.
- **Zoom-out**: step back and expose system-wide contradictions and hidden assumptions.

## Why It Feels Different

- It pushes until fuzzy language becomes decision-ready language.
- It is designed for planning, architecture, spec review, and product/design critique.
- It prefers asking the right next question instead of pretending consensus already exists.

## Install

This repository is a dedicated single-skill repo, but it uses the standard `skills/consume-me/` layout so it works cleanly with the open `skills` CLI ecosystem.

### Standard install

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me
```

### Path-style install

If you prefer the `owner/repo/path` style used by skill catalogs, this repository also supports direct installation from the skill directory:

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

### Global install

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -g -y
```

### Preview before install

```bash
npx skills@latest add hardydai-cell/consume-me --list
```

## Works With Many Agents

This skill is distributed through the `skills` CLI workflow, which supports Codex, Claude Code, OpenCode, Cursor, and many other agent environments.

## Example Prompts

- `Use $consume-me to stress-test this product spec.`
- `Use $consume-me to interrogate this architecture plan until every major trade-off is explicit.`
- `Use $consume-me to review this roadmap and surface hidden dependencies.`

## Repository Layout

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

## Why Star This

If most planning skills stop at "good enough", `consume-me` is the one that keeps pressing. It is built for teams and builders who would rather surface hard problems early than pay for them later.
