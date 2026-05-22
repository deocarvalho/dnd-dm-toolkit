---
name: dnd-session-summary
description: Use this skill at the end of every adventure, or when the player asks for a session summary. Produces a structured summary file that preserves everything needed to start the next session — events, resources, loot, decisions, NPCs, and unresolved threads. File naming convention and campaign details are in the campaign setup skill.
---

# Session Summary Skill

## When to Activate

- Player says "end of session," "let's wrap up," or "summarize what happened"
- Adventure reaches its conclusion
- After "End of Adventure [N]" is declared
- Session ends mid-adventure (see Partial Summary section below)

---

## Summary File Format

Produce the summary in this exact structure. Save it to the `/summaries/` folder using the file naming convention from the campaign setup skill (e.g., `/summaries/[campaign-code]-[N]-summary.md`).

```markdown
# ADVENTURE SUMMARY: "[ADVENTURE TITLE]"

## Adventure Overview
**Adventure Number:** [N]
**Level Range:** Started at Level [X] ([class breakdown]), ended at Level [Y]
**Location:** [Primary setting]
**Duration:** [Approximate in-world time]

## Initial Hook
[How Auriel got involved — 2-4 sentences]

## Key Events
[Chronological summary of major scenes, decisions, and discoveries]
[Use ### subheadings for major areas or scenes]
[For each room/area: what happened, what was found, what was learned]

## Combat Encounters
[For each combat:]
### [Enemy Name(s)] — [Location]
- Setup: [How combat started]
- Key moments: [Interesting tactical moments, spells used, close calls]
- Resolution: [How it ended]
- Resources spent: [HP lost, spell slots used, items consumed]
- Loot: [What was found]

## NPCs Encountered
[For each NPC:]
**[Name]** — [Role/description]
- Personality: [Brief notes]
- What they know/provided: [Information or items given]
- Current status: [Alive/dead/location]
- Relationship to Auriel: [Friendly/neutral/hostile/unknown]

## Puzzles & Discoveries
[Any puzzles solved, secrets found, lore uncovered]

## Items Acquired
[Full loot list with GP values if known]

## Items Sold/Spent
[What was sold, to whom, for how much]

## Final Resources at Adventure End
**HP:** [X]/[max]
**Spell Slots:** [by level — e.g., 1st [X/max] | 2nd [X/max] | 3rd [X/max]]
**Hit Dice:** [X/total] remaining
**Consumables:** [List all tracked items with counts]
**GP:** [Total]
**New permanent items:** [List]

## Key Decisions Made
[Choices Auriel made that might have consequences]
[Include: who was helped/harmed, what was taken/left behind, alliances formed]

## Unresolved Threads
[Loose ends, open questions, potential future hooks]
[Do NOT invent or speculate — only list things explicitly present in the adventure]

## Campaign Status After This Adventure
**Auriel's Level:** [X] ([class breakdown])
**Base of Operations:** [Location]
**Active Quest:** [Main goal]
**Known Allies:** [List]
**Known Enemies/Threats:** [List]
**Ongoing Mysteries:** [List]

---

**End of Adventure [N]**
```

---

## Rules for Summary Content

**Include:**
- Everything that happened, factually
- Exact resource counts as confirmed by player
- NPC names, personalities, and what they revealed
- Every item acquired (whether kept or sold)
- All decisions made by the player, without judgment
- Unresolved plot threads from the adventure text

**Do NOT include:**
- Invented plot hooks not in the adventure text
- Speculation about what threads "might lead to"
- Claude's opinions or commentary on player decisions
- Foreshadowing or hints at future adventures

**On mechanics errors:** Record final resource state using correct RAW rules, even if different from what was tracked during play. If a slot was spent that should not have been, or a rule was applied incorrectly, note the correction briefly at the end: *"Correction: 1× 2nd-level slot refunded per rules clarification."* Do not silently preserve an error in the numbers.

---

## Post-Summary Checklist

After producing the summary, confirm:

1. ✅ Level advancement noted (per campaign leveling rule in campaign setup)
2. ✅ All resources accurately reflected
3. ✅ All loot accounted for (kept and sold)
4. ✅ All NPCs recorded with status
5. ✅ Unresolved threads listed
6. ✅ "End of Adventure [N]" stated explicitly

Then wait for the player to:
- Upload the summary file to the project
- Provide the next adventure text
- Confirm level-up choices

Do NOT invent the next adventure or create bridging content.

If the player does not provide the next adventure file, prompt once: *"When you're ready for the next adventure, please upload the chapter file from the project."* Then wait.

---

## Partial Summary (Session Ends Mid-Adventure)

If a session ends before the adventure concludes, produce a partial summary using this format. Save it using the campaign file naming convention from the campaign setup skill (e.g., `[campaign-code]-[N]-partial.md`).

```markdown
# PARTIAL SUMMARY: "[ADVENTURE TITLE]" — Session [date or number]

## Current Status
**Adventure Number:** [N]
**Current Level:** [X] ([class breakdown])
**Current Location:** [Exact room or area — be specific]
**Session ended:** [brief note on where Auriel stopped]

## Events So Far
[Chronological summary of everything that happened this session, organized by scene]
[Use the same structure as the full summary's Key Events section]

## Current Resources
**HP:** [X]/[max]
**Spell Slots:** 1st [X/4] | 2nd [X/3] | 3rd [X/3]
**Hit Dice:** [X/6] remaining
**Mage Armor:** [Active / Inactive]
**Concentration:** [Spell or None]
**Consumables:** [List]
**GP:** [Total]

## NPCs Encountered This Session
[Same format as full summary — name, status, relationship, anything they revealed]

## Items Acquired This Session
[Full list, whether kept or not]

## Open Threads
[What Auriel knows, what she's trying to do, what she has not yet explored]
[This is what gets picked up at the next session — be precise]

---
**Partial — Adventure [N] in [Campaign Name] continues**
```

When resuming: player uploads this partial summary instead of a full summary. Pick up exactly where the location and open threads indicate. Do not replay events already summarized.
