# Design Alignment TL;DR

A portable **Cursor Agent Skill** that turns project requirements, scope, and goals into a short, paste-ready **alignment brief** for mixed stakeholders — design reviews, kickoffs, and meeting toppers for PMs, engineers, design managers, and partners.

Not a personal design-task backlog (use [`design-spec-tldr`](https://github.com/brianbeavers/design-spec-tldr-skill) for that).

## Quick start

```bash
mkdir -p ~/.cursor/skills
git clone https://github.com/brianbeavers/design-alignment-tldr-skill.git ~/.cursor/skills/design-alignment-tldr
```

In Cursor Agent chat:

```text
/design-alignment-tldr

[paste PRD / notes / epic — or point at a doc]
```

Or copy this folder into a project as `.cursor/skills/design-alignment-tldr/`.

## What it does

Produces a **60-second scan** anyone in the room can use:

- What the project is (one sentence)
- Why it exists
- Goals (product + design success)
- Scope in / out
- What design owns vs not design’s job
- Status & next milestone
- Risks, dependencies, asks, open questions

## Repo layout

| Path | Role |
| --- | --- |
| [`SKILL.md`](SKILL.md) | Skill instructions (agent loads this) |
| [`references/example.md`](references/example.md) | Format calibration / sample brief |

## Sibling skill

| Skill | Use when… |
| --- | --- |
| [`design-spec-tldr`](https://github.com/brianbeavers/design-spec-tldr-skill) | Designer wants *their* prioritized P0/P1 design tasks from a padded PRD |
| **design-alignment-tldr** (this) | Shared stakeholder alignment / pre-read / “are we aligned?” |

## License

MIT — see [LICENSE](LICENSE).
