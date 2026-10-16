# Example — before / after

## Input (compressed project write-up)

> **Project: Smart Save for later**
>
> Members lose content between sessions. We will ship save/unsave from item
> detail plus a saved list. Goals: increase return visits to saved content;
> make save obvious and trustworthy. Non-goals: folders, AI recommendations,
> social sharing, offline sync. Success metrics: +8% save rate; retention TBD.
> Design is exploring detail-page control + list + empty state. Eng owns
> persistence and analytics. Open: where Saved lives in nav; whether unsave
> from list is in v1. Sharing ahead of a design review with PM + eng.

## Output (what the skill should produce)

```markdown
# Design alignment TL;DR — Smart Save for later

**Audience:** Stakeholders (PM, eng, design, partners)  
**From:** Design  
**Phase:** Exploration  
**Use:** Design review pre-read

## In one sentence
Members can save an item from detail view and find it again in a saved list — v1 is save/unsave + list, not collections or sharing.

## Why this exists
- Members lose track of content across sessions and have no reliable "come back later" path
- Product wants a clear habit loop before investing in folders / recommendations

## Goals
- **Product / business:** Raise save rate and return visits to saved content
- **Design success looks like:** Save is obvious on detail; returning to the list feels trustworthy; empty state teaches the habit instead of looking broken

## Scope
### In for this release
- Save / unsave from item detail
- Flat saved list with persisted state
- Empty-list educational state

### Out / later
- Folders, AI recommendations, shareable collections
- Social sharing, offline sync

## What design owns
- Detail-page save control and feedback
- Saved list (populated + empty) and row hierarchy
- IA entry to Saved (once nav decision lands)

## Not design's job
- Persistence / sync implementation (eng)
- Analytics event wiring (eng)
- Retention metric definition (PM)

## Status & next milestone
- **Now:** Exploring detail control + list + empty state
- **Next:** Lock nav placement and list actions, then move to hi-fi

## Risks & dependencies
- Nav placement unresolved — blocks where Saved lives in IA
- Unsave-from-list unclear — could change list interaction model

## Decisions needed from the room
1. Where does Saved live in nav — new tab, profile, or overflow? (PM + design)
2. Can users unsave from the list in v1, or only from detail? (PM + eng)

## Open questions
1. What does an "item" row need visually — thumbnail + title enough, or price/meta? (owner: design + PM)
```
