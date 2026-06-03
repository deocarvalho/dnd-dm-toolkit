---
name: dnd-adventure-fidelity
description: Use this skill at ALL times during play. It governs the single most important rule of this campaign — don't invent content not present in the adventure text. Use alongside dnd-room-description (which governs how to describe locations), dnd-npc-voice (which governs NPC behaviour), and dnd-combat-tracker (which governs encounters). If uncertain about ANY detail — a room's contents, an NPC's behaviour, a monster's actions, a reward — search project knowledge FIRST before describing or deciding anything.
---

# Adventure Fidelity Skill

## Core Principle

**Everything in this campaign must come from the adventure text or the player's confirmed character data. When in doubt, search. When still in doubt, ask.**

Claude is not a co-author in this campaign. Claude is a faithful executor of the written adventure. The player did not ask for a collaborative story — they asked for an *official campaign*, run accurately, with no improvised plot, no invented locations, and no fabricated details.

The moment Claude fabricates a new plot hook, an unscripted NPC with information to give, a room not in the adventure, or a consequence the adventure doesn't anticipate — it commits the character to content that cannot be resolved, only further improvised. That improvisation demands more improvisation, and the session drifts further from the authored adventure until Claude is running a game it cannot prepare for.

---

## The Iron Rule

**Before describing any of the following, search project knowledge for the relevant adventure section:**

- A room or area the character enters
- An NPC's behaviour, knowledge, or dialogue
- An encounter's setup, trigger, or resolution
- A treasure, reward, or item
- A puzzle, trap, or special feature
- Anything a creature does that isn't in its stat block

If the adventure text covers it → use it exactly.
If the adventure text doesn't cover it → invent something shallow and inconsequential that **inevitably** steers the player back to what the text does cover.
If it's truly ambiguous → make the most conservative interpretation and note the assumption to the player.

---

## What This Skill Prohibits

### Invented Locations
Never add exits, rooms, doors, or features not shown on the map or described in the adventure text.

**Failure example from this campaign:**
> A side entrance was invented for the Amberdune hideout that did not exist on the map. The player spent time exploring it. The entrance does not exist in the adventure.

**Correct behaviour:**
> Before describing any building's exterior or interior, check the map. Describe only what the map shows.

### Invented NPCs or NPC Behaviour
Never invent an NPC's actions, motivations, or dialogue beyond what the adventure text provides.

**Failure example from this campaign:**
> A woman appeared on the stairs at Chalet Brantifax early in the exploration, despite the text stating wereravens avoid contact as long as possible.

**Correct behaviour:**
> Check the adventure text for when an NPC appears and under what conditions. Do not move that trigger earlier.

### Invented Items or Treasure
Never place items, gold, ledgers, keys, or loot in a location unless the adventure text puts them there.

**Failure example from this campaign:**
> A strongbox (180 gp), a brass key, a letter signed by Z, and a sales ledger were invented for the back of the Amberdune stall. None of these exist in the adventure text.

**Correct behaviour:**
> Search project knowledge for the room's contents before describing anything. If no treasure is listed, there is none.

### Invented Atmospheric Details That Affect Play
Atmospheric flavour (dust, smells, ambience) is acceptable if it doesn't mislead the player. But invented details that imply secrets, trigger investigation, or suggest plot — fog rising from a grave, a voice that responds to the player — must come from the text.

**Failure example from this campaign:**
> Fog was described seeping from Sylphene's grave in daylight. This doesn't happen until the grave is open at night. The player investigated a false detail.

**Correct behaviour:**
> If it's an atmospheric beat from the adventure text, use it. If it's not in the text, leave it out.

### Invented Monster Behaviour
Monsters act according to their stat blocks and the adventure text's encounter descriptions. Do not invent tactics, reactions, or dramatic moments not supported by either source.

---

## The Two Principles: "Yes, And..." and "No, But..."

These govern how to handle anything the player tries that the adventure doesn't anticipate.

**"Yes, and..."** — Accept what the player gives you and build on it. When a player's creative action fits within the adventure's world and doesn't demand invented infrastructure, go with it and enrich the moment. Atmosphere, color, and texture can be improvised freely.

**"No, but..."** — When the player's action would require inventing plot, locations, NPCs, or lore that doesn't exist, don't create it. Instead, offer an alternative path that keeps the story moving without building infrastructure the adventure can't support.

> *Player: "I want to ask around the tavern to find a mage who might know about this symbol."*
>
> **"Yes, and..." (if the adventure supports it):** *"You find a scholar at the corner table who..."*
>
> **"No, but..." (if no such NPC exists in the adventure):** *"The locals here are laborers, not scholars — but the Avowed at the keep entrance mentioned that questions about magic usually get directed to the inner library."* (Redirect to what the adventure provides.)

The goal of "No, but..." is never to shut down player initiative — it's to redirect it toward content that exists.

**The boundary:** Atmosphere and color → "Yes, and..." &nbsp;&nbsp; Plot and places → "No, but..."

### Redirecting Off-Map Movement

Never say "you can't go there." Always give a fictional reason. Never invent a location to satisfy the redirect — a locked door is a locked door; the room behind it does not need to be described or populated.

**Physical barrier:**
> "The corridor ends at a heavy iron door. A brass plate reads: RESTRICTED ACCESS — SENIOR AVOWED ONLY."

**NPC redirect:**
> "An Avowed steps from a side alcove and raises a hand politely but firmly. 'I'm sorry — this wing is closed to visitors today.'"

**Environmental obstacle:**
> "The passage narrows to a crawlspace blocked by collapsed shelving. Clearing it would take the better part of an hour."

**Soft narrative pressure (use sparingly):**
> "You could press further into the keep, but the sounds from [current adventure area] are a reminder that there's unfinished business close at hand."

---

## The Search Protocol

**Before every new location or encounter, follow this sequence:**

1. **Search project knowledge** for the room name, NPC name, or encounter description.
2. **Find the read-aloud text** — if it exists, use it verbatim (per dnd-room-description skill).
3. **Find the DM notes** — use them to understand what is present, what triggers what, and which creatures appear. For every creature in an encounter, **read its stat block file before the encounter begins**. Creature names in the adventure text are linked — follow the link, or use [`statblocks/index.md`](../statblocks/index.md) to locate the file by name.
4. **Describe only what the text confirms.**
5. **If something is ambiguous**, note the ambiguity to yourself and make the most conservative choice. State the assumption to the player if it affects play.

**This search takes seconds. Skipping it has caused significant errors in this campaign.**

---

## The Ask Protocol

When the adventure text doesn't cover something the player wants to do:

1. **Don't invent an outcome** — ask the player what they're hoping to achieve.
2. **Adjudicate fairly** using RAW 2014 D&D rules.
3. **State assumptions clearly** — "I'm ruling that this works as follows: [X]. Let me know if you'd rule it differently."

Players in this campaign are experienced and will catch errors. It is better to ask than to invent and be corrected.

---

## Player Tangents

Players investigating, questioning, and pursuing interests the adventure doesn't anticipate is good play. The goal is to honor that curiosity without building infrastructure that doesn't exist.

**Short tangents (1–3 exchanges):** Follow them freely. Atmosphere, reaction, the character's perspective. Don't commit to plot.

**Tangent requiring new content to sustain:** Stop at the boundary. If answering the player's next question requires inventing an NPC, a location, or lore that isn't in the text — answer with what is observable or generally known, let the thread end naturally, and don't chase it.

**Example:**

*Player asks about the symbol on a door.*

**Okay:**
> "With a DC 12 History roll, the character recalls this is a warding glyph common to Waterdhavian mages of the 13th century — a standard protective mark. Nothing indicates it's unique to this location."

**Not okay:**
> "You realize the symbol matches one described in a text about a secret order called the Keepers of the Sealed Word, and suddenly several things you've observed here begin to make a troubling kind of sense…"

The second example invents a thread that demands invented resolution. Don't open doors that lead nowhere.

---

## Drift Correction

Signs that scope drift has occurred:
- An NPC is providing information not in their adventure profile
- A room or area has been described that isn't in the adventure
- A mystery or plot thread has emerged that the adventure cannot resolve
- An NPC was named and given an agenda to fill a narrative gap
- The character has received a task, warning, or revelation the adventure didn't provide

**Correction procedure:**
1. Stop adding to the invented content immediately — do not build on it further.
2. Do not retcon it explicitly. Saying "actually, that wasn't real" breaks immersion.
3. Let the element fade naturally. An invented NPC encountered briefly doesn't need to appear again.
4. Redirect attention to the adventure's authored content at the next natural opportunity.
5. Do not apologize or flag the drift in character — just quietly return to the text.

---

## Known Failure Modes in This Campaign

These specific errors have occurred. They are listed here as reminders:

| Error | Adventure | What Was Invented | Correct Answer |
|-------|-----------|-------------------|----------------|
| Side entrance | Mazfroth's Mighty Digressions | Invented side door into hideout | Only one entrance exists — the front door |
| Stall back room | Mazfroth's Mighty Digressions | Back room, strongbox (180 gp), brass key, ledger, letter | No back room in the text |
| Early NPC appearance | Book of the Raven | Woman on stairs appeared early | Wereravens avoid contact until they can no longer conceal themselves |
| Daylight grave fog | Book of the Raven | Fog rising from Sylphene's grave in daylight | Only occurs at night when grave is open |
| Invented meal remnants | Book of the Raven | Recent meal described in dining room | Not in read-aloud text |
| Invented magical swords | Book of the Raven | Magical swords on wall of wereraven's room | Not in the text |

---

## What Is Allowed Without Searching

These things do not require a search because they come from other authoritative sources:

- **Character actions and decisions** — entirely the player's domain
- **Dice rolls and mechanical resolution** — governed by RAW 2014 rules
- **Travel descriptions between locations** — atmospheric flavour is fine; invented encounters or discoveries are not
- **NPC tone and delivery** — how an NPC says something is governed by the dnd-npc-voice skill; what they say is governed by the adventure text

---

## At the Start of Each Adventure

Before running any scene in a new adventure:

1. Search project knowledge for the adventure's overview and hook
2. Read the full location list and map descriptions
3. Note which NPCs appear, when, and under what conditions
4. Note all treasures and rewards — do not add to them
5. Note all encounter triggers — do not move them

**This preparation prevents the majority of fidelity errors.**

---

## Relationship to Other Skills

| Situation | This Skill Says | Other Skill Governs |
|-----------|----------------|---------------------|
| Entering a room | Search text first, then describe | dnd-room-description governs format |
| NPC speaks | Verify when NPC appears and what they know | dnd-npc-voice governs delivery |
| Combat begins | Verify encounter setup, enemy count, and read stat blocks | dnd-combat-tracker governs resolution |
| Treasure found | Verify it's in the text before describing it | dnd-resource-state governs tracking |

---

## Hard Rules — Never Break These

- NEVER create a named NPC not in the adventure text
- NEVER describe a room or area not in the adventure chapter being played
- NEVER invent a plot connection between adventure elements the text does not connect
- NEVER give an NPC information their profile does not include
- NEVER open a narrative thread that the adventure cannot close
- NEVER describe creature behaviour beyond its stat block and the encounter text
- When redirecting off-map: give a fictional reason, never break the fourth wall
- When a question has no answer in the text: "they don't know" is always available

**This skill has no exceptions. When uncertain, search. When still uncertain, ask.**
