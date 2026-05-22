---
name: dnd-ability-checks
description: Use this skill whenever a player attempts something that might warrant a D20 Test — an ability check, saving throw, or attack roll outside combat. Governs when to call for rolls, which ability to use, what DC to set, when to apply Advantage or Disadvantage, and how to handle failure. Use alongside dnd-room-description during exploration and dnd-npc-voice during social scenes. Prevents calling for unnecessary rolls and ensures DCs are consistent across the campaign.
---

# Ability Checks Skill

## Core Principle

Do not call for a D20 Test unless there is a meaningful chance of both success **and** failure, AND meaningful consequences for failure.

If the task is trivial, simply say it succeeds. If it's impossible, say so. A roll is only warranted when both outcomes — success and failure — have something interesting to contribute to the scene.

**Before calling for any roll, ask:** What happens on success? What happens on failure? If you can't answer both, don't roll.

---

## When NOT to Roll

- The task is trivially easy for anyone (opening an unlocked door, crossing an empty room): describe success
- The task is impossible regardless of the roll: describe the impossibility
- The character has time, no pressure, and can simply try repeatedly: describe how long it takes and move on
- Failure would have no consequence beyond "try again with no cost": skip the roll entirely

---

## Which Test to Call

| Situation | Test Type |
|-----------|-----------|
| Character actively tries to accomplish something | Ability check |
| Character is trying to hit something | Attack roll |
| Character reactively resists or avoids an effect | Saving throw |

Ability checks represent active effort. Saving throws represent reactive resistance. Don't use saving throws for things the character is actively attempting, and don't use ability checks for things they are being forced to resist.

---

## Setting the DC

| Difficulty | DC | Notes |
|------------|----|-------|
| Very easy | 5 | Most people succeed; skip the roll unless the stakes matter |
| Easy | 10 | A character with 10 in the relevant ability and no proficiency succeeds ~50% of the time |
| Moderate | 15 | Typically requires a higher score or proficiency to succeed consistently |
| Hard | 20 | Usually requires both a strong score and proficiency |
| Very hard | 25 | Out of reach for most low-level characters |
| Nearly impossible | 30 | Only exceptional characters at high level have a reasonable chance |

**Rule of thumb:** Use 10, 15, and 20 for most situations. If you can't decide between two difficulty levels, pick a number in between (17–18 for "between moderate and hard").

If the adventure text specifies a DC, use it — don't override it.

For saving throws, don't set DCs below 10 or above 20 unless a specific rule calls for it. Spells and abilities that impose saving throws use the formula: **DC = 8 + ability modifier + proficiency bonus**.

---

## Choosing the Ability

Ask: what ability has the most influence on the character's chance to succeed?

| Ability | Ability Checks | Saving Throws |
|---------|----------------|---------------|
| Strength | Lift, push, pull, break | Physically resist direct force |
| Dexterity | Move nimbly, quietly, quickly | Dodge out of harm's way |
| Constitution | Push body beyond normal limits | Endure a toxic or exhausting hazard |
| Intelligence | Reason, remember, research | Recognize an illusion as false |
| Wisdom | Notice things in the environment or in behavior | Resist a mental assault |
| Charisma | Influence, entertain, deceive | Assert identity against magical compulsion |

Be generous about letting skill and tool proficiencies apply. If a player argues their proficiency is relevant, hear them out — it often is. You can ask for an Intelligence check and let the player propose which skill might apply.

---

## Perception vs. Investigation

These are the most commonly confused checks. They serve different purposes.

### Wisdom (Perception)
Use when a character is **noticing something** — detecting a hidden creature, sensing a concealed door, hearing an unusual sound, smelling something out of place.

Perception answers: **"Is there something here to find?"**

### Intelligence (Investigation)
Use when a character is **figuring out how something works** — how to open a trick door, what a clue reveals, how a mechanism is constructed, what the evidence in a room suggests.

Investigation answers: **"How does this work?" or "What does this mean?"**

### The Sequence
A character can use both in sequence: a successful Perception check reveals that the bookcase isn't flush with the wall. A successful Investigation check then figures out the trick to opening it.

Do NOT use Investigation to determine whether a character notices something. That is Perception's job.

---

## Passive Checks

Passive Perception is 10 + all modifiers that apply to a Wisdom (Perception) check.

Use passive checks when:
- Asking for an active roll would tip off the player that something hidden exists
- You want to know if a character would routinely notice something without drawing attention to it
- The character is moving through an area without actively searching

For other skills (Insight, Investigation, History), you can establish passive scores the same way: 10 + relevant modifiers. These are especially useful in social encounters where rolling might signal to the player that something is being hidden from them.

---

## Advantage and Disadvantage

### Grant Advantage when:
- Circumstances outside the character's own abilities give them an edge
- An environmental factor improves the chance of success
- The player describes a creative or exceptionally well-reasoned approach
- A previous action (by the character or an ally) has improved the situation

### Impose Disadvantage when:
- Circumstances hinder success
- An environmental factor makes success less likely
- The character's approach has a meaningful flaw that would complicate the attempt

Advantage and Disadvantage always cancel out, regardless of how many sources there are on each side. Multiple advantages do not stack.

---

## Group Checks

Use when the party is trying to accomplish something together and skilled characters can compensate for less skilled ones.

**Procedure:** Everyone in the group makes the check. If at least half succeed, the whole group succeeds. Otherwise the group fails.

### When to use group checks:
- Research tasks where multiple characters can contribute different sources
- Roped-together climbing where strong climbers can catch weaker ones
- Group negotiations where a few smooth talkers can cover for awkward party members

### When NOT to use group checks:
- One failure would be a disaster (e.g., group stealth where one noisy character alerts the guards — use individual checks)
- One success is sufficient (e.g., finding a hidden door — the first character who finds it, finds it)

---

## Consequences of Failure

### Can They Try Again?
- If failure has no cost and the character can retry indefinitely, skip the roll. Say how long it takes and move on.
- If failure has a cost (time, noise, damage, alerting enemies), call for the roll and enforce the consequence.

### Success at a Cost
When a character fails by only 1 or 2, you may offer them success at the price of a complication:
- They pick the lock, but the noise was audible
- They climb the wall, but lose their grip and take minor damage
- They persuade the guard, but the guard now wants something in return

Put the choice in the player's hands when possible — it gives them agency in how the story unfolds.

### Degrees of Failure
Failing by 5 or more can carry heavier consequences than a narrow miss:
- Failing a DC 15 Dexterity (Sleight of Hand) check by 1–4: the lock doesn't open
- Failing by 5 or more: the lockpick snaps, requiring new tools

Use degrees of failure sparingly and only when the distinction creates an interesting situation, not just to pile on bad luck.

---

## Hidden Things

**Never hide adventure-critical information behind a single ability check that the characters might fail.**

If the characters must find something to progress, make it findable. Either:
- Set the DC within passive perception range, or
- Plant a visible hint that invites active searching, or
- Provide an alternate path to the same information

Extra treasures, optional secrets, and bonus discoveries can be hidden behind checks. Required clues and path-forward information must not be completely blocked by a failed roll.

**Plant hints:** A slight rattle in a drawer suggests a hidden compartment. Footprints leading to a blank wall suggest a secret door. These hints invite players to search actively rather than relying on lucky passive rolls.

---

## Trying Again

Failure at an ability check does not automatically mean the character can never try again. Consider:

- **Locks, mechanisms, puzzles:** Each attempt takes time; failure is a delay, not a permanent block
- **Social situations:** A failed Persuasion check might mean "not now" or "not without more" — rarely "never again"
- **Physical tasks:** Can often be reattempted after rest, better tools, or a different approach

When failure makes a retry impossible (the door is jammed, the NPC is now hostile), say so clearly so the player understands the situation has changed.
