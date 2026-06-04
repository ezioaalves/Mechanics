# Mechanics Registry: Naruto - Rokugan Rising

The engine of the Iron Shell. These rules define the tactical depth of our shinobi world.

---

## 📜 Core Rules
The foundational mechanics of the Naruto d20 system.

*   **[Basic Game Mechanics](Basic_Rules/Basic%20Game%20Mechanics.md)**
*   **[Ninja Ranks](Basic_Rules/Ninja_Ranks.md)**
*   **[Character Creation Guide](Basic_Rules/01_-_Character_Creation_Guide.md)**
*   **[Combat & Actions](Basic_Rules/Combat.md)** ([Actions Index](Basic_Rules/Actions.md))
*   **[Chakra & Energy](Basic_Rules/Chakra.md)** ([Chakra Gifts](Basic_Rules/Chakra%20Gifts.md) | [Energy Damage](Basic_Rules/Energy%20Damage.md))
*   **[Special Shinobi Features](Basic_Rules/Special%20Shinobi%20Features/Special%20Shinobi%20Features.md)**
*   **[Power Scaling: Strength & Speed Ranks](Basic_Rules/St%20Sp%20Ranks/Ranks.md)**
*   **[Skill Conversion Table](House_Rules/Skill%20-%20Conversion.md)** (d20 Modern to Pathfinder/Kaihou)
*   **[d20 Modern Base Rules](D20_Modern/Registry.md)** — the unmodified SRD foundation; Kaihou rules override where they overlap.

---

## 🛠️ Active House Rules
Custom modifications and high-power variants currently active in the campaign.

*   **[Feat Overhaul (Elephant in the Room)](Feat%20Overhaul%20(EITR).md)**
*   **[Power Units (PU)](Power%20Units.md)**
*   **[Bloodline Progression](Bloodline%20Progression.md)**
*   **[Empathic Learning](Empathic%20Learning.md)**
*   **[Solo Creatures (Boss Rules)](Solo%20Creatures.md)**
*   **[Mastercraft Upgrades](Mastercraft.md)**
*   **[Class Feature Scaling](Feature%20Progression.md)**

---

## 🏕️ Downtime & Activities
Rules for resting, training, and bonding between missions.

*   **[Conversas de Fogueira](Downtime/Conversas%20de%20Fogueira/)**
*   **[Desenvolvimento de Jutsu](Downtime/Desenvolvimento%20de%20Jutsu/)**

---

## 🧬 Character Options
Bloodlines, Classes, and customization.

*   **[Village Perks](Character_Options/Villages/)** - Minor mechanical benefits by origin.
*   **[Basic Ninja Classes](Character_Options/Classes/Basic/)** - The 6 foundational archetypes.
*   **[Prestige Classes](Character_Options/Classes/Prestige/)** - Advanced paths and specialization.
*   **[Bloodline Database](Character_Options/Bloodlines/Bloodlines.md)** - Clan hijutsu and heritage.
*   **[Skills Index](Character_Options/Skills/)** - Individual skill rules and **[Tactics](Character_Options/Skills/Tactics/)**.
*   **[Races](Character_Options/Races/)** - System-level/NPC races.

---

## 🌀 Techniques (Jutsu)
Master the elements and the mind.

*   **[Jutsu Database](Techniques/all_jutsus.md)**
*   **[Ninjutsu](Techniques/Ninjutsu/)**
*   **[Genjutsu](Techniques/Genjutsu/)**
*   **[Taijutsu](Techniques/Taijutsu/)**
*   **[Fuinjutsu](Techniques/Fuinjutsu/)**
*   **[Chakra Control](Techniques/Chakra_Control/)**

---

## 🎒 Equipment & Tools
The steel and the tools of the trade.

*   **[Equipment Shop Index](Equipment/Equipment_Shop.md)** - Browse by Merchant.

---

## 🧹 Cleanup Zone (Work in Progress)
*Audited 2026-05-29. Source-PDF names in earlier draft were stale; mapped to the actual `Sourcebooks/Naruto_d20/` filenames during the audit.*

### Still outstanding

2.  **[ ] Bloodline Audit:** 30+ bloodline files exist + Archive + Community_Compendium + rules. JSON-class-conversion goal (bloodlines take levels) not done.

### Won't do (GM decision 2026-05-29)

4.  **[~] School Design:** *Removed.* The L5R-inspired School concept for Chunin exams was dropped from the campaign.
5.  **[~] Calendar Audit:** *Removed.* Calendar will be handled by a Foundry VTT module rather than vault notes.
8.  **[~] School Extraction:** *Removed.* Paired with #4; same rationale.

### Completed (already done in prior sessions)

1.  **[x] Skills Overhaul:** *Done 2026-05-29.* All 43 Pathfinder-shaped skill files exist under [`Character_Options/Skills/`](Character_Options/Skills/) with the [Skill_Registry](Character_Options/Skills/Skill_Registry.md) as entry point. Naruto-Pathfinder-d20M merge done per source priority. Knowledge (Geography) intentionally omitted (terrain → Nature, locale → Local). Only [Perform (Martial Arts)](Character_Options/Skills/Perform%20(Martial%20Arts).md) subcategory file written; the other four Perform subcategories (Act, Dance, Music, Oratory) intentionally deferred until campaign demand surfaces.
3.  **[x] Prestige Audit:** *Done 2026-05-29.* Format pass via [`format_prestige_classes.py`](../Creation%20Zone/automation_scripts/format_prestige_classes.py) normalised 27 of 33 files (stripped trailing colons from `## Requirements:` etc.). Two structural outliers resolved: `Hisuigakure.md` was a village-perks stub mis-filed under Prestige — reformatted and moved to [`Character_Options/Villages/Hisuigakure.md`](Character_Options/Villages/Hisuigakure.md); `Naruto Clans.md` was an orphan design-planning document with no references — deleted.
6.  **[x] Gamemastering Extraction:** Content from `Sourcebooks/Naruto_d20/Supplments/Naruto d20 - GM_s Helper.pdf` is in [`GM_Tools/`](GM_Tools/) (7 substantive files: Collaboration_Techniques, Reality_Manipulation, Quick_Time_Events, Missions_and_Bounties, Village_Generation, Jounin_Examination, Traps).
7.  **[x] NPC Rewrite:** Stat blocks extracted into [`Bestiary/NPC_Archetypes/`](Bestiary/NPC_Archetypes/) (Low/Mid level Ordinary/Heroic Ninja, High Level Hunter-Nin, Ninja Law Enforcement, Ninja Scout) plus [`Bestiary/Templates/`](Bestiary/Templates/) (Aquatic Subtype, Chakra Vampire, Cursed Seal, Demonic, Heroic, etc.). Source: `Sourcebooks/Naruto_d20/Supplments/Naruto d20 - Creatures Compendium.pdf`.
9.  **[x] Summoning Extraction:** Rules + samples + feats + pacts in [`Summoning/`](Summoning/) (8 files including Summoning_Rules, Sample_Summons, Sage_Summons, Summon_Feats, Monster_Familiar, Golem, Fox community creation, Pacts/). Source: `Sourcebooks/Naruto_d20/Supplments/Naruto d20 - Conjurer_s Codex` volumes I-IV + Demon Clown + Limited Edition.
10. **[x] Puppeteering Extraction:** Rules + tables + components in [`Equipment/Ninja_Tools/Puppets/`](Equipment/Ninja_Tools/Puppets/) (6 files including Puppets_Table, Puppet_Crafting, Advanced_Puppet_Components, Puppet_Cores, GM_Helper_Puppet_Additions, Playwrights_Primer_Components). Source: `Sourcebooks/Naruto_d20/Supplments/Naruto d20 - Playwright_s Primer.pdf`.

*   **[Classes Archive](Character_Options/Classes/Archive/)**
*   **[Bloodlines Archive](Character_Options/Bloodlines/Archive/)**

---

## 🔬 Structured Index (auto-maintained)

Per-entity YAML sidecars feed the `naruto-d20-character-builder` skill. Coverage and lint state at **[Mechanics Dashboard](mechanics-dashboard.md)**.

Active rules projection: **[House Rules Active](schemas/house_rules_active.yaml)**.

See [docs/superpowers/specs/2026-06-04-kaihou-mechanics-audit-and-access-design.md](../docs/superpowers/specs/2026-06-04-kaihou-mechanics-audit-and-access-design.md) for the design.
