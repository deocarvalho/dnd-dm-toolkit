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
  [Mage Armor or equivalent: Active / Inactive — if relevant]
  Concentration: [spell or None]
  Spell Slots: [by level per campaign setup]
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

---

## Step 5: Enemy Turn — ALWAYS Offer Reactions First

Before resolving ANY attack that hits Auriel:

> "[Enemy] attacks Auriel — rolled [X] vs AC [X]. That hits. **Do you want to use Shield or any other reaction before I resolve damage?**"

Wait for player response before applying damage.

**Shield spell:** costs 1st-level slot, raises AC by 5 until start of next turn (may turn a hit into a miss — recalculate).

After player responds, apply damage and roll concentration check if applicable.

### Opportunity Attacks

When a creature moves out of Auriel's melee reach, offer the opportunity attack BEFORE the move completes:

> "[Creature] is moving away from you — do you want to make an opportunity attack (reaction) before they leave your reach?"

An opportunity attack uses Auriel's melee spell attack (+6) or a melee weapon roll. Using the reaction means no Shield until the start of her next turn.

---

## Step 6: Concentration Checks

If the character takes damage while concentrating on a spell:
> "Concentration check required — DC [half damage taken, min 10]. Roll CON save ([modifier from campaign setup])."

Wait for player's roll. On failure, concentration ends, note the spell.

---

## Step 7: Conditions Tracking

Track all conditions and their sources:
- **Grappled:** Movement 0, escape requires action + Athletics/Acrobatics vs DC
- **Restrained:** Speed 0, attacks against have advantage, own attacks have disadvantage
- **Invisible (Invisibility / Vanish):** Attacks against have disadvantage, own attacks have advantage — ends immediately after Auriel attacks or casts a spell
- **Invisible (Greater Invisibility):** Same attack/defense benefits — does NOT end when attacking or casting; persists until the spell's duration ends
- **Prone:** Speed halved to stand, melee attacks have advantage, ranged attacks have disadvantage
- **Poisoned:** Disadvantage on attack rolls and ability checks

Note round duration for any timed conditions.

---

## Step 8: Character Stat Reference

All character stats (AC, HP, initiative, spell attack, save DC, CON save, passive perception, spell slots, and spell list) are in the **campaign setup skill**.

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

---

## Step 10: Character at 0 HP — Activate Death Saves Skill

When the character is reduced to 0 HP, immediately switch to the **`dnd-death-saves`** skill. It governs the full dying sequence: death save rolls, stabilization, coup de grâce, instant death, and recovery.

Do not continue the combat turn until the death save situation has been announced to the player.

---

## Hard Rules — Never Break These

- NEVER reveal exact enemy HP
- NEVER suggest tactics or tell the player what to do
- ALWAYS offer reaction opportunity before resolving hits
- ALWAYS roll dice transparently: show the roll, modifier, and total
- ALWAYS check for concentration when Auriel takes damage
- Initiative ties: higher DEX wins, or ask the player
- Invisible (Invisibility): advantage on attacks, ends after attacking or casting
- Invisible (Greater Invisibility): advantage on attacks, does NOT end on attack or cast
- ALWAYS offer opportunity attack when a creature leaves Auriel's melee reach
- ALWAYS activate the dnd-death-saves skill the moment the character hits 0 HP
