# Sensei Relationships

Senseis are **gatekeepers of jutsu progression** (see [[Sensei]]). This file replaces the implicit "talk to NPC, get bonus" model with a tier track so they behave like scarce, contested resources instead of public faucets.

## The Five Tiers

| Tier | How a PC reaches it | What it grants |
| --- | --- | --- |
| **Unaware** | Default for every NPC. | None. The sensei doesn't know who the PC is. |
| **Aware** | 1 successful Influence check ([[Influência]], 1 block). | Sensei recognizes the PC, will sell rumors and basic technique gossip. Acts as a +1 Self-Teaching-equivalent on the PC's next solo Learn check in the sensei's specialty (one-shot, doesn't stack with a scroll bonus). |
| **Recognized** | 3 cumulative Influence successes (counting Aware) across separate days. At least 1 must be a Difficult DC or include a Discovery success. | Sensei agrees to teach. PC may book the sensei's weekly **Teaching Capacity** for Tutoring bonus (per [[11_Learn DC]]). |
| **Tutoring** | Complete one favor, errand, or C-rank mission for the sensei or their clan. | PC is the sensei's declared student in one discipline. While learning any technique the sensei knows, the PC may **reroll one failed Learn check per required success** of that technique (a 3-success technique grants 3 rerolls during its training). The reroll's result is final and does not consume additional days. The Tutoring bonus from [[11_Learn DC]] continues automatically as long as the relationship stays warm. |
| **Mentor** | Arc-level beat — vouched at a council, saved their life, exposed a corruption case, etc. GM permission required. | Any technique the PC trains while this Mentor relationship is active requires **1 fewer success** (minimum 1), regardless of source (self-teaching, other tutors, scrolls). A PC may have **only one Mentor** in their entire career. Mentor tier also unlocks access to the sensei's **Personal Hijutsu**, if they have one. Senseis do **not** teach the steps of Mastery — that is solo work. |

## Teaching Capacity (the scarcity)

Each named sensei has a weekly **Teaching Capacity** measured in blocks. Default is **8 blocks/week** for a standard Jounin instructor; lower for irregulars (Shushu-ya rogues, retired specialists) and higher for academy staff and clan elders during quiet weeks.

- Teaching Capacity is the budget the sensei spreads across all their students at Recognized+.
- If two PCs are both at Recognized with the same sensei, they negotiate or compete for the weekly pool.
- A PC at Tutoring tier gets first claim on at least half the sensei's weekly capacity by default.
- Capacity does **not** roll over week-to-week.

## Constraints

- A PC may hold **only one Tutoring sensei per discipline** (Ninjutsu, Taijutsu, Genjutsu, Chakra Control, Fuinjutsu) at a time.
- Switching Tutoring sensei drops the previous one to Recognized and forfeits any rerolls not yet used on in-progress techniques.
- A PC may have **only one Mentor in their entire career.** Choosing a Mentor is a permanent identity commitment; the Mentor tier cannot be moved to another sensei later.
- A sensei's tier with a PC **drops one step** if the PC skips them for 14+ consecutive days during downtime. (Active missions and arc beats pause the timer.) Mentor tier is exempt — it does not decay.
- A failed Influence check by 5+ blocks that skill for the social encounter; by 10+ blocks the sensei entirely for the rest of the arc phase ([[Influência]]).

## Stacking Rules

Per [[11_Learn DC]]: Tutoring and Self-Teaching do **not** stack. A PC choosing Tutoring forgoes any scroll/tablet bonus on that technique. Situational bonuses (weights, training environment) **do** stack with Tutoring.

The Mentor's −1 success modifier applies **regardless of stacking** with Tutoring or Self-Teaching — it represents the shaping effect of the Mentor relationship on how the PC learns, not a per-technique tutoring effect.

## Personal Hijutsu vs Clan Hijutsu

A sensei's **Personal Hijutsu** — a technique they personally developed, inherited as their own secret, or hold as a signature — can be taught at **Mentor tier** if the sensei is willing.

A **Clan Hijutsu** belongs to the clan as a whole, not to any individual sensei. Even a Mentor-tier sensei cannot grant access on their own authority. PCs gain access to Clan Hijutsu only by raising their **clan relationship** through dedicated arc missions; this is a separate track from the Sensei tiers above and is GM-mediated through specific campaign events (clan trials, oaths, public service, restoration of clan honor). No fixed DC table — those missions are designed per case.

Once granted by the clan, learning the Hijutsu still follows the normal Learn rules and Hijutsu success surcharge from [[11_Learn DC]].

## Arc-Phase Modifiers

Senseis are also subject to the [[Arc State Overlay]] (per-month state):
- Post-Wall-Breach (mid Month of the Hare): Teaching Capacity halved for any sensei reassigned to the wall. Track which senseis leave.
- Month of the Dragon (militarization): all senseis' Recognized DC raised by +2 unless the PC has a clan referral.

## Per-Sensei Card Stub

Each named sensei in the campaign should have an entry like:

```
Name • District / Home Location • Discipline(s)
Teaching Capacity: 8 blocks/week
Influence skills: Diplomacy, Sense Motive (primary), Knowledge (clan) (secondary)
Influence DCs: 18 typical / 23 difficult (APL 5)
Discovery rewards:
  - Strength: ...
  - Weakness: ...
Tutoring grant: Rerolls available for any technique the sensei knows (see tier table).
Mentor candidate: Yes / No. Personal Hijutsu (if any): [Hijutsu Y].
Clan affiliation: [Clan] — Clan Hijutsu gating is separate, see Personal vs Clan Hijutsu.
Notes: schedule quirks, factional alignment, leaves the village mid-Hare, etc.
```

The master roster lives in `Campaign Management/NPCs/Sensei Roster.md` (to be built in Step 3 of the rollout).

## Linked

- [[Sensei]] — campaign design notes that motivated this system.
- [[11_Learn DC]] — the underlying Learn check rules.
- [[Influência]] — the Influence and Discovery check rules.
- [[Action_Blocks]] — block economy.
- [[Location_Schema]] — how Sensei Hubs expose these tiers.
