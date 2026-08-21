# Revo System Information

### Primary statistics

Stats are the six fundamental character statistics that make (or break) a character. Stats start out with a base value of 1 and can be raised as far as 130. Base stats are increased by spending stat points, higher stats costing more to raise. Stat points are gained with base level increases, the amount increasing with higher levels.
![Primary stats](.gitbook/assets/Primary_stats.png)

- **STR:** For melee weapons, every point in STR increases StatusATK by +1. For ranged weapons, every 5 points in STR increases StatusATK by +1. Each point of STR also adds +30 Weight Limit. The bonus ATK per 10 STR for melee weapons is no longer applied.
- **AGI:** Every point in AGI adds +1 Flee and increases ASPD. Additionally, every 5 points in AGI adds 1 SoftDEF.
- **VIT:** Every point in VIT adds +1% MaxHP, +2% HP Healing Item effectiveness, and +1% resistance to several status effects. Every 2 points in VIT adds +1 SoftDEF. Every 5 points in VIT adds +1 SoftMDEF and +1 HP Recovery Rate.
- **INT:** Every point in INT adds +1.5 StatusMATK, +1% MaxSP, 1% SP Healing Item effectiveness, and decreases cast time. Every 2 points of INT adds +1 SoftMDEF and every 6 points in INT adds +1 SP Recovery Rate. The multiples of 5 and 7 bonus for minMATK and maxMATK is no longer applied.
- **DEX:** For ranged weapons, every point in DEX increases StatusATK by +1. For melee weapons, every 5 points in DEX increases StatusATK by +1. Every point in DEX also adds +1 HIT, decreases cast time, and increases ASPD. Every 5 points in DEX adds +1 StatusMATK and +1 SoftMDEF. The bonus ATK per 10 DEX for ranged weapons is no longer applied.
- **LUK:** Every point in LUK adds +0.3% Critical Hit Rate, as well as resistance to several status effects. Every 3 points in LUK adds +1 StatusATK, +1 StatusMATK, and +1 HIT. Every 5 points in LUK adds +1 Flee and +1% Anti-Critical Rate, and Every 10 points in LUK adds +1 Perfect Dodge.![Hit statistics](.gitbook/assets/Hit_statistics.png)

### Secondary statistics

- **ATK:** ATK is the byproduct of STR and DEX and is divided into two, StatusATK(red box) and WeaponATK(blue box). In essence, they both contribute to the final damage (StatusATK being multiplied by two). However, when amplified by % cards, only the WeaponATK is amplified. This makes it so that people don't rely on 4-slotted starter weapons (such as a Quad-Racial Composite Bow), and instead will strive to get better, rarer weapons to deal better damage. NOTE: Percent(%) damage modifiers are hidden values. Meaning, the amount they give isn't reflected on your stats window.
![Atk statistics](.gitbook/assets/Atk_statistics.png)![Substats](.gitbook/assets/Substats.png)
- **MATK** As with ATK, Magical Attack Power(MATK) is also divided into two, StatusMATK(red box) and WeaponMATK(blue box). In MATK's case, WeaponMATK makes up the greater percentage of the final damage, due to the variance factor which relates to weapon level.
![Matk statistics](.gitbook/assets/Matk_statistics.png)
- **DEF & MDEF** DEF and MDEF are values that reduces incoming damage. There are 2 types of defense: Softdef (red box): comes from INT and VIT and reduces damage by flat amount. Harddef: is the total of equipment defense, including upgrades(blue box) and have some calculation in it to reduce damage by percentage.
![Def statistics](.gitbook/assets/Def_statistics.png)
- **HIT** Hit rate is the accuracy rating, in which you land your physical attacks. It is affected by DEX and LUK, but primarily, luck is the significant factor between the two.
    - HIT can be calculated as (175 + BaseLv + DEX + Floor(LUK ÷ 3) + Bonus).
    - Based on the example above: (175 + 82 + 53 + Floor(5 / 3 = 1.3) + 0) = 311 Hit
- **FLEE** Flee is the stat that is responsible for a characters dodge.  There are 2 types of flee, Flee (red box) and Perfect dodge (blue box):
    - Flee is your evasion from physical attacks(excluding critical hits) and is calculated as (100 + BaseLv + AGI + Floor(LUK ÷ 5) + Bonus)
    - Perfect dodge is your evasion from physical attacks (including critical hits) and is increased every 10 LUK. It's default value is 1.
    - Based on the example above (100 + 82 + 52 + Floor(5/5 = 1) + 0) = 235 Flee
![Flee statistics](.gitbook/assets/Flee_statistics.png)

**NOTE**: at 100 perfect dodge, you're immune to physical attacks (but it is impossible to achieve since it requires you to have 1000 LUK).

- **CRITICAL** Critical is the byproduct of LUK and deals 40% more damage compared to non-critical attacks, it also ignores flee(never misses). Just like any normal attacks though, critical is reduced by the targets defense. However, there are items that provide Critical Damage bonuses, which means with the right combination of equipment and cards, it's possible to deal 200% your regular damage per critical hit, or even higher. NOTE: An assassin wielding a katar will have their critical doubled, but not shown in the stats window (hidden value).
![Critical statistics](.gitbook/assets/Critical_statistics.png)
- **ASPD** Attack Speed is the hit per second rating. It depends on the player's class, equipped Weapon Type, Speed Modifiers, AGI and DEX. ASPD increases hits/second exponentially. It has a limit of 190.
![Aspd statistics](.gitbook/assets/Aspd_statistics.png)
- **CAST TIME** Cast time is the time needed to completely activate a skill. It is split into Fixed cast time and Variable cast Time. Fixed cast time: is the casting time that cannot be reduced, unless by special means (third job skills and items - not implemented yet) Variable cast time: can be reduced by INT and DEX. To remove Variable cast time completely, the formula is ((DEX x2) + INT) = 530. NOTE: Not all skills have Fixed casting time.
- **DELAY & COOLDOWN** Delay is the time needed to cast another skill. Delay is divided into two: Cast Delay: is the time needed to cast another skill, and affects all skills (global cooldown).  ![Casting example](.gitbook/assets/Casting_example.gif)
    - **Delay example** Cooldown: is the time needed to cast the same skill (doesn't affect other skills, skill specific cooldown).![Delay cooldown 1](.gitbook/assets/Delay_cooldown_1.png) ![Delay cooldown 2](.gitbook/assets/Delay_cooldown_2.png)

**Hard def example**

- 200 HardDEF = 25% damage reduction
- 400 HardDEF = 40% damage reduction
- 20 HardMDEF = 15% damage reduction
- 40 HardMDEF = 25% damage reduction

The effect of HardDEF/MDEF is now reduced exponentially as the number goes up (the higher the number, the less effective it becomes)

### New formula for Stun, Silenced, Cursed

On this server we have also re-write the formula in regards to SCStun (Stun), SC_Silence (Silenced), and SC Curse (Cursed). **Not stone cursed**.

#### **Stun New Formula**

In order to achieve Immunity, there are 4 ways:

- You have to have 100% Resistance from Gears / Cards.
- Total VIT (Base + Additional) Equal or More than 160 -> Immune.
- Total LUK (Base + Additional) Equal or More than 160 -> Immune.
- Total of both Total VIT and Total LUK equal or More than 280 -> Immune.

##### **Important to know**

- Keep in mind that this formula, follows the rule of “Either This or That”. Which means, your resistance gained from Gears (Percentage Resistance) will not play any role with the VIT or LUK (Stats Resistance).
- Total VIT will affect the Durations of the negative statuses (Stun) above.
- Total LUK will affect the Chance of the negative statuses (Stun) being inflicted.

I will give an example, with 159 Total VIT you will get stunned for 0,03 Seconds. (5 Seconds divided by 160, which is Immune). With 159 Total LUK you will reduce the chance of getting stunned. (Stun skill chance percentage reduced by the Total LUK you have). It’s like this, 160 LUK = 100% Immune. For every point of LUK added, it will add Reduction in percentage against negative statuses. LUK = Reduce Chance getting Stun. VIT = Reduce Duration of the Stun.

#### **Silence New Formula**

In order to achieve immunity to Silence negative status, there are many ways actually.

**For Silence:** Instead of Total VIT, it’s your Total INT that’s in play. Both for the Durations and Chances. To achieve immunity; it’s Total INT = 180.

INT = Reduce both the Durations and Chance to get Silenced.

#### **Curse New Formula**

In order to achieve immunity to Curse negative status, also many ways.

**For Curse:** It’s only your Total VIT that’s in play. Both the Durations and Chances. To achieve immunity; it’s Total VIT = 160.

VIT = Reduce both the Durations and Chance to get Cursed.
