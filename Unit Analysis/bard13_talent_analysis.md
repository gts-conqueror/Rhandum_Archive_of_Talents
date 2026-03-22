# Mathematical Analysis: Bard 13 Talent Analysis

This analysis evaluates the mathematical efficiency of two competing Bard abilities under the
**Multiplicative Scaling Model**, confirmed via in-game testing.

- **Option A - Hymn of Vigor:** Attack Speed +20% for 10s after leaving music mode
- **Option B - Aria of Power:** Critical Damage +40% for 10s after 5 insp gained

> **Note: This analysis supersedes the original additive model. A critical correction was made
> after in-game testing revealed that Critical Damage bonuses in Rush Royale apply as
> multiplicative modifiers to the base Critical Multiplier, not additive ones.**

---

## I. Quantitative Framework

For the purpose of this analysis, Bard is evaluated at the level 13 state with 0 inspiration,
alongside some constant values and a crit of 2000%.

| Variable | Value |
|---|---|
| Base Damage (D_b) | 2,301 |
| Base Crit Multiplier (M) | 20.0x (2000%) |
| Base Crit Chance (P_c) | 0.05 (5%) |
| Time Window (T) | 10s |
| Option A Modifier | 1.2x Attack Speed |
| Option B Modifier | 1.4x Critical Multiplier (Multiplicative) |

---

## II. Comparative Performance Analysis

The following table breaks down the raw output of both options during the active 10s buff window.

| Metric | Hymn of Vigor (Attack Speed +20%) | Aria of Power (Crit Damage ×1.4) |
|---|---|---|
| Total Attacks (N) | 24 | 20 |
| Effective Crit Multiplier | 20.0x | 28.0x (20 × 1.4) |
| Standard EV per Hit | 1.95x | 2.35x |
| Standard Hit Damage | 4,487 | 5,408 |
| Calculated DPS | 10,769 | 10,815 |
| Total Expected Damage (Standard) | 107,687 | 108,147 |

*Table 1: Standard attack performance during the 10s active buff window.*

**Observation:** Standard arrow DPS is near-identical between both options under the multiplicative
model. Aria of Power hits harder per shot (28x crit vs 20x) while Hymn of Vigor fires more
frequently. The decisive factor shifts to Cacophony.

**Explanation:** Under additive scaling, +40% to a 20x multiplier is negligible. Under
multiplicative scaling, the entire 20x base is amplified - 20 × 1.4 = 28x - which meaningfully
changes the damage profile of every crit and, critically, every Chaotic Clump proc.

---

## III. Performance Analysis: Synergy with Cacophony

The Cacophony synergy is where the multiplicative model decisively shifts the outcome.
A Clump proc is a guaranteed critical hit - meaning it is directly and fully amplified by Aria
of Power's 1.4x modifier.

| Variable | Value |
|---|---|
| Base Damage (D_b) | 2,301 |
| Base Crit Multiplier (M) | 20.0x (2000%) |
| Base Crit Chance (P_c) | 0.05 (5%) |
| Clump Proc Chance (P_p) | 0.04 (4%) |
| Time Frame (T) | 10s |

| Metric | Hymn of Vigor (Attack Speed +20%) | Aria of Power (Crit Damage ×1.4) |
|---|---|---|
| Total Attacks (N) | 24 | 20 |
| Standard EV per Hit | 1.95x | 2.35x |
| Standard Damage | 107,687 | 108,147 |
| Effective Clump Crit Multiplier | 20.0x | 28.0x |
| Clump Hit Damage | 46,020 | 64,428 |
| Expected Clumps | 0.96 | 0.80 |
| Expected Clump Damage | 44,179 | 51,542 |
| **Total Expected Damage** | **151,866** | **159,689** |

*Table 2: Full performance comparison including Cacophony during the 10s window.*

**Observation:** Aria of Power produces **5.15% higher total output** than Hymn of Vigor.
The margin is driven by the amplified Clump damage — 64,428 per proc vs 46,020 — which more
than compensates for the four fewer shots fired.

---

## IV. The Synergy Effect & Battle Strategy

The multiplicative model reveals why Aria of Power's interaction with Cacophony is more
powerful than it initially appears.

**Why Multiplicative Crit Wins Against Speed:**

- **Clump Amplification:** Because Chaotic Clump is a guaranteed critical hit, it receives the
  full benefit of the 1.4x multiplier. Hymn of Vigor has no equivalent leverage on proc damage.
- **Diminishing Returns on Speed:** Adding 20% more shots to an already fast attack pattern
  produces linear gains. Multiplying the entire critical structure — including procs — produces
  compounding value per event.
- **Frequency vs. Magnitude:** At a 5% crit rate, most attacks are standard hits. Aria of Power
  makes each of the rare, high-value events (crits and Clumps) significantly more impactful
  rather than adding more of the common, lower-value events.

**Battle Strategy — "Precision Over Volume":**

Aria of Power's activation condition (5 inspirations) requires intentional play, but rewards it
with an amplified burst window that hits harder on every high-value proc. Hymn of Vigor remains
easier to activate consistently, which still makes it a valid choice for players who prioritise
simplicity — but the mathematical ceiling belongs to Aria of Power.

---

## V. Balancing and Equality

With the multiplicative model confirmed, the equilibrium point shifts significantly compared to
the original analysis.

**Hymn of Vigor Expected Output:** 1.95x Base Damage (standard EV, additive model baseline)

The question becomes: at what multiplicative modifier does Aria of Power produce equivalent
total output to Hymn of Vigor's 10s window of 151,866?

**Solving for Equilibrium:**

We solve for multiplier X such that Aria of Power's 10s total equals Hymn of Vigor's:

| Step | Operation | Result |
|---|---|---|
| Step 1 | Set target total | 151,866 |
| Step 2 | Subtract standard damage at X shots | 108,147 (at 20x, 20 shots) |
| Step 3 | Required clump contribution | 43,719 |
| Step 4 | Solve for clump multiplier at 0.80 procs | ~23.8x |
| Step 5 | Minimum multiplier to break even | ~1.19x (vs confirmed 1.4x) |

**Conclusion:** Aria of Power surpasses Hymn of Vigor at any multiplicative modifier above
approximately 1.19x. At the confirmed 1.4x, it comfortably exceeds the speed talent's output.

---

## VI. Final TL;DR Analysis

| Option | Pros | Cons |
|---|---|---|
| **Aria of Power** (Crit Damage) | Higher Clump amplification; multiplicative scaling on all crit events; mathematically superior total output | Requires 5 inspirations to activate; harder to maintain consistently |
| **Hymn of Vigor** (Attack Speed) | Easier activation (any exit from music mode); consistent and reliable; stronger in the original additive model | Lower ceiling under confirmed multiplicative scaling; no leverage on proc damage |

*Table 3: Final evaluation of Bard Ability Tree pathing — Multiplicative Model.*

**Conclusion: Aria of Power is the mathematically superior choice under confirmed multiplicative
scaling.** The 1.4x critical multiplier amplifies both standard crits and Cacophony procs,
producing 5.15% higher total output in a 10-second window despite firing four fewer shots.

---

## VII. Formulas & Resources

### A. Input Values

| Variable | Value | Description |
|---|---|---|
| Base Damage | 2,301 | Standard non-critical hit damage |
| Attack Interval | 0.5s | Time between shots |
| Base Attacks Per Second | 2.0 | Derived from interval (1 ÷ 0.5) |
| Base Crit Multiplier | 20x (2000%) | Total damage of a crit |
| Base Crit Chance | 5% (0.05) | Chance for a standard arrow to crit |
| Chaotic Clump Chance | 4% (0.04) | Separate proc chance for Tier 2 ability |
| Option A (Speed) | ×1.2 | Increases total shots fired by 1.2x |
| Option B (Crit) | ×1.4 | Multiplies the entire Crit Multiplier by 1.4 |

### B. Formula Dictionary

| Formula Name | Equation | Purpose |
|---|---|---|
| Multiplicative Crit EV | `Base × (1 + (P_c × ((M × modifier) - 1)))` | Expected damage per hit under multiplicative scaling |
| Shots in Window | `(Duration ÷ Interval) × (1 + Speed Buff)` | Total shots during the buff window |
| Clump Hit Damage | `Base × (M × modifier)` | Single Clump proc damage at given multiplier |
| Expected Clump Gain | `Total Shots × Proc Chance × Clump Hit Damage` | Average Clump contribution over window |
| Total Burst Damage | `(Shots × Avg Hit) + Expected Clump Gain` | Final total damage during the 10s window |

### C. The Multiplicative Correction

Under the original additive model, +40% Crit Damage was treated as 20.0x + 0.4 = 20.4x — a
negligible improvement. In-game testing confirmed the game applies this as a multiplier to the
full stat: 20.0x × 1.4 = 28.0x. This distinction is the entire reason the conclusion flips.
A 1% improvement on a rare event is worthless. A 40% amplification of the same rare event —
and every guaranteed-crit proc tied to it — is decisive.

---
*Note: This is the second version of the Bard analysis once it was confirmed the game engine used a 'Multiplicative Scaling Model' and not an 'Additive Scaling Model'*

*This project is based on MY.GAMES's Rush Royale: Update 35.0 (2026)*

*This project is a non-commercial fan work that is not affiliated with MY.GAMES or Rush Royale.
All Rush Royale names and terms remain their property.*
