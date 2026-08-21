# Champion — Skill Formulas

The **Champion** is the transcendent Acolyte → Monk branch: a **combo fighter** and burst-damage monster, famous for the one-shot finisher **Asura Strike**.

Every damage skill starts from a **base of 100%** and adds on top. The values below are the **exact ratios from this server's code**, applied to your ATK before DEF/element/size — see [Damage & Combat Formulas](damage-formulas.md).

## Damage skills

| Skill | Damage (by skill level) | Max level | Notes |
| --- | --- | --- | --- |
| **Investigate** | 100% + 75% × Lv | Lv5 → **475%** | **Ignores DEF** — the higher the target's DEF, the more it hits. |
| **Finger Offensive** | 100% + 50% × Lv | Lv5 → **350%** | Ranged; throws your **Spirit Spheres** at the target. |
| **Raging Trifecta / Chain Combo** | 150% + 50% × Lv | Lv5 → **400%** | Combo hit that continues from a normal attack. |
| **Raging Quadruple Blow** | 240% + 60% × Lv | Lv5 → **540%** | Next combo step after Chain Combo. |
| **Chain Crush Combo** | 400% + 100% × Lv | Lv5 → **900%** | Later combo step. |
| **Tiger Knuckle Fist** | 40% + 100% × Lv | Lv5 → **540%** | Combo step that can **immobilize** the target. |
| **Palm Strike** | 200% + 100% × Lv | Lv5 → **700%** | Ranged push. |
| **Asura Strike** *(Guillotine Fist)* | **800% + 10% × your current SP** — consumes **all** your SP and Spirit Spheres | huge | The ultimate finisher. Example: 500 SP → about **5,800%** in a single hit. |

> **Asura math:** with 5 Spirit Spheres and full SP, Asura Strike hits for 800% plus 10% of your SP total. It empties your SP bar and requires the **Fury (Explosion Spirits)** state, so it's a one-shot gamble — land it or you're left defenseless.

## Combo flow

Champions chain skills together: a normal attack → **Chain Combo** → **Raging Quadruple Blow** → **Tiger Knuckle Fist** → often finishing with **Asura Strike**. Each step must be pressed within the combo window.

## Key buffs & utility

- **Summon Spirit Sphere** — stores spheres that power your combos and Finger Offensive.
- **Fury (Explosion Spirits)** — the state required for Asura Strike; boosts SP and ASPD.
- **Steel Body (Mental Strength)** — hugely reduces damage taken for a short time.
- **Body Relocation (Snap)** — instantly teleport a short distance.
- **Blade Stop** — freeze you and an attacker in place.
- **Dodge (Flee)** — passive evasion boost.

*More classes under **Class Skill Formulas**.*
