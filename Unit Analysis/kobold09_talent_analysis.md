# Mathematical Analysis: Kobold's Mines Ore Efficiency Talent Analysis

This analysis evaluates the mathematical efficiency of two competing Mine abilities for the Kobold/Mine system:
- **Option A - Motherload**
- **Option B - Energy of the Deeps**

This analysis determines which talent provides superior damage scaling and board economy across different play styles and deck compositions.

---

## I. Quantitative Framework

| Variable | Definition |
|---|---|
| Base Ore Yield (Y_b) | 2 × Merge Rank |
| Motherload Yield (Y_m) | 3 × Merge Rank at 50% probability |
| Energy Yield (Y_e) | Merge Rank² (Guaranteed) |
| Damage Bonus (D_1) | +2% per ore (before soft cap) |
| Diminished Bonus (D_2) | +0.4% per ore (after soft cap) |

The **Expected Value (E)** for Motherload accounts for its probabilistic nature. Energy of the Deeps produces a deterministic, guaranteed output.

---

## II. Comparative Yield Analysis

| Merge Rank (R) | Motherload (E = 2.5R) | Energy of the Deeps (Y = R²) | Efficiency Leader |
|:---|:---|:---|:---|
| Rank 1 | 2.5 | 1 | **Motherload (+150%)** |
| Rank 2 | 5.0 | 4 | **Motherload (+25%)** |
| Rank 3 | 7.5 | 9 | **Energy (+20%)** |
| Rank 4 | 10.0 | 16 | **Energy (+60%)** |
| Rank 5 | 12.5 | 25 | **Energy (+100%)** |
| Rank 6 | 15.0 | 36 | **Energy (+140%)** |
| Rank 7 | 17.5 | 49 | **Energy (+180%)** |

>**Observation:** A critical crossroads occurs at Rank 3. Below Rank 3, Motherload is mathematically superior. At Rank 3 and above, Energy of the Deeps enters quadratic growth yielding nearly triple the ore of Motherload at Rank 7.

---

## III. The Synergy Effect: Board Economy vs. Raw Yield

While Energy of the Deeps offers higher raw numbers at high ranks, it introduces a "Tactical Tax" through its interaction with the **Mana Power-up (MPU)**.

### 1. The "Board Lock" Dilemma (Energy of the Deeps)

Kobolds using Energy of the Deeps do not vanish until an MPU is triggered. This creates two compounding disadvantages:

- **Space Congestion:** The Kobold occupies a board tile, reducing board real estate.
- **Repositioning Penalty:** The MPU can only move *empty* mines. A Kobold still inside a mine prevents that mine from being repositioned to a more advantageous tile until the MPU clears it.

### 2. Immediate Payoff (Motherload)

Motherload preserves the standard vanishing mechanic. This enables high-tempo play, mines are constantly emptied and repositioned to collect new Kobolds, supporting faster early-game ore accumulation and maintaining full board flexibility throughout.

---

## IV. Damage Scaling & The Soft Cap

- **Pre-cap:** Each ore provides a significant +2% damage boost.
- **Post-cap:** Each ore provides a marginal +0.4% damage boost.

**Strategic Impact:** Energy of the Deeps is the most efficient tool for reaching the Max Ore Limit in massive bursts. A Rank 7 unit produces 49 ore in a single occurence, which is perfect for suddenly overwhelming your opponent. Motherload builds toward the cap steadily without the board management overhead, making it the better fit for decks that cannot afford to tie up tile space waiting for MPU clearance.

---

## V. Formulas & Resources

| Formula Name | Equation | Purpose |
|---|---|---|
| Motherload Expected Yield | `E = (0.5 × 2R) + (0.5 × 3R) = 2.5R` | Average ore output accounting for 50% proc probability |
| Energy Yield | `Y = R²` | Deterministic ore output at a given merge rank |
| Crossover Point | `2.5R = R²` → `R = 2.5` | The merge rank at which Energy of the Deeps surpasses Motherload in expected yield |

---

## VI. Final TL;DR Analysis

| Option | Pros | Cons |
|:---|:---|:---|
| **Motherload (A)** | Superior early-game tempo; strong for low-rank and frequent merges; keeps board clear; consistent across all deck types | Weak scaling at high ranks; 50% RNG can produce dry spells in critical waves |
| **Energy of the Deeps (B)** | Quadratic scaling (R²); guaranteed outcome; exceptional late-game and soft-cap efficiency | Congests board space; creates MPU dependency; penalises Rank 1–2 units heavily |

**Conclusion:** There is no universal superior choice, the correct answer depends on the Unit you're playing

Use **Motherload** for high-tempo, aggressive merging strategies where board flexibility is non-negotiable.

Use **Energy of the Deeps** if your deck builds consistently to high-rank units and can manage the MPU cadence needed for regular board clearing. Units like Dark Inquisitor or Solitude Banshee, which naturally operate with fewer occupied tiles, are well-suited to absorbing the board lock cost in exchange for the exponential ore yield.
*(Sidetip: Using the scrapper unit in this deck will be a great asset)*

---
*This analysis originated from a 'Das Boot' conversation*

*This project is based on MY.GAMES's Rush Royale: Update 35.0 (2026)*

*This project is a non-commercial fan work that is not affiliated with MY.GAMES or Rush Royale. All Rush Royale names and terms remain their property.*
