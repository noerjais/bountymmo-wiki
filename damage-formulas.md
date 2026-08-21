# Damage & Combat Formulas

Bounty MMO runs on **Renewal** mechanics (with the **classic attack-speed** formula) — the "Revo-Classic" style. That means your **base level** directly boosts your damage, and defense works differently from old-school servers.

This page explains **how your ATK and MATK turn into real damage**. For the stat basics (what STR/AGI/VIT/INT/DEX/LUK do, plus HIT, FLEE, CRIT and cast time), see [Revo System Information](revo-system-information.md).

## Physical damage — step by step

When you land a physical hit, the game builds your damage roughly in this order:

1. **Your ATK** = **Status ATK** (red box: from STR/DEX/LUK and your base level) + **Weapon ATK** (blue box: the weapon's ATK, its refine, and a random swing based on weapon level). Status ATK effectively counts **twice**, but only **Weapon ATK** is boosted by **% ATK cards** — that's why a great weapon beats a 4-slotted starter weapon.
2. **Skill multiplier** — a normal hit is 100%; a skill applies its own % (see the per-class skill pages).
3. **Size modifier** — your weapon does more or less depending on the target's size (small/medium/large).
4. **Element modifier** — your attack's element vs the target's element (the elemental table; e.g. Fire vs Earth hits hard, Fire vs Water is weak).
5. **% bonuses** — race, element, and size cards (like a race-killer card) multiply your damage here.
6. **Enemy defense** (this is the big one):

   > **Damage = Damage × (4000 + eDEF) ÷ (4000 + 10 × eDEF) − sDEF**

   - **eDEF** = hard DEF, the "blue" DEF from equipment and refine — reduces damage by a **percentage**.
   - **sDEF** = soft DEF, the "red" DEF from VIT, AGI and base level — subtracted as a **flat** amount afterward.
7. **Base-level bonus** — because this is Renewal, higher base level adds extra damage on top.

Every hit deals at least **1** damage.

### How much does hard DEF actually block?

| Enemy eDEF | Damage you still deal | Reduction |
| --- | --- | --- |
| 100 | 82% | 18% |
| 200 | 70% | 30% |
| 300 | 61% | 39% |
| 400 | 55% | 45% |
| 500 | 50% | 50% |
| 1000 | 36% | 64% |

Notice the **diminishing returns** — each point of DEF is worth a little less than the last. Soft DEF (flat) is then subtracted on top, so it matters most against many small hits.

## Magic damage — step by step

1. **Your MATK** = **Status MATK** (red box) + **Weapon MATK** (blue box, with a random swing):
   - **Status MATK** = INT + (INT ÷ 2) + (DEX ÷ 5) + (LUK ÷ 3) + (Base Level ÷ 4)
   - **Weapon MATK** swings from about **70% to 130%** of the weapon's MATK — a higher weapon level makes the swing land higher.
2. **Skill multiplier** — the spell's % (almost all magic is skill-based).
3. **Element modifier** — the spell's element vs the target's element.
4. **Enemy magic defense**:

   > **Damage = MATK × (1000 + eMDEF) ÷ (1000 + 10 × eMDEF) − sMDEF**

   - **eMDEF** = hard MDEF (mostly from equipment) — a **percentage** cut.
   - **sMDEF** = soft MDEF (from INT/VIT and base level) — a **flat** cut afterward.

### How much does hard MDEF block?

| Enemy eMDEF | Damage you still deal | Reduction |
| --- | --- | --- |
| 10 | 92% | 8% |
| 20 | 85% | 15% |
| 30 | 79% | 21% |
| 40 | 74% | 26% |
| 50 | 70% | 30% |
| 100 | 55% | 45% |

MDEF uses **1000** as its base (physical DEF uses 4000), so **each point of MDEF blocks much more** than a point of physical DEF. That's why "MDEF-piercing" gear is prized for magic builds.

## Critical hits

- A crit deals **+40% damage** and **never misses** (it ignores the target's FLEE).
- Crits are still reduced by the target's DEF, but cards and gear can push crit damage well past +40%.
- An **Assassin wielding a Katar** has their **critical rate doubled** (a hidden bonus not shown on the stat window).

## Attack speed (ASPD)

This server uses the **classic ASPD** formula (not the Renewal one). Your ASPD comes from your **class + your weapon's base delay**, sped up mainly by **AGI** and slightly by **DEX**, plus any ASPD potions and skills. The cap is **193** — hitting 193 means the fastest possible attacks, which is why so many builds aim for it.

## Cast time

Skill casting is split into **Variable** and **Fixed** cast time:
- **Variable cast** is reduced by **DEX and INT**. You remove it completely when **(DEX × 2) + INT = 530**.
- **Fixed cast** can't be lowered by stats (only special gear/skills). Not every skill has a fixed portion.

See [Revo System Information](revo-system-information.md) for cast delay vs cooldown details.

## Why base level matters so much

Because Bounty MMO is **Renewal**, your **base level feeds directly into your Status ATK, Status MATK, and a bonus to damage**. Two identical characters at different levels will not hit for the same amount — leveling up is itself a damage upgrade.

---

*Next up: per-class skill formulas — the exact damage % of each class's skills. See the pages under **Class Skill Formulas**.*
