# Location Schema (Kanigakure)

This file replaces the old 7-section template (Identity / Actions / Statistics / NPCs / Secrets / Events / Inventory) used in `Lore/World_of_Rokugan/Kanigakure/`. Every location card in the Training Arc and beyond should follow this schema.

The schema is **role-typed**: a location declares one Primary Role and at most one Secondary Role. Sections that aren't relevant to a location's roles are omitted — a forge does not need an Influence DC table; a tavern does not need a crafting bonus.

## Roles

| Role | Exposes | Plugs into |
| --- | --- | --- |
| **Training Venue** | Learn check modifiers, environment, equipment | [[11_Learn DC]] |
| **Sensei Hub** | Named sensei NPCs with tier tracks | [[Sensei_Relationships]] |
| **Mission Board** | D-rank and C-rank pools, refresh cadence | [[Missions_and_Bounties]] |
| **Market** | Purchase DC ceiling, restricted catalog | Wealth / Purchase DCs |
| **Social Venue** | Influence DCs, Discovery skills, recurring NPCs | [[Influência]] |
| **Hazard / Exploration** | Random encounter table, risk/reward | GM table |

A location may be a single role (Yato's Weapons → Market) or hybrid (Shinobi Academy → Training Venue + Sensei Hub). Avoid >2 roles per card; if a location truly does more, split it into sub-locations.

## Card Template

```markdown
# [Location Name]
> District • Primary Role • Secondary Role • Access tier

## Hooks
One paragraph. Why does a genin walk in. What do they walk out with. Tone in one sentence.

## Action Menu
| Action | Cost (blocks) | Roll | DC | Output | Cooldown |
| --- | --- | --- | --- | --- | --- |
| ... | ... | ... | ... | ... | ... |

(Every action's cost MUST appear in `Action_Blocks.md`'s canonical table.
Every Output MUST hook one of: Learn check, Influence check, Discovery check, Mission resolution, Purchase, Craft, lore reveal, Sensei tier progress.)

## NPCs   ← only if Sensei Hub or Social Venue
For each named NPC use the stub from `Sensei_Relationships.md` (Sensei Hub) or the abbreviated form (Social Venue):

  Name • Role • Discipline / Specialty
  Influence skills: primary / secondary
  Influence DC: typical / difficult (APL-scaled)
  Discovery skills: ...
  Strengths / Weaknesses (revealed by Discovery)
  Hooks / agenda

## Inventory   ← only if Market
| Item | Purchase DC | Restriction | Stock state |
| --- | --- | --- | --- |

Reputation gates: e.g. "Aware tier with Yato raises ceiling to PDC 22."

## Mission Pool   ← only if Mission Board
D-rank list:
| Mission | Roll | DC | Pay class | Block cost | Chakra | Failure consequence |
C-rank list:
| Mission | Travel days | Pay class | Hook | Escalation |

Refresh: weekly (default) or per arc phase.

## Monthly State
Reference the [[Arc State Overlay]] for global changes. Add only location-specific deltas here:
- Ox: ...
- Tiger: ...
- Hare (post-Breach): ...
- Dragon: ...
- Serpent: ...

## Random Events (optional)
d6 or d10 table, scaled to current arc phase. Use only if the location is supposed to surprise.
```

## Rules of Engagement

1. **No invented action costs.** If an action doesn't fit the canonical table in `Action_Blocks.md`, redesign it — don't ship a one-off cost.
2. **Bonuses must declare their bucket.** A Learn-bonus action says whether it's Tutoring, Self-Teaching, or Situational (per [[11_Learn DC]]). Two Situational bonuses from the same location don't stack with each other; they pick the highest.
3. **Every Sensei is named.** No "rotating pool." If a sensei isn't worth naming, they aren't worth showing on the card.
4. **Influence checks resolve per check, not per phase.** A 1-block visit = 1 Influence attempt, per the campaign's house ruling. Track NPC tier progress cumulatively across days.
5. **Mission entries are concrete.** Title, roll, DC, pay class, block cost, chakra, failure consequence. No "missions can happen here."
6. **Markets declare the ceiling, not the floor.** Players know nothing's too cheap to buy; what matters is the highest Purchase DC currently available, and the gate to unlock it.
7. **Monthly state isn't decorative.** If a line doesn't change a number, an NPC, an item, or a DC — delete it.

## What to Drop From the Old Template

| Old section | Where its content goes now |
| --- | --- |
| Identity | Compressed into the header + Hooks. |
| Actions | Stays, but only with the canonical block costs. |
| Statistics | **Deleted.** Bonuses inline with their actions; risks inline with their actions. |
| NPCs | Stays, but only named NPCs with influence wiring. |
| Secrets | Folded into Hooks / Monthly State; secret unlocks live in Mission Pool failure/success branches. |
| Events | **Deleted** as a section; Random Events table covers the dice-driven ones, Monthly State covers the scheduled ones. |
| Inventory | Stays, but as the Purchase DC table. |

## Examples (to be written in Step 2 of the rollout)

- `Shinobi Academy` — Training Venue + Sensei Hub
- `Shushu-ya` — Social Venue + Market (restricted catalog)
- `Yato's Weapons` — Market + Training Venue (crafting / weapon Learn bonuses)

## Linked

- [[Action_Blocks]] — canonical action costs.
- [[Sensei_Relationships]] — Sensei Hub mechanics.
- [[11_Learn DC]] — training math.
- [[Influência]] — Influence and Discovery checks.
- [[Missions_and_Bounties]] — D/C-rank reward and warning system.
