---
name: design-alignment-tldr
description: >-
  Distill a project's requirements, scope, and goals into a short, paste-ready
  TL;DR for stakeholder alignment — design reviews, kickoffs, or pre-reads for
  PMs, engineers, design managers, and other partners. Use when a designer
  wants a shared project summary, meeting topper, design-review pre-read,
  "are we aligned?", or requirements/scope/goals brief for mixed stakeholders
  — not when they need their own prioritized design task list (use
  design-spec-tldr for that).
icon: users
color: blue
---

# Design Alignment TL;DR

Turn project material into a **60-second alignment brief** anyone in the room
can scan: what the project is, why it matters, what's in/out of scope, what
design owns, and what still needs a decision.

You are writing **from the designer on the project, for shared stakeholder
alignment** (PM, eng, design manager, skip-level, partners) — not a PRD
rewrite, not an eng plan, and not a personal design-task backlog.

**Sibling skill:** For "what should *I* design first?" (P0/P1/P2 tasks from a
padded PRD), use `design-spec-tldr` instead.

## When to use

- Pre-read or top-of-meeting brief before a design review / critique
- Kickoff or alignment check with PM, eng, and design leadership
- "TL;DR of this project's requirements, scope, and goals"
- "Are we aligned?" / shared summary to paste in Slack, Notion, or the invite
- They have a PRD, epic, ticket dump, or notes and need a stakeholder-facing cut

## When not to use

- Designer wants their own prioritized design tasks → `design-spec-tldr`
- Competitive comps / pattern research → `competitive-research`
- Crazy 8 / rapid concepting → a concepting skill, not this one

## Inputs

Accept any of:

1. Pasted PRD / epic / ticket / meeting notes / Figma Discovery copy
2. A file, Notion, Confluence, or ticket link (fetch with available tools if needed)
3. Designer-spoken context ("we're doing X, goals are Y, out of scope is Z")

If the input is too thin to state goals and scope honestly, ask once for the
source material or the missing pieces. Do not invent product strategy.

Optional context (use if offered; do not block on it):

- Audience for this share (design review, kickoff, 1:1, Slack pre-read)
- Current phase (discovery, exploration, hi-fi, handoff, polish)
- Specific decisions they want the room to make

Load [references/example.md](references/example.md) if you need format calibration.

---

## Step 1 — Extract alignment-relevant signal

Read the whole input. Keep only what mixed stakeholders need to align:

| Bucket | Keep | Drop |
| --- | --- | --- |
| **Problem / opportunity** | Concrete user or business pain | Vision poetry, "north star" filler |
| **Goals** | Outcomes that justify the work | Vanity metrics with no product implication |
| **Scope** | Explicit in / out for this release | Speculative phase-2 wishlists |
| **Design ownership** | Surfaces, flows, content, research design leads | Pure eng / analytics / infra detail |
| **Constraints** | Brand, platform, legal, timeline, dependencies | Generic "best practices" |
| **Status & risk** | Where the work is, blockers, open decisions | Ceremony (standup format, Jira hygiene) |

**Alignment test:** If a bullet would not change how someone in the room
prioritizes, scopes, unblocks, or decides — cut it.

---

## Step 2 — Translate to a shared lens

Prefer crisp third-person project facts (easy to forward). Use ownership lines
("Design owns…", "Eng owns…") when they prevent crossed wires.

Always answer:

1. **What is shipping** (for users), in one sentence
2. **Why it matters** — user / business problem at stake
3. **What design is responsible for** vs what is not design's job
4. **What's in vs out** for the current release
5. **What still needs a decision** from the room (or FYI only)

Do not expand into a full work breakdown, critique agenda, or roadmap unless asked.

---

## Step 3 — Output format (always)

Keep the whole response short — aim for something pasteable into a meeting
invite, Slack, or the top of a design-review doc. Default to this structure and
**nothing else** unless the designer asks for more:

```markdown
# Design alignment TL;DR — [Project name]

**Audience:** Stakeholders (PM, eng, design, partners)  
**From:** Design  
**Phase:** [Discovery / Exploration / UI design / Handoff / Polish / Unknown]  
**Use:** [Design review pre-read / Kickoff / Alignment check / Unknown]

## In one sentence
[Who] can [do what] so that [outcome] — this release is [MVP cut], not [explicitly later].

## Why this exists
- [User / business problem — concrete]
- [Why now, if stated]

## Goals
- **Product / business:** …
- **Design success looks like:** [observable experience outcome, not "delight"]

## Scope
### In for this release
- …
### Out / later
- …

## What design owns
- …
- …

## Not design's job
- …

## Status & next milestone
- **Now:** …
- **Next:** …
- **Target / dependency:** … (only if known; else omit)

## Risks & dependencies
- …

## Decisions needed from the room
- [Who / what] …
- Or: *None — FYI / alignment only.*

## Open questions
1. … (owner: PM / eng / design / …)
2. …
```

### Style rules for the output

- Plain language. Short bullets. No corporate adjectives.
- Write so the designer can paste it with minimal edits.
- Do not mirror the PRD's section order or paste large quotes.
- Do not invent timelines, headcount, metrics, or scope.
- Do not produce wireframes, user stories, or eng tickets.
- If the source is contradictory or mostly fluff, say so in one blunt line under
  the one-sentence summary, then still give the best honest brief.
- Prefer **Decisions needed from the room** to be empty ("FYI / alignment only")
  unless something truly needs a call in that meeting.

---

## Optional follow-ups (only if asked)

- Tighter Slack / invite blurb (≤8 lines)
- "Top of meeting" spoken version (60 seconds)
- Companion designer task list via `design-spec-tldr` (P0/P1/P2)
- Critique-ready one-pager (problem, options considered, recommendation)

## Anti-patterns

- Dumping the full PRD under new headings
- Turning this into the designer's personal task backlog (that's `design-spec-tldr`)
- Strategy theater (principles, opportunity statements, north stars)
- Fake certainty on phase, dates, or staffing
- Softening ambiguity — call contradictions out under Open questions or Risks
- Addressing only design leadership when the share is for a mixed room
