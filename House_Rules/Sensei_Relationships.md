# Sensei Relationships

Senseis are **gatekeepers of jutsu progression** (see [[Sensei]]). This file replaces the implicit "talk to NPC, get bonus" model with a tier track so they behave like relationships with access, trust, favors, and political costs instead of public faucets.

> Training Arc update: the old **Teaching Capacity** block economy is retired. Use [[Training Schedules]] to decide whether a sensei is available, who else is present, and what scene pressure surrounds the training. Legacy capacity numbers on old cards are only descriptive availability cues.

## The Five Tiers

| Tier | How a PC reaches it | What it grants |
| --- | --- | --- |
| **Unaware** | Default for every NPC. | None. The sensei doesn't know who the PC is. |
| **Aware** | 1 successful Influence check ([[Influência]], 1 block). | Sensei recognizes the PC, will sell rumors and basic technique gossip. Acts as a +1 Self-Teaching-equivalent on the PC's next solo Learn check in the sensei's specialty (one-shot, doesn't stack with a scroll bonus). |
| **Recognized** | 3 cumulative Influence successes (counting Aware) across separate days. At least 1 must be a Difficult DC or include a Discovery success. | Sensei agrees to teach at scheduled opportunities. PC may use the sensei for the Tutoring bonus when the fiction and [[Training Schedules]] make them available. |
| **Tutoring** | Complete one favor, errand, or C-rank mission for the sensei or their clan. | PC is the sensei's declared student in one discipline. While learning any technique the sensei knows, the PC may **reroll one failed Learn check per required success** of that technique (a 3-success technique grants 3 rerolls during its training). The reroll's result is final and does not consume additional days. The Tutoring bonus from [[11_Learn DC]] continues automatically as long as the relationship stays warm. |
| **Mentor** | Arc-level beat — vouched at a council, saved their life, exposed a corruption case, etc. GM permission required. | Any technique the PC trains while this Mentor relationship is active requires **1 fewer success** (minimum 1), regardless of source (self-teaching, other tutors, scrolls). A PC may have **only one Mentor** in their entire career. Mentor tier also unlocks access to the sensei's **Personal Hijutsu**, if they have one. Senseis do **not** teach the steps of Mastery — that is solo work. |

## Retired: Teaching Capacity

Do not track a weekly teaching-block pool. The scarcity is now **time, access, attention, risk, and competing students**, handled through the Training Arc schedule and event beats.

- If two PCs want the same sensei in the same week, decide whether they share a scene, split attention, or collide with another genin team's schedule.
- If a PC is at Tutoring tier, the sensei will make time unless a named event, crisis, deployment, or faction obligation blocks them.
- If old notes list "Teaching Capacity: 4/6/8 blocks", read that as a quick availability label: **rare**, **normal**, or **institutionally available**.
- Capacity does **not** create rollover, budgeting, or per-student entitlement.

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

Senseis are also subject to the Training Arc calendar and schedule state:
- Post-Wall-Breach (mid Month of the Hare): any sensei reassigned to the wall becomes harder to reach. Replace normal training access with letters, emergency drills, or one-off scene windows.
- Month of the Dragon (militarization): all senseis' Recognized DC raised by +2 unless the PC has a clan referral.

## Per-Sensei Card Stub

Each named sensei in the campaign should have an entry like:

```
Name • District / Home Location • Discipline(s)
Availability: rare / normal / institutional / deployed
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
