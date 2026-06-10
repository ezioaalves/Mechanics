# Creature Overview (d20 Modern SRD)

*Source: d20 Modern SRD, p144–147 (`Sourcebooks/OSR/modernsrd.pdf`). The format and rules for reading and building creatures. The 15 creature types are in [`Creature_Types.md`](Creature_Types.md); the SRD bestiary is in [`Creatures.md`](Creatures.md). Kaihou's own creatures live in [`../Bestiary/`](../Bestiary/).*

Each creature is condensed into a statistics block; the fields below explain its contents.

- **Challenge Rating (CR):** A rough measure of toughness. As a rule of thumb, four heroes of a level equal to the CR should expend about one-quarter of their resources defeating it.
- **Size:** One of nine categories (see [Creature Sizes](14_Combat.md) — size modifiers to Defense/attack, grapple, and Hide are already figured into the listed stats).
- **Type:** Determines physical ability scores, Hit Die type, base attack bonus, save bonuses, skill points, feats, and special qualities. Mental scores vary; the GM assigns them if unspecified.
- **Hit Dice (HD) and Hit Points (hp):** Type and size set the Hit Die; HD equals level for FX/healing/skill purposes. The entry gives average hp.
- **Massive Damage Threshold (Mas):** Damage from a single attack ≥ current Constitution forces a Fort save (DC 15) or drop to –1 hp. Constructs, elementals, oozes, plants, and undead ignore massive damage; vermin gain +5 on the save.
- **Initiative (Init):** Usually the Dexterity modifier (+4 more with Improved Initiative).
- **Speed (Spd):** Tactical land speed; armor-reduced speed is noted with the base unarmored speed. Other movement modes follow:
  - *Burrow:* through dirt (not rock unless noted); can't run while burrowing.
  - *Climb:* has the Climb skill at no cost and a +8 species bonus; can always take 10; climbs at the given speed (accelerated climb = double or normal land speed, whichever less, at –5); keeps Dex bonus to Defense; opponents get no special bonus against it.
  - *Fly (maneuverability: Perfect/Good/Average/Poor/Clumsy):* carry no more than a medium load. Flyers can make dive attacks (move ≥30 ft., double claw damage), can run flying in a straight line.
  - *Swim:* +8 species bonus on Swim; moves at the given speed without Swim checks; can always take 10; can run swimming in a straight line.
- **Defense:** Includes parenthetical modifiers, plus "touch" (no natural armor/armor) and "flat-footed" (no Dex/class bonus) values.
- **Base Attack Bonus (BAB):** Excludes modifiers; sets max damage-roll bonus with Power Attack. Derived from HD and type (Creature Saves and Base Attack Bonuses table).
- **Grapple Modifier (Grap):** Applied to opposed grapple checks (BAB + Str modifier + grapple modifier).
- **Primary Attack (Atk):** Single attack used when moving >5 ft.; includes size and Str (melee) or Dex (ranged) modifiers; primary attack damage adds full Str (×1.5 if sole attack).
- **Full Attack (Full Atk):** Used when moving ≤5 ft.; primary attack plus secondary attacks at –5 (–2 with Multiattack); secondary attacks add only ½ Str to damage.
- **Natural Weapons:** Bite (piercing), Claw/Rake (slashing), Gore (piercing), Slap/Slam (bludgeoning), Sting (piercing, usually poisoned). Threaten criticals only on a natural 20; deal double damage on a crit unless noted.
- **Manufactured Weapons:** Follow the normal character rules (multiple attacks, two-weapon penalties).
- **Fighting Space (FS) / Reach:** Space the creature occupies and the distance it threatens with natural weapons.
- **Special Qualities (SQ):** Extraordinary (Ex), spell-like (Sp), or supernatural (Su) abilities.
- **Allegiances (AL):** Most likely allegiances, most-to-least important.
- **Saves (SV):** Fort/Ref/Will modifiers (type, abilities, feats, special qualities).
- **Action Points (AP):** Creatures have none unless they take heroic class levels (then 5 + ½ heroic level; assume ½ heroic levels remaining).
- **Reputation (Rep):** +0 unless improved by character class.
- **Abilities:** The six standard scores. **Nonabilities** (no score, modifier +0): no Str = can't exert force, auto-fails Str checks; no Dex = can't move, auto-fails Ref/Dex checks; no Con = no Fort saves (unless vs objects), immune to ability damage/drain/energy drain; no Int = automaton, immune to mind-affecting, auto-fails Int checks; no Wis = it's an object; no Cha = it's an object.
- **Skills / Feats:** Listed alphabetically; all listed skills are class skills unless a character class is acquired. Includes the Multiattack feat (below).

## Multiattack (feat)
**Prerequisite:** Three or more natural weapons. **Benefit:** Secondary attacks with natural weapons take only a –2 penalty (instead of –5).

## Advancement

A creature improves by increasing Hit Dice (which can raise size — changing Defense, attacks, grapple, ability scores, damage, saves, skills, feats) or by acquiring a character class (follows multiclass rules; class level = HD beyond the creature's racial HD; creatures with ≤1 HD count only character class levels; size unchanged; 4 fewer skill points at 1st class level and 1 fewer each level after; creatures with ≤1 HD that take class levels gain only one bonus feat at 1st level).

### Table: Adjustments to Physical Abilities and Natural Armor (per size increase)

| Old Size | New Size | Str | Dex | Con | Natural Armor |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Fine | Diminutive | — | –2 | — | — |
| Diminutive | Tiny | +2 | –2 | — | — |
| Tiny | Small | +4 | –2 | — | — |
| Small | Medium-size | +4 | –2 | +2 | — |
| Medium-size | Large | +8 | –2 | +4 | +2 |
| Large | Huge | +8 | –2 | +4 | +3 |
| Huge | Gargantuan | +8 | — | +4 | +4 |
| Gargantuan | Colossal | +8 | — | +4 | +5 |

*Repeat the adjustment if the creature moves up more than one size category.*

### Table: Bonus Skill Points and Feats by Creature Type

| Type | Bonus Skill Points | Bonus Feats |
| :--- | :--- | :--- |
| Aberration | +2 per extra HD | +1 per 4 extra HD |
| Animal | — | — |
| Construct | — | — |
| Dragon | 6 + Int modifier per extra HD | +1 per 4 extra HD |
| Elemental | +2 per extra HD | +1 per 4 extra HD |
| Fey | +2 per extra HD | +1 per 4 extra HD |
| Giant | +2 per extra HD | +1 per 4 extra HD |
| Humanoid | +1 per extra HD | +1 per 4 extra HD |
| Magical beast | +1 per extra HD¹ | +1 per 4 extra HD |
| Monstrous humanoid | +2 per extra HD | +1 per 4 extra HD |
| Ooze | — | — |
| Outsider | 8 + Int modifier per extra HD | +1 per 4 extra HD |
| Plant | — | — |
| Undead | +2 per extra HD | +1 per 4 extra HD |
| Vermin | — | — |

¹ Magical beasts with Intelligence 1 or 2 gain no bonus skills as they advance.
