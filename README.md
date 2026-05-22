# D&D DM Toolkit

A set of Claude AI skills and adventure files for running official D&D 5th Edition adventures as an AI-assisted Dungeon Master.

## Repository Structure

```
/skills/        Claude skill files (.md) — loaded into the Claude project
/adventures/    Adventure chapter files (.md) — uploaded per session
/summaries/     Session and adventure summaries (.md) — created after each session
/reference/     DM reference material (DMG chapters, etc.)
```

## How to Use

1. **Claude Project setup:** Connect this repository to a Claude Project. The `/skills/` folder contains all skill files that teach Claude how to run the game.
2. **Starting a session:** Tell Claude which adventure chapter to load from `/adventures/` and which summary (if any) from `/summaries/`.
3. **After a session:** Save the generated summary file to `/summaries/` and push to keep the project in sync.
4. **Level-ups / major changes:** Update `skills/dnd-campaign-setup.md` to reflect new stats, spells, and equipment.

## Skills Overview

| Skill | Purpose |
|-------|---------|
| `dnd-campaign-setup` | Single source of truth — character stats, spells, equipment, NPCs |
| `dnd-combat-tracker` | Step-by-step combat flow, initiative, actions, conditions |
| `dnd-death-saves` | Handles 0 HP, death saving throws, stabilization |
| `dnd-monster-behavior` | Tactical monster AI — targeting, morale, fleeing, parley |
| `dnd-ability-checks` | D20 test adjudication — when to roll, DCs, outcomes |
| `dnd-room-description` | Environment narration, lighting, perception vs. investigation |
| `dnd-npc-voice` | Consistent NPC portrayal, attitudes, social mechanics |
| `dnd-adventure-fidelity` | Keeps Claude grounded in the written adventure text |
| `dnd-resource-state` | Tracks HP, spell slots, consumables during play |
| `dnd-session-summary` | Produces structured summaries at session or adventure end |

## Campaign Notes

- Skills are designed to be **generic and reusable** across campaigns and characters.
- All character- and campaign-specific data lives in `skills/dnd-campaign-setup.md`.
- To start a new campaign: duplicate `dnd-campaign-setup.md`, fill in the new character and campaign details, and update file path conventions.
