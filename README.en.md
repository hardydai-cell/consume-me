English | [简体中文](./README.md)

# consume-me

**Let your Claude Code / Codex eat your brain down to the last spark.**

`consume-me` is not here to gently organize your thoughts. It turns your agent into a cognitive pressure machine that blocks every lazy escape, crushes every soft assumption, and squeezes the last useful idea out of your head.

This is not a “help me think a little” skill.  
This is the skill that corners you until the real answer finally comes out.

## How It Consumes You

- **Drill-down**: chase every branch until it finally yields a hard decision.
- **Lateral Scan**: hunt down the options you skipped because they were inconvenient, messy, or scary.
- **Zoom-out**: drag the whole system into the light and expose structural contradictions, hidden dependencies, and comforting lies.

## Why It Hits Hard

- It does not help you sound smart. It forces you to think harder.
- It does not accept “good enough”. It wants the stripped-down decision that survives pressure.
- It turns Claude Code / Codex into a feral cognitive hound that keeps chewing until every weak idea is gone.
- It is built for specs, architecture, roadmaps, product bets, prompt design, and any plan that still has soft spots.

## Install

If you are ready to feed it your brain, install it like this.

This repository is a dedicated single-skill repo, but it uses the standard `skills/consume-me/` layout so it works cleanly with the open `skills` CLI ecosystem.

It is also a pure text skill: no scripts, no binaries, no extra executables. From a distribution standpoint, it is very safe.

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

### openclaw

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -a openclaw
```

### Global install

```bash
npx skills@latest add hardydai-cell/consume-me --skill consume-me -g -y
```

### Preview before install

```bash
npx skills@latest add hardydai-cell/consume-me --list
```

## Where It Can Feed

This skill ships through the `skills` CLI workflow and can be installed into Codex, Claude Code, openclaw, OpenCode, Cursor, and many other agent environments.

## Example Prompts

- `Use $consume-me to eat through this product spec until only hard decisions remain.`
- `Use $consume-me to squeeze every lazy assumption out of this architecture plan.`
- `Use $consume-me to keep drilling until the last useful spark shows up.`

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

If you want a skill that nods along, flatters your half-formed thinking, and helps fuzzy nonsense look respectable, this is not that repo.  
If you want your agent to consume your brain until the last real idea breaks loose, install it.
