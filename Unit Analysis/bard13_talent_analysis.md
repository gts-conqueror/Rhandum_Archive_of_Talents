# Mathematical Analysis: Bard 13 Talent Analysis

This analysis finally uncovers the secrets of the 3rd ascension talent for the Bard unit — a question that has continued to trouble players as a definite conclusion has yet to be achieved. All formulas and resources used are deposited below along with disclaimers. This analysis will help you choose the stronger talent (if you haven't already) and inspire a newfound boost of power and understanding in your unit, inevitably winning you more matches.

This scientific analysis evaluates the mathematical efficiency of two competing Bard abilities:

- **Option A — Hymn of Vigor:** Attack Speed +20% for 10s after leaving music mode
- **Option B — Aria of Power:** Critical Damage +40% for 10s after 5 insp gained

---

## I. Quantitative Framework

For the purpose of this analysis, Bard is evaluated at the level 13 state with 0 inspiration to keep calculations and tables less complex and easy to follow, alongside some constant values and a crit of 2000%.

To calculate the 10-second burst window, we define the following variables based on the provided stats:

| Variable | Value |
|---|---|
| Base Damage (D_b) | 2301 |
| Base Crit Multiplier (M) | 20.0x (2000%) |
| Base Crit Chance (P_c) | 0.05 (5%) |
| Time Window (T) | 10s |

The **Total Expected Damage (E)** is derived from the sum of standard hits (including natural crit hits).

---

## II. Comparative Performance Analysis

The following table breaks down the raw output of both options during the active 10s buff window. Note that Hymn of Vigor increases the *frequency* of attacks, while Aria of Power increases the *magnitude* of the multiplier.

| Metric | Hymn of Vigor (Attack Speed +20%) | Aria of Power (Crit Damage +40%) |
|---|---|---|
| Total Attacks (N) | 24 | 20 |
| Avg. Normal Hit Damage | 4,486.95 | 4,532.97 |
| Calculated DPS | 10,768.8 | 9,065.9 |
| Total Expected Damage (in 10 seconds) | 107,688 | 90,659 |

*Table 1: Performance comparison during the 10s active buff window.*

**Observation:** Hymn of Vigor results in an **18.4% higher DPS floor** compared to Aria of Power. The primary driver of this disparity is the increased frequency of attacks, leading to a higher total output.

**Explanation:** This is an interesting breakdown because the Base Crit Multiplier (20x) is massive, but the Crit Chance (5%) is very low. This creates a "lottery" effect where most of your damage comes from rare, huge spikes. Since we can't know exactly when the critical hit will land, I spread it out among individual hits so when it occurs it'll be well accounted for. Even though Aria of Power has a higher *damage per hit*, it loses to Hymn of Vigor because it hits 4 extra times in the same time period with a similar Crit rate and Crit bonus.

---

## III. Performance Analysis: Synergy with Cacophony

After finding out the power differences between the two talents, I sought to find out if the final talent could sway the results — or if one talent has a better synergy with it than the other.

To calculate the 10-second burst window, we define the following variables:

| Variable | Value |
|---|---|
| Base Damage (D_b) | 2301 |
| Base Crit Multiplier (M) | 20.0x (2000%) |
| Base Crit Chance (P_c) | 0.05 (5%) |
| Clump PROC Chance (P_p) | 0.04 (4%) |
| Time Frame (T) | 10s |

The **Total Expected Damage (E)** is derived from the sum of standard hits (including natural crits) and the expected Clump procs.

| Metric | Hymn of Vigor (Attack Speed +20%) | Aria of Power (Crit Damage +40%) |
|---|---|---|
| Total Attacks (N) | 24 | 20 |
| Avg. Normal Hit Damage | 4,486.95 | 4,532.97 |
| Chaotic Clump Damage | 46,020 | 46,940.4 |
| Expected Clumps | 0.96 | 0.80 |
| Total Expected Damage | 151,866 | 128,211 |

*Table 2: Performance comparison during the 10s active buff window with Cacophony factored in.*

**Observation:** The Total Expected Damage in 10 seconds is still higher for Hymn of Vigor.

---

## IV. The Synergy Effect & Battle Strategy

The introduction of Cacophony creates a **"scaling trap"** for Critical Damage. Since Cacophony is a guaranteed critical hit, it seems intuitive to buff Critical Damage. However, in stochastic systems (RNG-based games), frequency usually beats magnitude when the magnitude is already high.

**Why Speed Dominates:**

- **Linear Scaling:** Speed multiplies the entire damage profile. Crit Damage only adds a small fractional increase to an already saturated 20.0x multiplier.
- **Cacophony Multiplier:** Because the Clump proc is a fixed 4% per shot, increasing shots per second increases Cacophony's contribution to your total DPS — hence increasing your DPS as a whole.

**Battle Strategy — "Mechanical Advantage":**

Both talents share similar mechanics, but Hymn of Vigor *moggs* due to its activation criteria being only *after leaving music mode*. This means you could theoretically be in the boosted state for the duration of the game. Aria of Power has a numerical requirement to be achieved as well as an upper limit, making it less practical in the heat of battle. Speed paired with a low inspiration cooldown is a lethal combo.

---

## V. Balancing and Equality

Once I determined that Hymn of Vigor was superior to Aria of Power, I wondered exactly how much Critical Damage Bonus Aria of Power would require to match Hymn of Vigor's DPS.

**Theoretical Description:**

To determine the Equilibrium Point, we solve for the bonus value that allows Aria of Power to reach the same Expected Value (E) as the Attack Speed modifier.

- **Hymn of Vigor Expected Output:** 2.34 × Base Damage
- **Aria of Power Goal:** Must also reach 2.34 × Base Damage

> *Note: It's 2.34 rather than 1.2 to account for the critical chance of a 20x damage effect.*

**Equating the Talents:**

Using the standard probability distribution formula, solve for the unknown variable B:

```
E = Base × (1 + (P_c × ((M + B) - 1)))
```

Where **B (Required Bonus)** = Unknown

**Step-by-Step Mathematical Proof:**

| Step | Operation | Result |
|---|---|---|
| Step 1 | Isolate the Bonus Segment | 0.05 × (19 + B) = 1.34 |
| Step 2 | Remove Probability Constraint | 19 + B = 26.8 |
| Step 3 | Solve for B | B = 7.8 |

**Conclusion:** The analysis reveals a major discrepancy in stat weight. For Aria of Power to achieve mathematical parity with Hymn of Vigor, it would need to provide a **+780% Critical Damage Bonus**.

---

## VI. Final TL;DR Analysis

| Option | Pros | Cons |
|---|---|---|
| **Hymn of Vigor** (Attack Speed) | Higher Clump frequency; scales better with base 20x multiplier; more consistent; easier activation | — |
| **Aria of Power** (Crit Damage) | Larger single-hit "screen numbers"; zero resource cost change | Mathematically inferior; high reliance on RNG; poor scaling with existing 2000% base multiplier |

*Table 3: Final evaluation of Bard Ability Tree pathing.*

**Conclusion: Hymn of Vigor is the mathematically superior choice.** It offers higher average damage, better synergy with Cacophony, and higher reliability through ease of activation.

---

## VII. Formulas & Resources

### A. Input Values (The "Raw Data")

These are the static numbers used as the foundation of the calculations.

| Variable | Value | Description |
|---|---|---|
| Base Damage | 2,301 | The damage dealt by a standard, non-critical arrow. |
| Attack Interval | 0.5s | The time between shots. |
| Base Attacks Per Second | 2.0 | Derived from interval (1 ÷ 0.5). |
| Base Crit Multiplier | 20x (2000%) | The total damage of a crit (Base + 1900% bonus). |
| Base Crit Chance | 5% (0.05) | The chance for a standard arrow to crit. |
| Chaotic Clump Chance | 4% (0.04) | The separate proc chance for the Tier 2 ability. |
| Option A (Speed) | +20% | Increases total shots fired by 1.2x. |
| Option B (Crit Bonus) | +40% | Adds 0.4x to the Crit Multiplier (20.4x total). |

### B. Formula Dictionary

These formulas convert chance-based effects into stable comparison values.

| Formula Name | The Math Equation | Purpose |
|---|---|---|
| Average Hit Damage | `Base × (1 + (Chance × (Multiplier - 1)))` | Determines expected damage per hit when crits are probabilistic. |
| Shots in Window | `(Duration ÷ Interval) × (1 + Speed Buff)` | Calculates total shots during the buff window. |
| Expected Clump Gain | `Total Shots × Proc Chance × (Base × Multiplier)` | Calculates average bonus damage from Clumps. |
| Total Burst Damage | `(Shots × Avg Hit) + Expected Clump Gain` | Final total damage during the 10-second window. |

### C. The "Logic Check": Why 1900%?

If you take your time to check the math, you'll find I treated the crit multiplier as 19 + 1. A 20× crit multiplier is handled as 19 in probability calculations because **1 represents the original damage** and **19 represents the bonus damage** added on top of it. The base hit is always guaranteed; only the bonus portion is probabilistic.

This is similar to systems where you start with 200% critical damage: 100% is your normal damage, and the additional 100% is the bonus applied when a crit occurs. The total becomes 2× damage, but only the extra 1× is the added benefit. If the formula mistakenly treated all 20 as bonus, it would calculate 21 pizzas total — which is incorrect.

---

*This project is based on MY.GAMES's Rush Royale: Update 35.0 (2026)*

*This project is a non-commercial fan work that is not affiliated with MY.GAMES or Rush Royale. All Rush Royale names and terms remain their property.*
