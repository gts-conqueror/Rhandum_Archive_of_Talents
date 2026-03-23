# Shaman

## Unit Overview

**Role:** Special **|**
**Rarity:** Legendary **|**
**Core Mechanic:** Reduces or increases the merge rank of opponent or ally units.

### Current State
Shaman performs reliably through early Leagues, its ability to directly manipulate merge ranks is powerful enough to swing boards with limited counterplay, and this directness has given it a reputation for feeling overpowered at mid-level play. That same bluntness is its ceiling: a single, binary use case with no layered decision-making leaves it shallow for the player running it and leaves no room to grow at higher Leagues where board states stabilise and rank manipulation loses relevance.

### Design Goal
These talents reframe Shaman from a blunt instrument into a ceremonial strategist one that operates through ritual formation, timing, and board commitment rather than raw rank manipulation. Fox's Blessing rewards preparation and spatial awareness on your own board; Fox's Curse exports that pressure onto the opponent's merge economy. A player running Shaman well should feel like they are conducting something deliberate: setting the stage, holding the formation, and watching a prepared sequence land.

---

## Base Mechanic Adjustment
Before diving into the talents, the following baseline adjustments are proposed to modernize the unit’s utility:
- Reduces Curse activation to 1 curse every 2 merges
- Gains a mana ability reducing the merge rank of the highest-rank Shaman (cannot drop below 1).
- Cooldown: *TBD by developers. Probably around 20s*


## Talent & Reincarnation Proposal
---
### 1st Talent

- **Left: Fox's Blessing**
  - A new Shaman variant is introduced: **Chief Ritualist**.
  - The first pair of Shamans merged does not produce a curse, instead, it creates a Chief Ritualist.
  - With the Chief Ritualist placed in the center of the board and one Shaman at each of two corners, forming a combined merge rank of 7:
    - For 15s, the formation conducts a blessing that increases the merge rank of 2 units adjacent to the Ritualist by 2.
    - The Shamans must not be merged or disturbed during the ritual, any disruption cancels the blessing and restarts the process.

- **Right: Fox's Curse**
  - A new Shaman variant is introduced: **Chief Ritualist**.
  - With the Chief Ritualist placed in the center of the board and one Shaman at each of the four corners, forming a combined merge rank of 10:
    - For 20s, the formation conducts a curse that shrouds the opponent's board in miasma, making any attempt by the opponent to merge two units has a 15% chance to fail, leaving the resulting unit's rank unchanged (resets at the end of the wave).
    - The Shamans must not be merged or disturbed during the ritual, any disruption cancels the effect and restarts the process.
    - *(In co-op, the curse inverts: the miasma has a chance to increase the merge rank of ally units instead.)*

  >*VFX / SFX to indicate ritual activation, miasma presence, and disruption.*
---

### 2nd Talent

- **Left: Loved by the Goddess**
  - After successful ritual, each unit has:
    - 3% chance for 1st talent change of merge rank by 2.
    - 0.5% chance for merge rank change by 3.

- **Right: A Believer’s Faith**
  - Merging other units has a 3% chance to activate Shaman’s basic mechanic.

---

### 3rd Talent

- **Left: Totem of Great Fortune**
  - Throws a totem on the path before the Phantom (30s duration).
  - Totem has 5% chance to cancel boss’s effect by goddess’s power.

- **Right: Venge Totem of Calamity**
  - Throws a totem on opponent’s path during Phantom (30s duration).
  - Totem has a 2.5% chance to double boss’s effect by goddess’s power.

---

### Final Talent

- **Deity of Reality**
  - Every wave: 5% chance for a Shaman to be possessed upon summoning.
  - Possessed Shaman does not attack. When merged with Chief Ritualist, becomes enlightened.
  - After last monster appears:
    - Summons the goddess of reality (two fox spirits):
      - *Fox of Destruction*: Stuns 3 units on opponent’s board.
      - *Fox of Creation*: Creates traps slowing boss by 20%, then grants your highest merge rank unit +30% damage for the boss wave.

---

## Reincarnation Skills

### Skill 1: Enlightened Spirit (with Dryad)
- Enlightened Shaman grants 1% crit chance to adjacent units (or all units if in center).
  - L1: 0.75% crit chance
  - L2: 1.00% crit chance
  - L3: 1.25% crit chance

### Skill 2: Deity’s Punishment (with Knight Statue)
- Deity of Reality’s fox can lock opponent’s hero ability.
  - L1: 5% chance for 2.5s
  - L2: 10% chance for 3.5s
  - L3: 15% chance for 5s

### Skill 3: Witch Doctor (with Witch)
- Enlightened Chief Ritualist can remove negative effects from adjacent units.
  - L1: 7% chance
  - L2: 14% chance
  - L3: 20% chance
