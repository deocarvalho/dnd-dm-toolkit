# D&D DM Toolkit

A set of Claude AI skills and adventure files for running official D&D 5th Edition adventures as an AI-assisted Dungeon Master.

## Repository Structure

```
/skills/        Claude skill files (.md) — loaded into the Claude project
/adventures/    Adventure chapter files (.md) — one file per adventure
/summaries/     Session and adventure summaries (.md) — created after each session
/reference/     DM reference material (DMG chapters, etc.)
```

## How to Use

1. **Claude Project setup:** Connect this repository to a Claude Project. All files sync automatically — no manual uploading needed.
2. **Starting a session:** Tell Claude which adventure to run (from `/adventures/`) and which summary to load as context (from `/summaries/`), if one exists.
3. **After a session:** Save the summary Claude generates to `/summaries/` and commit it to keep the project in sync.
4. **Level-ups / major changes:** Update `skills/dnd-campaign-setup.md` to reflect new stats, spells, and equipment, then commit and push.

## Skills Overview

| Skill | Purpose |
|-------|---------|
| `dnd-campaign-setup` | Single source of truth — character stats, spells, equipment, NPCs, campaign details |
| `dnd-combat-tracker` | Step-by-step combat flow, initiative, actions, conditions |
| `dnd-death-saves` | Handles 0 HP, death saving throws, stabilization |
| `dnd-monster-behavior` | Tactical monster AI — targeting, morale, fleeing, parley |
| `dnd-ability-checks` | D20 test adjudication — when to roll, DCs, outcomes |
| `dnd-room-description` | Environment narration — prioritises adventure read-aloud text; filters secrets from DM-only descriptions; lighting and vision rules |
| `dnd-npc-voice` | Consistent NPC portrayal, attitudes, social mechanics |
| `dnd-adventure-fidelity` | Keeps Claude grounded in the written adventure text |
| `dnd-resource-state` | Tracks HP, spell slots, consumables during play |
| `dnd-session-summary` | Produces structured summaries at session or adventure end |

## Current Campaign

- **Campaign:** Candlekeep Mysteries (Forgotten Realms — standalone anthology adventures)
- **Character:** Auriel Harpell — Male Half-Elf, Cleric (Knowledge Domain) 1 / Wizard (Order of Scribes) 5, Level 6
- **Progress:** Adventures 1–5 completed; summaries in `/summaries/`

## Reuse for a New Campaign

Skills are designed to be **generic and reusable** across campaigns and characters. All campaign- and character-specific data lives in `skills/dnd-campaign-setup.md`. To start a new campaign:

1. Duplicate `dnd-campaign-setup.md` and fill in the new character and campaign details
2. Add adventure files to `/adventures/`
3. Clear or archive `/summaries/`
