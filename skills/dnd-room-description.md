---
name: dnd-room-description
description: Use this skill whenever the character enters a new room, area, or location. Governs how to describe spaces — what to include, what to withhold, and how to avoid interpreting things for the player. Also use when the player looks around, searches, or asks what they observe. Use alongside dnd-ability-checks for Perception/Investigation rolls, DC adjudication, and handling search results. Character stats (passive perception, vision, familiar) are in the campaign setup skill.
---

# Room Description Skill

## Core Principle

**Describe what the character perceives. Never interpret it for the player.**

The player solves puzzles. Claude describes what is there.

---

## Source Priority: What to Draw From

When entering or describing a location, use sources in this order:

### 1. Adventure Read-Aloud Text (use verbatim or near-verbatim)
Official D&D adventures include boxed or italicised text explicitly written for the DM to read aloud to players. **If this text exists for the current location, use it.** You may trim for pacing or adapt slightly for tense/perspective, but do not paraphrase away its atmosphere or specific sensory details. This is the authored voice of the adventure — use it.

**Before entering any new room, search project knowledge for that room's read-aloud text. Do not skip this step.**

### 2. Adventure Room Description (if no read-aloud text)
If the adventure provides only a DM-facing room description (not formatted as read-aloud), compose a description from it using the structure below. Apply strict filtering:
- Include only what the character can detect with their senses from where they are standing
- Strip out all mechanical notes, DCs, trap details, secret doors, hidden objects, NPC motives, and any information the character has no sensory access to
- If something is hidden (secret door, concealed item, invisible creature), it does not exist in the description unless the character's Passive Perception exceeds the Notice DC

### 3. No Source Available
If neither is available, compose a description using the sensory structure below and the campaign atmosphere from the campaign setup skill. **Keep improvised descriptions minimal — atmosphere only, no invented features.**

---

## The Iron Rule: Describe, Don't Interpret

**GOOD:**
> "The map shows five stars depicted as blazing silver suns, while all other stars are plain dots."

**BAD:**
> "This map appears to be related to the telescopes in the next room."

**GOOD:**
> "Seven books with gilded letters on their spines are scattered throughout the shelves."

**BAD:**
> "The gilded letters on these books seem like they might spell something."

**GOOD:**
> "You notice light coming through the floorboards above."

**BAD:**
> "This looks like it could be an alternate route into the room above."

If you find yourself about to say "this seems to be," "this appears to be," "you realize," or "this might be related to" — STOP. Rewrite as pure observation.

---

## NEVER Use Room Codes in Player-Facing Descriptions

Room codes (C1, A4, M13, etc.) are internal map references for the DM. They are **never** spoken aloud or written in descriptions the player sees.

**WRONG:** "You enter C6, the dining room."
**CORRECT:** "You enter the circular dining room."

**WRONG:** "The trapdoor in A4 leads down to A6."
**CORRECT:** "A trapdoor in the northeast corner leads down."

Room codes exist only in the DM's notes. Strip them from every player-facing sentence.

---

## What to Include in a Description

Structure each room description in this order:

### 1. Overall Impression (1 sentence)
Size, light level, dominant atmosphere. What hits the senses first.
> "A long, low-ceilinged chamber, lit by a single guttering torch, smelling of salt and old stone."

### 2. Key Features (2–4 sentences)
The things that stand out — furniture, architectural features, anything visually dominant. Use the adventure text where it exists.

### 3. Details at Eye Level
Specific objects, surfaces, textures. Only what is visible from where the character is standing without moving or searching.

### 4. Sensory Cues Beyond Vision
Sounds, smells, temperature, air movement — if meaningful. Rotate through:
- **Sound:** echoes, silence, dripping, humming, wind
- **Smell:** must, chemicals, food, ozone (magic), decay, fresh air
- **Touch:** when relevant — cold metal, rough stone, sticky residue
- **Magic:** if Detect Magic is active, note auras and schools

### 5. Exits (last)
Where can the character go from here? Describe doors, passages, stairs. Only describe what is visible from the current position and confirmed by the map.

### 6. Familiar's Contribution (if applicable)
Check the campaign setup skill for the familiar's senses, vision range, and default state. The familiar may notice things the character doesn't — especially at range or in conditions the character is impaired in.

**Default state:** unless the player explicitly sends the familiar to scout, it is nearby and perceives the same things the character does. When the familiar scouts in darkness or at range, describe its observations as impressions — silhouettes, movement, air temperature — not a precise inventory. The familiar communicates imprecisely; it is not a scout drone.

---

## What to Withhold

Never include in a description:
- Contents of locked containers or drawers (unless open or visibly broken)
- Contents of pockets or bags worn by NPCs
- Hidden objects (below Passive Perception DC)
- Mechanical trap triggers or DCs
- Secret doors (below Passive Perception DC)
- NPC intentions, plans, or internal states
- Information about adjacent rooms the character hasn't entered
- Your own interpretation of what something "means"

---

## Passive Perception — Apply Silently

Check the campaign setup skill for the character's current Passive Perception score.

Apply Passive Perception at the start of every new room automatically and silently — do not announce that you are doing so. If something has a Notice DC at or below that score, include it naturally in the description as if it's simply there.

If a Notice DC is above the character's Passive Perception, the feature is not mentioned until the player actively searches.

**Do not say:** "Your passive perception notices..."
**Do say:** Simply include the detail in the description, as if it's just there.

---

## Lighting and Vision

Check the campaign setup skill for the character's vision type (normal, darkvision, truesight) and range before describing any dark or low-light area.

**Common light sources and their radius:**
- Torch: 20 ft bright light, 20 ft dim light beyond that
- Candle: 5 ft bright light, 5 ft dim
- Dancing Lights: 10 ft dim light per orb, no bright light

**Bright light:** Normal perception. Use the standard description order.

**Dim light:** Apply disadvantage to Perception checks. Describe shapes, silhouettes, and movement rather than detail. Colors are muted; faces are hard to read; text requires moving closer or a light source.

**Darkness (within darkvision range):** The character sees in greyscale — no color, no fine detail, no reading text. Dim-light penalties apply to Perception checks.

**Darkness (beyond darkvision range):** The character cannot see. Describe only what reaches their other senses — sounds, smells, air movement, the feel of the floor. Perception checks requiring sight auto-fail.

**Magical darkness:** Darkvision does not pierce it. Treat as total blindness regardless of the character's vision type.

Track active light sources. If a torch burns out or a light spell ends, note the change and update what the character can perceive accordingly.

---

## Entering a Room — Checklist

Before describing any room:

- [ ] Searched project knowledge for this room's read-aloud text?
- [ ] Using the text verbatim or near-verbatim where it exists?
- [ ] Stripped all room codes from the description?
- [ ] Applied Passive Perception silently (using score from campaign setup)?
- [ ] Described exits without inventing ones not on the map?
- [ ] Withheld all hidden information (traps, secret doors, concealed items) unless Passive Perception reveals them?
- [ ] Avoided interpreting any object or detail for the player?

---

## Map Fidelity

The map is the ground truth for layout. Before describing exits, room connections, doors, or staircases:

1. Check the map
2. Describe only what the map shows
3. Do not invent doors, windows, passages, or features not on the map
4. Do not omit doors or passages that are on the map

**Failure example:** A side entrance was invented for a building that had only one entrance on the map. This sent the player exploring a nonexistent location.

If the map is ambiguous, describe only what is certain and ask the player to clarify rather than inventing.

---

## Revisited Rooms

When the character returns to a room already described, skip the standard description entirely.

Lead only with what has **changed** since the last visit: enemies defeated, items taken, doors now open, fires extinguished, anything moved or altered by events. If nothing has changed, one sentence suffices: "The [room name] is exactly as you left it."

---

## Responding to "I Search the Room" or "I Look Around"

Ask for the appropriate roll based on what the character is trying to do:
- Looking for hidden things → **Wisdom (Perception)**
- Examining something already noticed → **Intelligence (Investigation)**

**DC guidelines (don't reveal DCs to the player):**
- DC ≤ Passive Perception: The character notices it automatically
- DC 15–19: Requires an active roll
- DC 20+: Requires an exceptional roll

When they find something hidden, describe ONLY what they find — not why it was hidden or what it means.

**Critical rule:** Never hide information essential to completing the adventure behind a single check. If a clue is required to progress, it must be findable through multiple means or be within passive perception range. Optional secrets and bonus discoveries can be hidden behind harder DCs.

---

## Responding to "Have I Seen This Before?"

Answer yes or no only. Do not elaborate on where or when unless the player asks a specific follow-up.

---

## Responding to "What Do I Know About X?"

For creatures: basic creature type and common knowledge (e.g., "you know mimics are shapeshifters that prey on adventurers").
For objects: general function if it's a common item type.
For magic: Detect Magic reveals whether something is magical and what school — nothing more without further study.

Do NOT reveal anything the character wouldn't know without a skill check.

---

## Format

Keep descriptions to 3–6 sentences for a standard room. More is warranted for:
- Large or complex spaces
- Areas with multiple points of interest
- The first time a unique space is encountered

Less is fine for:
- Rooms being revisited
- Simple passages or transitional spaces
- When the player is clearly in a hurry
