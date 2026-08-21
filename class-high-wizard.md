# High Wizard — Skill Formulas

The **High Wizard** is the transcendent Mage → Wizard branch: the server's premier **magic nuker**, dealing massive area damage with the elements.

Magic damage is built from your **MATK** (see [Damage & Combat Formulas](damage-formulas.md) for how MATK and MDEF work). Most spells deal **MATK per hit** and strike several times. The percentages below are the **exact ratios from this server's code**, applied on top of your MATK before the enemy's MDEF and element are counted.

## Single-target spells

| Spell | Element | Damage | Notes |
| --- | --- | --- | --- |
| **Fire / Cold / Lightning Bolt** | Fire / Water / Wind | **100% MATK per bolt**, one bolt per skill level (Lv10 = 10 bolts) | Match the bolt element to the enemy's weakness. |
| **Soul Strike** | Ghost | 100% + 5% × Lv per hit (multi-hit) | Homing; extra damage vs **Undead**. |
| **Frost Diver** | Water | 100% + 10% × Lv | Chance to **Freeze** the target. |
| **Napalm Vulcan** *(HW)* | Ghost | 125% per hit (multi-hit) | Chance to **Curse**. |
| **Magic Crasher** *(HW)* | Weapon's element | An **instant** hit that uses your **MATK as attack power** | No cast time — great for interrupting. |

## Area spells

| Spell | Element | Damage | Notes |
| --- | --- | --- | --- |
| **Fire Ball** | Fire | 140% + 20% × Lv | Small splash. |
| **Fire Wall** | Fire | 50% MATK per hit | Wall that blocks and pushes enemies. |
| **Thunderstorm** | Wind | 80% MATK per hit | Area lightning. |
| **Heaven's Drive** | Earth | 125% MATK | Small ground area. |
| **Sightrasher** | Wind | 100% + 20% × Lv | Fires off your Sight orbs, knockback. |
| **Water Ball** | Water | 100% + 30% × Lv per hit | Hits once per water tile around you — huge on watery maps. |
| **Storm Gust** | Water | 100% + 40% × Lv **per hit**, hits many times | The classic AoE — repeated hits **Freeze** enemies. |
| **Meteor Storm** | Fire | ~125% MATK per meteor, many meteors | Wide area, chance to **Stun**. |
| **Lord of Vermilion** | Wind | Multi-hit Wind area | Chance to **Blind**. |
| **Jupitel Thunder** | Wind | Multi-hit, knockback | Pushes the target away with each hit. |
| **Gravitation Field** *(HW)* | Neutral | Heavy fixed damage over an area | You can't move while channeling it. |

## Key buffs & utility

- **Mystical Amplification (Amplify Magic Power)** — greatly boosts the damage of your **next single spell**.
- **Energy Coat** — reduces incoming damage using your SP.
- **Ganbantein** — erases ground-based skills (Safety Wall, Pneuma, etc.).
- **Quagmire** — slows enemies and lowers their AGI/DEX.
- **Stave Crasher / Sight / Fire Pillar** — utility and setup spells.

> **Tip:** Lower your cast time with DEX and INT — see [Damage & Combat Formulas](damage-formulas.md#cast-time).

*More classes under **Class Skill Formulas**.*
