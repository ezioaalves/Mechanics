# Chakra Control

**Ability:** Wisdom (Wis)
**Trained Only:** Yes
**Armor Check Penalty:** No

Chakra Control governs every act of *intentional* chakra manipulation that doesn't itself constitute a technique: concealing the cost of a jutsu so chakra-sensors can't read it, drawing on personal reserves to fuel a desperate push, and — adapted from the Concentration check of older d20 systems — holding focus on a technique through pain, motion, weather, or grappling.

In the Kaihou system, Chakra Control fully replaces the d20 Modern Concentration skill and the Pathfinder Concentration check.

---

## Description

A character with Chakra Control is *deliberate* with their chakra in a way most shinobi are not. Where Ninjutsu, Genjutsu, Taijutsu, and Fuinjutsu let a character *execute* techniques, Chakra Control governs the chakra itself — its visibility, its flow, its retention under pressure.

This skill is the foundation of every other chakra-using skill. A character can fail to learn a technique they're trying to perform; a character with low Chakra Control may fail to keep that technique running once the world starts hitting them back.

---

## Check

Chakra Control has four primary uses. Each uses the same skill modifier; the DC and what the check measures differ.

### 1. Conceal Chakra Cost *(Naruto D20)*

Conceal the chakra expenditure of a technique you are performing so that creatures with chakra-sensing abilities cannot detect the activity. You cannot conceal *part* of a technique's cost — it is concealed in full or not at all.

| Conceal Chakra | Base DC |
| :-- | :-- |
| Base check DC | 15 |
| Every Rank of the technique | +1 |
| Every point of chakra cost | +1 |

A successful check means the technique is performed without alerting creatures that can sense chakra. You cannot take 10 or take 20 when concealing chakra cost.

### 2. Tap Reserves *(Naruto D20)*

Gain temporary chakra by deliberately lowering your chakra reserve by an equivalent amount.

| Tap Reserves | Base DC |
| :-- | :-- |
| Performed as a move action ¹ | 10 |
| Performed as a swift action ¹ | 15 |
| Per point of temporary chakra gained | +1 |
| Character performs no seals ² | — |
| Character performs a half-seal ² | −2 |
| Character performs a hand seal ² | −5 |

¹ Choose one action speed.
² Choose one seal option (the seal sequence reduces the DC at the cost of broadcasting your activity).

A successful check grants temporary chakra for 1 minute per character level by lowering your reserve by the same amount. You cannot take 10 or take 20 when tapping your reserves.

### 3. Maintain Focus When Distracted *(adapted from Pathfinder & d20 Modern Concentration)*

When something interrupts you while you are performing a technique, you must make a Chakra Control check or **lose the technique without effect** (its chakra cost is still paid). The DC depends on the source of the distraction. Replace "spell level" with the technique's **Rank**.

| Distraction | DC |
| :-- | :-- |
| Damaged during the technique | 10 + damage dealt + technique Rank |
| Continuous damage during the technique | 10 + ½ continuous damage + technique Rank |
| Affected by a non-damaging technique mid-cast | the other technique's Save DC + your technique Rank |
| Grappled or pinned | 10 + grappler's CMB + technique Rank |
| Vigorous motion (bouncy ride, small boat in rough water, riding horse) | 10 + technique Rank |
| Violent motion (rough vehicle, rapids, galloping horse, storm-tossed deck) | 15 + technique Rank |
| Extraordinarily violent motion (earthquake) | 20 + technique Rank |
| Entangled in net or snare | 15 + technique Rank |
| Wind carrying blinding rain or sleet | 5 + technique Rank |
| Wind-driven hail, dust, or debris | 10 + technique Rank |

A pinned character can only perform techniques without somatic components (i.e. that require no seals). If you fail the check, you lose the technique without effect.

### 4. Perform Defensively *(adapted from Pathfinder & d20 Modern)*

Perform a technique while avoiding the attacks of opportunity it would normally provoke.

- **DC 15 + technique Rank** to perform the technique without provoking.

If the check succeeds, you perform the technique normally without attacks of opportunity from initiating it. If the check fails, the technique fails (its chakra is still spent) and you still don't provoke for the *initiation*, but you do provoke for any other reason (e.g. moving in a threatened square). A successful defensive check still does not let you take 10 on the technique itself.

---

## Action

Making a Chakra Control check does not require an action by itself — it is either a reaction (when made in response to a distraction) or part of the action you were already taking (when made actively to conceal, tap, or perform defensively).

The exception is **Tap Reserves**, which is either a swift or move action by the chosen option above.

---

## Try Again

- **Conceal Chakra:** Cannot retry on the same performance; try again by performing the technique again.
- **Tap Reserves:** Yes, with another action of the same kind.
- **Maintain Focus When Distracted:** Yes — but a success does not cancel the effects of a previous failure (e.g. a jutsu already lost stays lost).
- **Perform Defensively:** No — the technique either succeeded defensively or it failed; retry by performing the technique again on a later action.

---

## Special

- You cannot take 10 or take 20 on any Chakra Control check.
- A character with the **Focused** feat (d20 Modern) gains a +2 bonus on all Chakra Control checks.
- A character with the **Chakra Control Adept** feat (Naruto D20 — if active) gains a +2 bonus on all Chakra Control checks.

---

## Synergy

- A character with **2 or more ranks** in Chakra Control gains a **+2 bonus on Learn checks** for Chakra Control techniques. *(Naruto D20 originally "5 ranks"; converted via the −3 rank-prereq rule.)*
- A character with **7 or more ranks** in Chakra Control can create Chakra Control *hijutsu* or *kinjutsu* techniques without suffering the standard additional penalty. *(Naruto D20 originally "10 ranks"; converted via the −3 rank-prereq rule.)*

---

## Source Notes

*Priority: Naruto D20 > Pathfinder > d20 Modern.*

- **Naruto D20 (NarutoD20 Redux v1.3.pdf):** Conceal Chakra, Tap Reserves, Synergy, Hijutsu/Kinjutsu creation. Ability score (Wis) and Trained Only status follow Naruto D20.
- **Pathfinder (aonprd.com/Rules.aspx?ID=205):** Distraction DC table — formulas adapted from "+ spell level" to "+ technique Rank" to fit Naruto D20's Rank system. Defensive Performance DC formula (15 + Rank × 2) adapted from defensive casting.
- **d20 Modern (modernsrd.pdf, p. 66):** Distraction DC table cross-referenced (matches Pathfinder for motion/weather/grapple values); Defensive Action DC 15 baseline preserved as a flat check (Pathfinder's scaling-with-level formula takes priority per the Naruto > PF > d20M rule). The Focused feat +2 is preserved as a portable bonus.

**Conflict resolution & Rank conversion:** The defensive-performance DC is the Pathfinder scaling formula (`15 + spell_level × 2`) re-expressed for Naruto Ranks. Naruto Ranks scale roughly **2× faster** than Pathfinder spell levels (Ranks routinely reach 20+; spell levels cap at 9), so the multiplier is halved: PF's `15 + (spell_level × 2)` becomes **`15 + Rank`**, preserving the same effective difficulty curve. Rank-prerequisite numbers in the Synergy block are likewise converted via the project-wide **−3 rule** (Naruto D20 / d20 Modern rank prereqs minus 3 to match Pathfinder's narrower rank progression).
