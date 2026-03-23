# Robot (Reincarnation Robot)

## Unit Overview: Robot

**Role:** DPS **|**
**Rarity:** Legendary **|**
**Core Mechanic:** Deals damage scaled to the number of parts accumulated through merging,  
each Robot merge contributes parts that when applied, directly increase the unit's damage output.

### Current State
Robot is a competitive DPS option that holds its own against other damage dealers through
solid part-scaling and a satisfying merge-investment loop. Its vulnerability is structural:
parts accumulated over time can be lost to RNG events with no recovery mechanism, meaning
a well-built Robot can be set back significantly through no fault of the player. As the meta's
top DPS units grow more reliable, Robot's lack of insurance makes it increasingly hard
to justify at higher levels where losing parts mid-run is decisive.

### Design Goal
These reincarnation skills introduce a recovery architecture that preserves Robot's high
investment identity without removing the risk the A.R.A. system creates a floor beneath
the damage ceiling, rewarding players who build deep while protecting them from catastrophic
part loss. A player running Robot well should feel like they are managing a war machine:
powerful, resource-hungry, and now equipped with an off site backup that keeps it from
going down for good.

---

## Reincarnation Proposal

### Skill 1: Overclocked (with Harlequin)
- Attack speed increases by 1% per merge rank on the field.
- Gains +0.2% per merge rank after max is reached.

| Level | Max Attack Speed Boost |
|-------|------------------------|
| L1    | 10%                   |
| L2    | 15%                   |
| L3    | 20%                   |

---

### Skill 2: Aerial Strike (with Phoenix)
- Every 10 parts applied, small drones appear, attacking for 5s dealing a total of Robots Combined Critical Damage in an Area.

| Level | Area Damage % of Combined Robot's Crit Damage |
|-------|-----------------------------------------------|
| L1    | 200%                                          |
| L2    | 300%                                          |
| L3    | 400%                                          |

---

### Skill 3: Med-Bay Protocol / Cloud Backup (with Scrapper)
- Introduces new robot: **A.R.A. (Advanced Recovery Assistant)**
  - 10% chance of spawning (cannot upgrade with parts).
  - When a robot is destroyed, A.R.A. recovers a number of its parts when close by *(like **Twilight Rangers** soul Mechanic. Parts are applied when merged with a regular robot)*.

| Level | Cache Parts |
|-------|-------------|
| L1    | 7           |
| L2    | 9           | 
| L3    | 12          | 
