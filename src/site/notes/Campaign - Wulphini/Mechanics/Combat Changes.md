---
{"dg-publish":true,"permalink":"/campaign-wulphini/mechanics/combat-changes/","created":"2026-02-12T16:12:44.940-05:00","updated":"2026-02-12T19:16:11.060-05:00"}
---


# Weapon Changes

> [!infobox|ws-med]+
> 
> ![Pasted image 20260212162212.png](/img/user/_meta/_attachments/Pasted%20image%2020260212162212.png)

The basic formula for calculating weapon damage and armor penetration remains the same.

*Magnitude*, *Damage*, *Accuracy*, *Penetration* are all unchanged.

==Damage Ratings==. The "Phys" damage type has been split into *Puncture* and *Impact*.  *Shock* damage is now the default damage type.  Any damage this isn't *Thermal*, *Puncture*, or *Impact* is counted as *Shock* damage.  As before, the weapon's listed damage ratings cannot sum to more than 10.  This rating translates into the percentage of the weapon's damage that is treated as that damage type.  In this example 30% of its damage is *Puncture* and 70% is *Impact*.

==Lethality==.  The rating is a value of 1 - 10 and translates into the percentage of the weapon's damage that counted towards calculating the severity of injuries inflicted.

==MoS Die==.  This is the die used to roll added damage from margins.  This might not be used by players but its something I've wanted the ability to change for certain environmental effects.

#### Tech Points and Firmware

The five Firmware types are labeled as αPen, βPen, αDmg, βDmg, and Precision.  The darkened fields above the labels are the level of the Firmware installed on the weapon, and the white fields underneath are the number of tech points currently assigned to each Firmware.

==Firmware==. Weapons in this era are smart enough to have their performance configured, on the fly as a Muse action.  The quality, or Level, of the Firmware dictates exactly how much the performance changes.  The higher the level, the more impact that Firmware has per Tech Point.  In this example you can see that the weapon has a Level 2 beta-Penetration (βPen), and a Level 1 beta-Damage (βDmg) installed.

==Tech Points==. Weapons that have a total Tech Point stat shown next to Blast and under Lethality.  This is the total number of points that can be distributed between Firmware.  In this example, you can see the weapon has 4 Tech Points.  You could put all 4 in βPen or βDmg, 2 in each, or however you like, as long as the total less than or equal to the weapon's Tech Point total.

Assigning Tech Points to a Firmware multiplies the Level of that Firmware.  In this example, putting 2 Tech Points each into βPen and βDmg means the next attack is augmented with the effects of Level 4 βPen, Level 2 βDmg, and Level 0 in all others.

###### Firmware Types
==Alpha-Penetration (αPen)== Increases the global chance to penetrate armor. 
> [!hint]- Math
> When Weapon Magnitude and Armor Magnitude are equal, there is a base 50% chance to penetrate Layer 1.  As Weapon Magnitude rises above Armor Magnitude, this penetration chance rises, and vice versa. The weapon's Penetration stat is added to its Weapon Magnitude when making this comparison.  
> 
> αPen increases the base chance by 4% per TP at Level 1 and 10% per TP at Level 6.

==Beta-Penetration (βPen)== Increases the chance to penetrate armor layers past the first layer. 
> [!hint]- Math
> When damage passes through an armor layer, its penetration is reduced by 50% for the next layer.
> 
> βPen increases this chance by 4% per TP at Level 1 and 6% per TP at Level 4

==Alpha-Damage (αDmg)== Increases the raw damage gained from Weapon Magnitude. 
> [!hint]- Math
> When Weapon Magnitude and Armor Magnitude are equal, the raw damage is equal to the lists Damage stat of the weapon.  As Weapon Magnitude rises above Armor Magnitude, this damage value rises, and vice versa. 
> 
> αDmg increases the raw damage from Magnitude by 10% per TP at Level 1 and 25% per TP at Level 5.

==Beta-Damage (βDmg)== Increases the damage added by Margins of Success from the Attack Roll. 
> [!hint]- Math
> Each MoS of an Attack roll adds one roll of the weapon's Margin Die to its initial raw damage (before Magnitude adjustment).
> 
> βDmg adds 0.4 damage per MoS per TP at Level 1 and 1.0 damage per MoS per TP at Level 6.  These values were chosen to make αDmg and βDmg roughly equal in power for 3 MoS Attacks. At lower margins, αDmg is slightly more efficient, but at 4 MoS, βDmg adds about 25% more damage than αDmg would.

==Precision== Reduces the target value of your attack roll to gain a bonus to the attack roll.  Highly skilled combatants can use this Firmware to trade some of there "wasted" accuracy to improve the odds are rolling higher margins.
> [!hint] Math (WIP)

# Damage Types and Weapon Tech
The following is a general guideline for how certain weapon technologies are represented in damage types.  Specific weapons may have slightly different values.

|Tech     |      | Thermal | Puncture | Impact | Shock |
| ---     | ---  | ---     | ---      | ---    | ---   |
|Laser    |      |    7    |     3    |       |      |
|         |Beam  |    7    |     *s*    |       |   3   |
|Coil     |      |    3    |     7    |       |      |
|       |Magwave |    *s*    |     7    |       |   3   |
|Slug/Bullet |   |        |     3    |    7   |      |
|   | Pellet/Bag |        |     *s*    |    7   |   3   |
|Sabot/Flechette |  |     |     7    |    3   |      |
|Plasma    |      |    7    |         |    3   |      |
|Percussion    |      |    3    |         |   7   |      |
|    | Compression    |    3   |         |    *s*   |   7   |
|    |      |       |         |       |      |
|Blast    |      |        |     5    |    5   |      |
|Fission  |      |    5    |     5    |       |      |
|Lance    |      |    5    |         |    5   |     |
|    |      |       |         |       |      |
|Kelvinic    |      |    10    |        |       |      |
|Sheer  |      |        |     10    |       |      |
|Sonic/Seismic    |      |        |         |    10   |      |
|Shock    |      |        |         |       |   10   |

# Armor Changes
The only change to armor is that Protection has been split into values for each Damage Type, and for each layer.

# Injury Changes
Injury categories will change to 4 types: Minor, Serious, Major, Deadly.  Each has its own Condition penalty.  Your total Condition modifier is the sum of the penalties of the injuries you have.

Injury category is no longer based on a morph's Resistance.  They now have a fixed damage value.  Only a portion of actual damage dealt is counted towards this threshold, as listed by the weapons Lethality rating.

| Injury Type | Damage Threshold | Condition |
| --- | --- | --- |
| Minor | 15 - 29 | +2 |
| Serious | 30 - 44 | +5 |
| Major | 45 - 59 | +12 |
| Deadly | 60+ | +30 |

You can have 3 of each type of Injury except Deadly.  A 3rd Deadly is Body Death.  If you have 3 Injuries of a category and receive another of that category, you instead take an injury of the next higher category.  When you heal an injury it becomes 2 Injuries of the category below.

==Deadly Injuries== A deadly injury will eventually lead to body death if left untreated.  When a Deadly is received, roll 1d100 + 1d20 to find the number of minutes you have to get treated.  This creates a nice "up to 2 hours" timer with a slight bias away from very, very low rolls.

###### Resistance
A morph's Resistance stat will be converted into a skill-like stat.  When you receive an injury, your Resistance will be rolled like a skill check.  If you fail this check, you gain an injury as listed.  If you succeed the Resistance Check, the injury is reduced by 1 category per MoS to a minimum of Minor.

Resistance will be skill-like but not a skill.  You can't spend rez on it, use Luck, get assists, nor Learning Opportunities.  You can augment it with morph augments and traits.

| Morph Type | Resistance |
| --- | --- |
| Birth | 25 - 35 |
| Standard Bio | 30 - 40 |
| Premium Bio | 40 - 50 |
|Pinnacle Bio | 50 - 60 |
| Standard Synth | 40 - 50 |
| Premium Synth | 50 - 60 |
| Pinnacle Synth | 60 - 70 |
|Biotech | 90 |

Overall this should be a slight nerf to top end morphs, and a buff to lower end morphs.



