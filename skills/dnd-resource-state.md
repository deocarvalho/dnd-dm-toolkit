---
name: dnd-resource-state
description: Use this skill after every combat, every rest (short or long), every spell cast, and every item use. Tracks HP, spell slots, hit dice, active spells, and consumables. Also use when the player asks "what resources do I have?" or "what's my status?" Character stats, spell lists, and starting baseline are in the campaign setup skill.
---

# Resource State Tracker Skill

## When to Activate

Trigger after ANY of these events:
- Combat ends
- A spell is cast (any level)
- A potion or consumable is used
- A long-duration spell is cast or expires (e.g., Mage Armor, Arcane Eye)
- The familiar is dismissed, killed, or re-summoned
- Items are looted, sold, or purchased (update GP)
- A short rest completes
- A long rest completes
- Player asks about current resources

---

## Character Stats

Maximum HP, hit dice, spell slots, spell list, and starting consumables are in the **campaign setup skill**. Load that skill at the start of each session and use it as the baseline.

---

## Resource Block Format

Always display resources in this format when updating:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[CHARACTER NAME]'S RESOURCES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
HP:           [X]/[MAX]
Hit Dice:     [X]/[total] remaining

Spell Slots:
  [list by level, e.g.:]
  1st level:  [X]/[max]
  2nd level:  [X]/[max]
  3rd level:  [X]/[max]

[Long-duration spells, e.g.:]
  Mage Armor: [Active — ~X hrs remaining / Inactive]

Concentration: [Spell name + duration, or None]
Active Effects: [Any other buffs/conditions]

Consumables:
  [List all tracked items with counts]
  Familiar: [Alive / Dead — needs ritual recast]

GP: [X]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Rest Rules

### Short Rest (1 hour)
- Player may spend any number of Hit Dice
- Each die: roll the hit die + CON modifier = HP recovered
- Cannot exceed max HP
- **Arcane Recovery** (Wizard, once per day): recover spell slots totaling up to half Wizard level rounded up
  - Cannot recover 6th level or higher slots
  - Example for level 5 Wizard: up to 3 levels worth (one 3rd, or one 2nd + one 1st, etc.)

### Long Rest (8 hours)
- HP fully restored to maximum
- All spell slots recovered
- Hit Dice recovered: half of total rounded down (minimum 1)
- Arcane Recovery resets
- All daily abilities reset
- Long-duration spells (Mage Armor, etc.) may still be active if cast recently enough

---

## Concentration Tracking

Only ONE concentration spell active at a time. Starting a new one ends the previous immediately.

When the character takes damage while concentrating:
- CON saving throw required
- DC = max(10, half damage taken)
- Use the CON save modifier from the campaign setup
- Failure = concentration ends

---

## Familiar Tracking

If the character has a familiar (see campaign setup):
- **Dismissed:** Safe. Can be resummon as a bonus action (from within range).
- **Dead:** Requires the ritual version of *Find Familiar* to resummon — typically 1 hour, no spell slot cost, but takes real time and cannot be done mid-combat.
- Track state clearly: Alive / Dismissed / Dead.

---

## GP Tracking

Update GP immediately on any transaction:
- Items or loot acquired → add value when sold, or note as inventory
- Items purchased or services paid → subtract cost
- Confirm amounts with the player before recording if uncertain

---

## Notes
- Trust player's numbers but note any discrepancies politely
- If player corrects a resource count, update immediately
- Always show resources after combat and after rests — don't wait to be asked
- Track new items as they're acquired, even before they're sold or identified
- After level-up: update HP MAX, HIT DICE, and SPELL SLOTS before the next adventure. The level-up confirmation in the session summary is the source of truth.
- At adventure start: confirm actual state with the player rather than assuming the campaign setup baseline.
