# Frontciti Skill

<p align="center">
  <img src="assets/frontciti-mark.svg" alt="Frontciti mark" width="260">
</p>

Frontciti is a frontend design, redesign, SaaS UI, dashboard, component, and motion skill for AI coding agents.

It helps coding agents produce frontend work with stronger taste, better UX, cleaner design systems, accessibility, responsive behavior, and purposeful animation.

## Install

### Codex

```bash
tmp="$(mktemp -d)"
git clone --depth 1 https://github.com/sandilyapoorv/Frontciti.git "$tmp/frontciti"
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
rm -rf "${CODEX_HOME:-$HOME/.codex}/skills/frontciti"
cp -R "$tmp/frontciti/skills/frontciti" "${CODEX_HOME:-$HOME/.codex}/skills/frontciti"
```

Then start a new Codex thread and ask for `$frontciti`, for example:

```txt
Use $frontciti to redesign this dashboard with stronger hierarchy, responsive states, and production polish.
```

### Claude Code

```bash
tmp="$(mktemp -d)"
git clone --depth 1 https://github.com/sandilyapoorv/Frontciti.git "$tmp/frontciti"
mkdir -p "$HOME/.claude/skills"
rm -rf "$HOME/.claude/skills/frontciti"
cp -R "$tmp/frontciti/skills/frontciti" "$HOME/.claude/skills/frontciti"
```

### Cursor

From your project root:

```bash
tmp="$(mktemp -d)"
git clone --depth 1 https://github.com/sandilyapoorv/Frontciti.git "$tmp/frontciti"
mkdir -p .cursor/rules
cp "$tmp/frontciti/adapters/cursor-rules/frontciti.mdc" .cursor/rules/frontciti.mdc
```

### VS Code / Copilot-Style Agents

From your project root:

```bash
tmp="$(mktemp -d)"
git clone --depth 1 https://github.com/sandilyapoorv/Frontciti.git "$tmp/frontciti"
mkdir -p .github
cp "$tmp/frontciti/adapters/copilot-instructions.md" .github/copilot-instructions.md
```

### Generic Agent Instructions

For tools that read `AGENTS.md` from a project root:

```bash
tmp="$(mktemp -d)"
git clone --depth 1 https://github.com/sandilyapoorv/Frontciti.git "$tmp/frontciti"
cp "$tmp/frontciti/adapters/AGENTS.md" AGENTS.md
```

## Compatibility

Frontciti is packaged as an agent skill and includes adapters for tools that use project rules instead of native skills.

| Tool | Status | How to use |
| --- | --- | --- |
| Codex | Native | Install or copy `skills/frontciti/` into a Codex skills directory. |
| Claude Code | Native-compatible | Use `skills/frontciti/` as a skill package, or use `adapters/CLAUDE.md` as project guidance. |
| Cursor | Adapter | Copy `adapters/cursor-rules/frontciti.mdc` to `.cursor/rules/frontciti.mdc`. |
| VS Code agents / Copilot-style setups | Adapter | Use `adapters/copilot-instructions.md` as the project instruction file, commonly `.github/copilot-instructions.md` where supported. |
| Antigravity | Adapter | Add `adapters/antigravity-rules.md` to the project's Antigravity rules or agent instructions. |

For generic agent setups that read `AGENTS.md`, use `adapters/AGENTS.md`.

## What It Handles

- Landing pages.
- SaaS apps.
- Dashboards.
- Admin panels.
- Client portals.
- Components.
- UX shaping and end-to-end frontend craft.
- Redesigns.
- Design critiques.
- UI audits.
- Design systems.
- Typography, color, layout, copy, onboarding, and responsive adaptation.
- Frontend polish.
- GSAP and motion animation.
- Production hardening.
- Image-first visual design-to-code workflows.

## Commands

- `/frontciti init`
- `/frontciti shape`
- `/frontciti craft`
- `/frontciti landing`
- `/frontciti saas`
- `/frontciti dashboard`
- `/frontciti component`
- `/frontciti redesign`
- `/frontciti critique`
- `/frontciti audit`
- `/frontciti polish`
- `/frontciti animate`
- `/frontciti harden`
- `/frontciti design-system`
- `/frontciti extract`
- `/frontciti bolder`
- `/frontciti quieter`
- `/frontciti distill`
- `/frontciti delight`
- `/frontciti layout`
- `/frontciti typeset`
- `/frontciti colorize`
- `/frontciti clarify`
- `/frontciti onboard`
- `/frontciti adapt`
- `/frontciti optimize`
- `/frontciti image-first`

## Usage

Use Frontciti when asking an AI coding agent to build, redesign, audit, polish, or animate frontend interfaces.

```txt
Use /frontciti saas to redesign this dashboard into a premium B2B SaaS interface. Keep the existing functionality, improve hierarchy, add realistic states, and make it responsive.
```

```txt
Use /frontciti landing to create a high-converting landing page for this product. Avoid generic AI-looking sections. Make the hero specific and memorable.
```

```txt
Use /frontciti animate to add a tasteful GSAP animation to the hero and feature reveal sections. Respect reduced motion and keep performance clean.
```

```txt
Use /frontciti critique to review this dashboard for AI-looking patterns, hierarchy issues, accessibility gaps, and production risks.
```

## Philosophy

Frontciti is not just a UI beautifier. It helps the agent understand product intent, user task, brand tone, information architecture, interaction states, responsive behavior, and motion purpose before implementing.
