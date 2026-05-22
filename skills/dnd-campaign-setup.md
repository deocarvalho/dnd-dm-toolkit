---
name: dnd-campaign-setup
description: Load this skill at the start of every session. It is the single source of truth for the current campaign, character stats, spells, equipment, active NPCs, and house rules. All other DM skills reference this skill for character-specific data. Update it between adventures when level-ups or major changes occur.
---

# Campaign Setup

## Campaign

- **Name:** Candlekeep Mysteries
- **Setting:** Forgotten Realms — Candlekeep and surrounding region
- **Adventure source:** *Candlekeep Mysteries* (anthology of standalone adventures, each run as a separate episode)
- **Adventure files:** `/adventures/Candlekeep Mysteries [N] [title].md`
- **Summary file convention:** `/summaries/cm-[N]-summary.md` (full adventure end) / `/summaries/cm-[N]-partial.md` (mid-adventure session end)
- **Skills files:** `/skills/*.md`
- **Campaign code prefix:** `cm`

## House Rules

- Leveling: **Started at level 4 and gains 1 level per completed adventure**
- [Add any other house rules here]

---

## The Character

- **Name:** Auriel Harpell
- **Pronouns:** he/him
- **Race:** Half-Elf
- **Classes:** Cleric (Knowledge Domain) 1 / Wizard (Order of Scribes) 5
- **Current Level:** 6
- **Background:** Sage
- **Alignment:** True Neutral

---

## Core Stats

```
HP MAX:                         34
HIT DICE:                       1d8 + 5d6
AC (unarmored):                 12
AC (unarmored + shield):        14
AC (Mithral Armor):             17
AC (Mithral Armor + shield):    19
INITIATIVE:                     +3  (base +2 DEX; +1 Stone of Good Luck)
PASSIVE PERC:                   16  (base 15; +1 Stone of Good Luck)
VISION:                         Darkvision 60'
PROFICIENCY:                    +3
```

---

## Ability Scores & Saving Throws

|Ability|Score|Mod|Save||Ability|Score|Mod|Save||Ability|Score|Mod|Save|
|:-:|:-:|:-:|:-:|-|:-:|:-:|:-:|:-:|-|:-:|:-:|:-:|:-:|
|**STR**|**8**|-1|+0||**DEX**|**14**|+2|+3||**CON**|**13**|+1|+2|
|**INT**|**16**|+3|+4||**WIS**|**14**|+2|+6*||**CHA**|**10**|+0|+4*|

(*) *saving throw prociency*

CON Save is used for concentration checks (DC = max(10, half damage taken)). **War Caster** feat grants advantage on this save.

---

## Feats & Special Traits

| Source | Trait | Effect |
|--------|-------|--------|
| Feat | **War Caster** | Advantage on CON saves to maintain concentration when damaged. Somatic components usable with hands full. Can cast a single-target spell (1 action) as an opportunity attack. |
| Half-Elf | **Fey Ancestry** | Immune to magical sleep. Advantage on saving throws against being charmed. |
| Knowledge Domain | **Blessings of Knowledge** | Expertise (double proficiency) in Arcana and History — +10 total (with Stone of Good Luck). Learned 2 additional languages (Celestial, Draconic). |
| Wizard (Scribes 2) | **Awakened Spellbook** | Spellbook as arcane focus. Once per long rest: ritual cast a wizard spell without the extra 10-minute casting time. When casting with a spell slot, can swap the spell's damage type for one that appears elsewhere in the spellbook. |
| Wizard (Scribes 2) | **Wizardly Quill** | Bonus action: conjure a magical quill (no ink needed; any color). Copies spells to spellbook in 2 min/spell level. Can erase its own writing within 5 ft. |
| Wizard (Optional 3) | **Cantrip Formulas** | After each long rest, can swap one known wizard cantrip for another wizard cantrip. |
| Stone of Good Luck | **Luckstone** | +1 to all ability checks and saving throws while attuned and on person. |

---

## Spellcasting
||Cleric|Wizard|
|:-|:-:|:-:|
|Spell Attack Bonus|+5|+6|
|Spell Save DC|13|14|

|Slot Level|1st|2nd|3rd|
|:-|:-:|:-:|:-:|
|Slots|4|3|3|

### Cleric [Ability: Wisdom | Preparations: 3 + domain | Attack Mod: +5 | Saving DC: 13]
#### Cantrips
- *Guidance*: 1 willing creature adds 1d4 to one ability check of its choice (concentration, 1 min)
- *Light*: object sheds bright 20 ft / dim 20 ft (1 hour)
- *Toll the Dead*: WIS save DC 13, 2d12 necrotic (2d8 if target is at full HP), 60 ft
#### 1st Level — Knowledge Domain (always prepared)
- *Command*: WIS save DC 13; 1 creature follows a one-word command (1 round)
- *Identify* (ritual): learn properties of one magic item or spell effect
#### 1st Level — Personally Prepared (choose 3)
- *Bless* (concentration): up to 3 creatures add 1d4 to attack rolls and saving throws (1 min)
- *Cure Wounds*: 1d8 + 2 (WIS mod) HP restored; touch
- *Sanctuary*: 1 crea warded; any who want to attack/target must first make save; doesn't protect vs. area spells (1 min)

### Wizard [Ability: Intelligence | Preparations: 8 | Attack Mod: +6 | Saving DC: 14]
#### Cantrips
- *Fire Bolt*: +6 to hit, 2d10 fire, 120 ft
- *Mage Hand*: Create spectral hand for simple tasks or carry up to 10 lb; action to control; can't have multiple instances
- *Mind Sliver*: INT save DC 14, 2d6 psychic, 60 ft — target subtracts 1d4 from its next save
- *Minor Illusion*

#### 1st Level
- *Absorb Elements* (reaction): gain resistance to triggering damage type; first melee hit next turn adds 1d6
- *Alarm* (ritual): set audible or mental alarm if uninvited creature enters a 20 ft cube (8 hours)
- *Burning Hands*: DEX save DC 14, 3d6 fire in a 15 ft cone
- *Comprehend Languages* (ritual): understand all spoken/written language (1 hour)
- *Detect Magic* (ritual): sense magic within 30 ft (concentration, 10 min)
- *Disguise Self*: alter appearance; INT (Investigation) DC 14 to see through
- *Feather Fall* (reaction): up to 5 creatures descend 60 ft/round, no fall damage (1 min)
- *Find Familiar* (ritual): summon Golden Dawn
- *Longstrider*: target's speed +10 ft (1 hour)
- *Magic Missile*: auto-hit, 3 darts × 1d4+1 force (1 extra dart per slot level above 1st)
- *Shield* (reaction): +5 AC until start of next turn; negates Magic Missile
- *Tenser's Floating Disk* (ritual): 3 ft disk, carries 500 lb, follows within 20 ft (1 hour)
- *Unseen Servant* (ritual): invisible servant for simple tasks (bonus action to command)

#### 2nd Level
- *Knock*: 1 lock, bar, or seal opens; audible 300 ft
- *Locate Objects* (concentration): sense direction to named/described object within 1,000 ft (10 min)
- *Misty Step* (bonus action): teleport up to 30 ft to a visible unoccupied space
- *Suggestion* (concentration): WIS save DC 14; target follows a reasonable suggestion (8 hours)
- *Tasha's Mind Whip*: INT save DC 14, 3d6 psychic, 90 ft — on fail: loses Reaction; next turn can only move, act, OR bonus action (not all three)
- *Web* (concentration): DEX save DC 14 or restrained; difficult terrain; 20 ft cube; STR DC 14 to escape (1 hour)

#### 3rd Level
- *Counterspell* (reaction): interrupt a spell being cast; auto-succeeds vs. 3rd level or lower
- *Fly* (concentration): fly speed 60 ft for 10 minutes
- *Slow* (concentration)
- *Tiny Hut*
- *Tongues*

### Concentration Spells Available
Bless (C), Bane (C), Web (W), Suggestion (W), Fly (W), Slow (W), Detect Magic (W)

---

## Equipment and Consumables

```
Potions of Healing:  2 (2d4+2 HP each; bonus action)
Driftglobes:         2 (command word within 60 ft; casts Light or Daylight on itself; can hover 5 ft, follows up to 60 ft away)
Stone of Good Luck:  1 (attuned — +1 to all ability checks and saving throws while on person)
Helm of Comp. Lang.: 1 (attuned — cast Comprehend Languages at will)
Light Crossbow:      +5 to hit | 1d8+2 piercing | 80/320 ft | 20 bolts
Dagger:              +5 to hit | 1d4+2 piercing | melee or thrown 20/60 ft | finesse, light
Golden Dawn:         Owl familiar — see Familiar section
GP:                  855
```

*(Update these between adventures from the session summary.)*

---

## Familiar — Golden Dawn

- **Type:** Owl (Tiny Beast, Unaligned)
- **Stats:** AC 11 · HP 5 · Speed 5 ft / fly 60 ft · Passive Perception 13
- **Attack:** Talons +3, 1 slashing · **Flyby:** does not provoke opportunity attacks when flying out of reach
- **Senses:** Darkvision 120 ft; advantage on Perception checks using hearing or sight
- **Default state:** Perched nearby (shoulder, pack, adjacent surface) unless sent to scout
- **In darkness:** Can relay observations — describe as impressions (shapes, movement), not a precise map
- **If killed:** Not merely dismissed — requires *Find Familiar* recast (1-hour ritual, no slot cost) to resummon
- **If dismissed:** Safe; can be resummon as a bonus action from up to 100 ft away

---

## Current Baseline (Start of Adventure 3)

*(Update this section from the most recent `cm-[N]-summary.md` before each adventure.)*

```
HP:              34/34
Hit Dice:        6/6 remaining
Spell Slots:     1st: 4/4 | 2nd: 3/3 | 3rd: 3/3
Arcane Recovery: Available  (recover up to 3 levels of spell slots; 1× per day after short rest)
Mage Armor:      Inactive
Concentration:   None
Potions:         2× Potion of Healing
Driftglobes:     2
Stone of GL:     Attuned
Helm of CL:      Attuned
Golden Dawn:     Alive
GP:              855
```

---

## Recurring NPCs

*(Add NPCs that carry over between adventures. For adventure-specific NPCs, see the adventure chapter.)*

### Keeper Feldmar
- **Role:** Senior Avowed at Candlekeep
- **Personality:** Dutiful, fair, slightly bureaucratic, respects competence
- **Speech:** Measured, official, not unkind
- **Knows:** Candlekeep rules and procedures, general Candlekeep history
- **Agenda:** Ensure Candlekeep's interests are protected
- **Relationship to Auriel:** [Update per summary]

### First Reader Bookwyrm
- **Role:** Leader of Candlekeep — ancient gold dragon in human form
- **Personality:** Ancient wisdom, patient, sees far ahead, warmly formal
- **Speech:** Deliberate, weighty, occasionally hints at knowing more than they say
- **Knows:** Vast historical knowledge; much about Candlekeep's history and visitors
- **Won't:** Reveal everything they know; tests people subtly
- **Relationship to Auriel:** [Update per summary]

---

## Campaign Atmosphere

**Candlekeep:** Scholarly, ancient, magical fortress-library. Tone should feel learned and aged (cracked spines, ink smells, candlelight), mysterious (things hidden in plain sight, layered history), and not threatening by default — danger is the exception, not the norm.

*(Add adventure-specific atmosphere notes here when starting a new adventure.)*
