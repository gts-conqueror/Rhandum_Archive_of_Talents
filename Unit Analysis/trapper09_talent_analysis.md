# Mathematical Analysis: Trapper Talent for Utility and Wave Control

This analysis evaluates the mathematical efficiency of Trapper's First talents options under the
**Uniform Multiplicative Scaling Model** established via in-game testing:
- **Option A - Big Game Hunting** 
- **Option B - Trap Master**

---

## I. Quantitative Framework

| Variable | Value |
|---|---|
| Base Crit Multiplier (M) | 20.0x (2000%) |
| Base Crit Chance (P_c) | 0.05 (5%) |
| Option A Modifier (B_a) | 1.2x to Critical Magnitude (Max Stacks) |
| Option B Modifier (B_b) | 1.4x to Final Damage Output (Max Stacks) |

---

## II. Comparative Multiplier Analysis

The following table demonstrates how these bonuses interact under the multiplicative model.

| Metric | Base (No Talent) | Option A (Crit Path) | Option B (Damage Path) |
|:---|:---|:---|:---|
| Crit Multiplier | 20.0x | 24.0x (×1.2) | 20.0x |
| Final Damage Modifier | 1.0x | 1.0x | 1.4x |
| Expected Value (E) | **1.95x** | **2.15x** | **2.73x** |
| Efficiency Increase | - | **+10.3%** | **+40.0%** |

>***Observation:** Option A produces a genuine 10.3% efficiency gain over the baseline. However, Option B still dominates by applying
its multiplier globally to *all* damage, not just the 5% crit window.*

---

## III. The "Scope Gap" (Crit Multiplier vs. Global Multiplier)

### 1. The Scope Limitation (Option A)

Option A only amplifies the crit component of expected damage. With a 5% crit rate, that means 95% of all hits receive zero benefit from the talent.

Expected Value breakdown at Option A:
- Normal hits (95%): contribute `0.95 × 1.0 = 0.95` to EV
- Crit hits (5%): contribute `0.05 × 24.0 = 1.20` to EV
- **Total EV: 2.15x**

### 2. The Global Advantage (Option B)

Option B applies to every single hit regardless of type normal hits, crit hits, and proc
damage all receive the full 1.4x modifier. There is no scope limitation.

Expected Value breakdown at Option B:
- All hits: `[1 + (0.05 × 19)] × 1.4 = 1.95 × 1.4`
- **Total EV: 2.73x**

Critically, Option B also produces a larger crit hit (28.0x) than the talent specifically
dedicated to crits (24.0x) - because the global multiplier applies on top of the existing
20x base.

---

## IV. Utility: Target Hunting vs. Area Denial

- **Option A:** Focuses pressure on Bosses and Mini-bosses. Provides genuine
  value in compositions built specifically around boss burst - decks that already handle wave
  control through other units. Outside of that context, it leaves the most common cause of
  defeat unaddressed: **wave leakage** (lack of wave control) from insufficient area control.
- **Option B:** Replaces standard nets with Mantraps, spreading the 40% damage
  modifier across the full path and assisting in clearing high-health armoured waves. Also
  includes a **discrete damage proc** on trap landing, which itself benefits from the global
  multiplier.

---

## V. Formulas & Resources

| Formula Name | Equation | Purpose |
|---|---|---|
| EV - Option A (Multiplicative Crit) | `1 + [P_c × (M × 1.2 - 1)]` | Expected damage per hit with crit-only multiplier |
| EV - Option B (Global Multiplier) | `[1 + P_c × (M - 1)] × 1.4` | Expected damage per hit with global multiplier |
| Crit Hit - Option A | `Base × (M × 1.2)` = `Base × 24.0x` | Single crit damage under Option A |
| Crit Hit - Option B | `Base × M × 1.4` = `Base × 28.0x` | Single crit damage under Option B |

---

## VI. Final TL;DR Analysis

| Feature | Option A (Sniper) | Option B (Shredder) |
|:---|:---|:---|
| Primary Stat | ×1.2 Crit Magnitude (Max) | ×1.4 Total Damage (Max) |
| Scaling | Multiplicative - crit window only (5% of hits) | Multiplicative - all hits universally |
| Effective Crit Hit | 24.0x | 28.0x |
| Expected Value | 2.15x (+10.3% over baseline) | 2.73x (+40.0% over baseline) |
| Targeting | Boss-centric | Wave-centric |
| Best In | Dedicated boss-burst compositions | General use; all deck types |

**Conclusion: Trap Master  is the mathematically superior choice** by a margin
of 26.9% over Option A. A Global Multiplier outperforms a Critical Multiplier because it applies to every
hit including the larger crits it already produces rather than only the 5% crit window.
The scope advantage of Option B is fundamental and cannot be overcome by increasing the crit
modifier alone at this crit rate.

---

*This project is based on MY.GAMES's Rush Royale: Update 35.0 (2026)*

*This project is a non-commercial fan work that is not affiliated with MY.GAMES or Rush Royale.
All Rush Royale names and terms remain their property.*
