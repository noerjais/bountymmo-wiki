# Lord Knight — Skill Formulas

The **Lord Knight** is the transcendent Swordman → Knight branch: a tanky, high-damage melee class built around spears and two-handed swords.

Every damage skill starts from a **base of 100%** and adds a bonus on top. The percentages below are the **exact skill ratios used on this server** (pulled from the server's own combat code). Remember: this % is applied to your ATK, and then modifiers, size, element, and the enemy's DEF still apply — see [Damage & Combat Formulas](damage-formulas.md) for the full picture.

## Damage skills

| Skill | Damage (by skill level) | Max level | Notes |
| --- | --- | --- | --- |
| **Bash** | 100% + 30% × Lv | Lv10 → **400%** | Single powerful strike. |
| **Magnum Break** | Inner 3×3: 100% + 20% × Lv · Outer 5×5: 100% + 10% × Lv | Lv10 → **300% / 200%** | Fire-element area hit; also briefly gives your weapon the Fire element. |
| **Pierce** | 100% + 10% × Lv | Lv10 → **200%** | Hits extra times against larger targets. |
| **Spear Stab** | 100% + 20% × Lv | Lv10 → **300%** | Knocks the target back. |
| **Spear Boomerang** | 100% + 50% × Lv | Lv5 → **350%** | Ranged throw — hits from a distance. |
| **Brandish Spear** | 100% + 20% × Lv (area cone) | Lv10 nearest cell ≈ **560%** | Area attack in front; the cells closest to you take a big bonus at higher levels, outer cells less. |
| **Bowling Bash** | 100% + 40% × Lv | Lv10 → **500%** | Area attack that shoves enemies together. |
| **Head Crush** | 100% + 40% × Lv | Lv5 → **300%** | Can inflict **Bleeding**. |
| **Joint Beat** | 50% + 10% × Lv (**×2** if it breaks the Neck) | Lv10 → **150%** (up to **300%**) | Randomly breaks a body part, applying a debuff; Neck break also doubles the damage. |
| **Spiral Pierce** | 100% + 50% × Lv | Lv5 → **350%** | **Always hits** (can't be dodged); damage also **scales with your weapon's weight**. Spear only. |

> **How to read this:** e.g. Bash Lv10 = 100% + 30%×10 = **400%** of a normal attack's ATK, *before* the enemy's DEF and your element/size/card modifiers are applied.

### Brandish Spear detail

Brandish Spear hits a cone of cells in front of you. The base is **100% + 20% × Lv**, but the tiles closest to you gain extra damage as the skill levels up (roughly +half, +quarter, +eighth of the base at Lv 4+, 7+, and 10). At Lv 10 the nearest cell can reach about **560%**, while the far cells stay near the base.

## Key buffs & utility

- **Two-Hand Quicken** — big ASPD and HIT boost while using a two-handed sword.
- **Concentration** — raises HIT and ATK for a while, at the cost of some DEF/FLEE.
- **Aura Blade** — adds a flat bonus of extra damage to every hit.
- **Parrying** — chance to block incoming physical attacks (two-handed swords only).
- **Berserk (Frenzy)** — massively boosts Max HP, ASPD, and ATK, but drains your HP over time and locks you out of items and most skills.
- **Tension Relax** — greatly speeds up HP recovery while resting.
- **Provoke / Endure / Auto Counter** — classic Swordman utility for tanking and countering.

*More classes coming next — see the other pages under **Class Skill Formulas**.*
