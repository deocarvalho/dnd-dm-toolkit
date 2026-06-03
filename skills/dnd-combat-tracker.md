---
name: dnd-combat-tracker
description: Use this skill the moment combat begins — when initiative is rolled, when a creature attacks, or when the player declares a hostile action. Handles initiative, turn order, HP tracking, condition management, reaction prompts, and post-combat resource updates. Use alongside dnd-monster-behavior (enemy decision-making), dnd-resource-state (slot/HP tracking after combat), and dnd-death-saves (if character reaches 0 HP). Character stats are in the campaign setup skill.
---

# D&D Combat Tracker Skill

## Trigger Conditions
Activate this skill when:
- Player declares an attack or hostile action
- An enemy attacks or initiative is called for
- Any phrase like "roll initiative", "combat begins", "it attacks"

---

## Step 1: Initiative

Roll initiative for ALL parties before any actions resolve.

**Character's initiative:** d20 + DEX modifier (see campaign setup)
**Enemy initiative:** Roll per stat block

**Tie-breaking rule:** Higher DEX modifier wins. If still tied, ask player their preference.

Display initiative order clearly. Show the character's modifier; show enemies' rolled totals only (their modifiers are not information the character would have):
```
INITIATIVE ORDER
================
1. [Name] — Initiative XX
2. [Character] — rolled XX (+X DEX)
...
```

---

## Step 2: Combat State Block

Display this block at the start of combat and update it every round:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
COMBAT STATE — Round [X]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[CHARACTER NAME]
  HP: [X]/[MAX] | AC: [base] ([buffed if applicable])
  [Any active defensive buffs — per campaign setup]
  Concentration: [spell or None]
  Spell Slots: [by level, per campaign setup]
  Active conditions: [list or None]

ENEMIES
  [Name]: [Descriptive condition — see below]
  Active conditions: [list or None]

TURN: [Whose turn it is]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Step 3: Enemy HP — Descriptive Only

NEVER give exact enemy HP. Use descriptive language:
- **Full health:** "Uninjured, moving confidently"
- **Lightly wounded:** "A few minor wounds, still aggressive"
- **Bloodied (~50%):** "Bloodied, slowing slightly"
- **Badly hurt (~25%):** "Badly hurt, movements desperate"
- **Near death:** "Barely standing, one hit away"

---

## Step 4: Character's Turn

Prompt the player: **"[Character name]'s turn — what do you do?"**

Do NOT suggest actions or tactics unless explicitly asked.

After player declares action, resolve in this order:
1. Action (attack, spell, dash, etc.)
2. Bonus Action (if applicable)
3. Movement (if applicable)
4. Note any free object interactions

### CRITICAL: Spell Slot Tracking

**Every time a levelled spell is cast, immediately:**
1. Deduct the slot from the running count in the Combat State block
2. Confirm the new total out loud: *"2nd level slot spent — 2nd slots: 2/3 remaining"*
3. Update the block before resolving the next turn

**Do not wait until post-combat to reconcile slots.** Slot tracking errors compound across a long combat and become irreconcilable. Track every single cast the moment it happens.

If the player corrects a slot count mid-combat, accept the correction immediately and update the block. Do not argue. Do not recalculate independently — the player's confirmed count is authoritative.

---

## Step 5: Enemy Turn — ALWAYS Offer Reactions First

Before resolving ANY attack that hits the character:

> "[Enemy] attacks [character] — rolled [X] vs AC [X]. That hits. **Do you want to use any reaction before I resolve damage?**"

Wait for player response before applying damage. If a reaction costs a spell slot, deduct it immediately.

After player responds, apply damage and roll concentration check if applicable.

### Opportunity Attacks

When a creature moves out of the character's melee reach, offer the opportunity attack BEFORE the move completes:

> "[Creature] is moving away from you — do you want to make an opportunity attack (reaction) before they leave your reach?"

Use the character's melee attack modifier from campaign setup. Using a reaction here means no further reactions until the start of their next turn.

Check campaign setup for any feats or abilities that modify what the character can do as an opportunity attack.

---

## Step 6: Concentration Checks

If the character takes damage while concentrating on a spell:
> "Concentration check required — DC [half damage taken, min 10]. Roll CON save ([modifier from campaign setup])."

Wait for player's roll. Check campaign setup for any features that affect this save (e.g. advantage from feats).

On failure, concentration ends — note the spell. On success, the spell continues.

---

## Step 7: Conditions Tracking

Track all conditions and their sources. The DC for any saving throw to end a condition equals the spell save DC of whatever caused it — check the source's stat block or campaign setup.

- **Grappled:** Movement 0; escape requires an action + Athletics or Acrobatics vs. the grappler's Athletics DC
- **Restrained:** Speed 0; attacks against have advantage, own attacks have disadvantage; DEX saves at disadvantage
- **Prone:** Speed halved to stand up; melee attacks against have advantage, ranged attacks have disadvantage
- **Poisoned:** Disadvantage on attack rolls and ability checks
- **Frightened:** Can't move toward the source of fear; disadvantage on ability checks and attack rolls while the source is in sight
- **Paralyzed:** Incapacitated; can't move or speak; auto-fail STR and DEX saves; attacks against have advantage; hits within 5 ft are critical hits
- **Slow:** Speed halved; −2 AC and DEX saves; no reactions; action OR bonus action each turn (not both); one attack per turn if the Attack action is taken; WIS save at end of each of the affected creature's turns to end the effect
- **Invisible:** Attacks against have disadvantage; own attacks have advantage. Duration and end conditions depend on the source — check the spell or ability that granted it

Note round duration for any timed conditions.

---

## Step 8: Character Stat Reference

All character stats (AC, HP, initiative modifier, attack bonuses, save DC, CON save, passive perception, spell slots by level, spell list, and relevant feats) are in the **campaign setup skill**.

Load that skill at the start of the session. Refer to it throughout combat for exact numbers.

---

## Step 9: Post-Combat Update

After combat ends, immediately display updated resources:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
POST-COMBAT RESOURCES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
HP: [X]/[MAX]
Spell Slots: [by level, per campaign setup]
Hit Dice remaining: [X/total]
Concentration: [active spell or None]
Consumables: [potions, items — per campaign setup]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

If there is ANY discrepancy between the tracked count and the player's recollection, the player's count is authoritative. Update and note the correction.

---

## Step 10: Character at 0 HP — Activate Death Saves Skill

When the character is reduced to 0 HP, immediately switch to the **`dnd-death-saves`** skill. It governs the full dying sequence: death save rolls, stabilization, coup de grâce, instant death, and recovery.

Do not continue the combat turn until the death save situation has been announced to the player.

---

## Hard Rules — Never Break These

- NEVER reveal exact enemy HP
- NEVER suggest tactics or tell the player what to do
- ALWAYS offer reactions before resolving any hit
- ALWAYS roll dice transparently: show the roll, modifier, and total
- ALWAYS check for concentration when the character takes damage
- ALWAYS deduct spell slots immediately when cast — never defer
- ALWAYS confirm updated slot count after every levelled spell
- Initiative ties: higher DEX wins, or ask the player
- Opportunity attacks: offer them before the triggering move completes
- Large creatures occupy a 10×10 space and threaten all squares within 5 ft of that space — account for this when adjudicating reach and opportunity attacks
- Timed conditions: track their end triggers every turn without being prompted
- ALWAYS activate the dnd-death-saves skill the moment the character hits 0 HP
