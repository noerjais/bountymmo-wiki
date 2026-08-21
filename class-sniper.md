# Sniper — Skill Formulas

The **Sniper** is the transcendent Archer → Hunter branch: a ranged powerhouse that fights with bows, a loyal Falcon, and battlefield traps.

Every damage skill starts from a **base of 100%** and adds a bonus on top. The values below are the **exact skill ratios used on this server** (pulled from its combat code). This % applies to your ATK; the enemy's DEF, element, size, and your cards still apply afterward — see [Damage & Combat Formulas](damage-formulas.md).

## Bow skills

| Skill | Damage (by skill level) | Max level | Notes |
| --- | --- | --- | --- |
| **Double Strafe** | 100% + 10% × (Lv − 1) | Lv10 → **190%** | Fires two arrows in a rapid shot. |
| **Arrow Shower** | 150% + 10% × Lv | Lv10 → **250%** | Area attack around a target spot; can knock back. |
| **Charge Arrow** | **150%** (fixed) | — | Single shot that knocks the target far back. |
| **Phantasmic Arrow** | **150%** (fixed) | — | Knockback shot that uses **no arrows**. |
| **Sharp Shooting** | 200% + 50% × Lv | Lv5 → **450%** | High **critical rate** (+200 crit) and hits everything in a line. |

## Falcon skills

Your Falcon's damage doesn't use the normal weapon formula — it scales with **DEX, INT, and your Steel Crow level**:

- **Blitz Beat** — each strike = **(DEX ÷ 10 + INT ÷ 2 + Steel Crow Lv × 3 + 40) × 2**. It hits several times (more hits with higher Falcon Mastery / Blitz Beat level). It can also trigger automatically while auto-attacking.
- **Falcon Assault** — takes that Blitz Beat damage and multiplies it by **(150% + 70% × Lv)**. At Lv5 that's **5× the Blitz Beat base** in a single heavy hit. Great burst that ignores normal weapon ATK.

## Traps

Traps are placed on the ground and detonate on enemies. On this server their damage scales with **Skill Level, DEX, INT, and your base level**:

> **Land Mine / Blast Mine / Claymore Trap damage = Skill Lv × DEX × (3 + Base Level ÷ 100) × (1 + INT ÷ 35)** (±10% swing)

- **Land Mine** — Earth-element single hit.
- **Blast Mine** — small area, Wind element.
- **Claymore Trap** — larger area, Fire element.
- **Ankle Snare** — doesn't damage, but roots the enemy in place (great for kiting).

The **Research Trap** skill adds extra flat damage to all of these.

## Key buffs & utility

- **Improve Concentration (Attention Concentrate)** — raises AGI and DEX and reveals hidden enemies.
- **True Sight** — temporary boost to all stats plus HIT and critical.
- **Wind Walk** — boosts your party's FLEE and movement speed.
- **Falcon Mastery / Falcon Eyes** — improves your falcon and enables the falcon skills.
- **Remove Trap** — recover or clear traps.

*More classes coming next — see the other pages under **Class Skill Formulas**.*
