Polytweak version 2.0 has ten main components. More are in development.

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXXX|/|__Creature Changes__|\|XXXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

1) PNP MIND FLAYER ATTACKS: Several mods (Tactics, Questpack and SCSII) already improve mind flayer scripting and psionic powers, so I don't touch their AI; instead this component changes the behaviour of the mind flayer's "Devour Brain" attack. The vanilla game implementation as as a short duration penalty to the target's intelligence score with each hit was a bit ridiculous, since your character's half-eaten brain grows back in 30 seconds, and highly intelligent characters (presumably having brains toughened by exercise) survive their attacks for longer.

Each hit from a flayer strips 25% of the target's hp to simulate this monster's PnP ability to kill with four successful tentacle hits. Note that this damage cannot "gib" a  character, doesn't bypass stoneskin on grounds of "realism" (some would say this makes fighter/mages overpowered vs mind flayers, I'd say F/Ms are already broken beyond repair) and doesn't affect elementals, slimes, skeletons, wraiths or very large creatures. Fighter NPCs with low-average intelligence such as Minsc are now more viable against illithids.

XP is now gained for kills made while shapechanged into a mind flayer, which also properly sets magic resistance to 90%.

Additionally the THAC0 of most mindflayers is corrected. Ulitharids gain six attacks per round (as they should have) and "Supra-genius" intelligence that allows them to ignore low level illusions. Vampiric illithids are a bit more dangerous since they can devour brains as well as drain levels. The latter critters are recoloured slightly to stand out from regular mind flayers.

Compatibility: This will work best if installed after the g3 fixpack and before SCSII (though SCSII is not required). Installing my mod after SCSII shouldn't break anything, but Alhoon(s) won't be affected in that case.

2) IMPROVED (LESS BUGGY) TROLLS: The behaviour of trolls in the vanilla game (i.e. often "forgetting" to die while in combat and being unable to die while webbed) makes battles with trolls unnecessarily long and full of micromanagement and is a source of frustration to many players including myself. This component allows trolls to be killed directly, providing fire or acid is used, it is somewhat similar to the "Streamlined Trolls" component of Tactics, however unlike Tactics the trolls gain no damage resistance and still require fire or acid damage to be finished off, trolls are also now susceptible to mind affecting spells (they were immune to script-breaking effects like confusion in vanilla BG2, mainly so that their "lie down when near death and become immune to everything except fire/acid" script would function).

Spectral and spirit trolls, being undead creatures get appropriate immunities and may now be turned by paladins or priests. They will not be encountered during the daytime (outside De'Arnise keep or in the druid grove).

Vanilla game spirit trolls had claws which work like the Staff of the Magi, i.e. granting invisibility on equip, this interacts badly with SCS melee scripting because the troll "equips" their claws before attacking (and thus becomes invisible) several times per round. Their invisibility is now applied by script and less frequently, they also drain more strength per hit, but only by their claws (not their bite) and for a shorter time.

Add this as late as possible in the installation order.

3) IMPROVED UMBER HULKS: These beasts receive a number of stat fixes, they had fewer HD than they should in vanilla (6 rather than 8+8) and their saving throws were too high. Their AI scripting is improved (an Umber Hulk is supposed to have 8-10 intelligence, equivalent to an average human), although their gaze attack is intentionally random (it's supposed to affect anyone who happens to make eye contact, nearby characters are the most likely). Umber Hulk claw/bite attacks are now coded correctly as slashing weapons.

Elder umber hulks now have a tougher save penalty against their confusing gaze, and their claws cause bleeding wounds. The random monster spawns of umber hulks now have one elder umber hulk leading them rather than a minotaur.

Install order shouldn't matter too much here, as few mods touch umber hulks, but ideally last and certainly after Quest Pack.

4) IMPROVED YUAN-TI: The snake men had a variety of spell like abilities in 2nd edition (cause fear, poison, darkness and suggestion), which weren't implemented in game, these are restored. Being a highly intelligent race Yuan-Ti also have a chance to wield magical swords or axes and lesser Yuan-Ti now have proficiency in their weapons. The XP awards for defeating Yuan-Ti are increased a little.

This component does not affect Yuan-Ti mages whose AI is already improved by various mods, it should be installed after SCS otherwise my changes to Yuan-Ti scripts may interact badly with SCS scripting.

5) IMPROVED MINOTAURS: Most were weak creatures in the vanilla game (they're still not very tough), their movement rate, HD and morale are fixed to match their MM descriptions and they gain the ability to charge targets who aren't yet in close combat; a minotaur's charge deals crushing damage with a chance of knocking the target down if a save vs death is failed, charging minotaurs also take double damage if struck by a piercing weapon (excepting missiles).

6) CORRECTED VAMPIRE STATS: As with the mind flayers (and for the same reason) I haven't touched vampire AI, this component just matches vampire XP values, physical stats and saving throws to their level. All vampires except fledglings gain a little magic resistance. Vampires without names are now labelled according to their level of power, which seems to have been intended but unimplemented in game.

More powerful varieties of vampire impose a greater saving throw penalty against their charming gaze. Vampire fear also now applies a -2 penalty to all of a victim's dice rolls (rather than just THAC0) if the save is failed, and doesn't stack with itself (as it used to).

Durst and Gellal, the special vampires the party may meet in Bodhi's lair in Chapter 2 get a level boost to match their vanilla XP values, as does Lassal.

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXX|/|__NPC and rule Changes__|\|XXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

1) RELATED WEAPON PROFICIENCIES: I always thought it strange that a grandmaster of the longsword would fumble with a bastard sword, or that a crack shot with a longbow would be unable to hit the side of a barn with a short bow.

Polytweak RWPs groups similar weapons together: Long swords and bastard swords; scimitars and katanas; clubs and maces (...depending on install choice); shortbows and longbows. Specialization in a weapon type automatically grants proficienct use of similar weapons (however class restrictions are respected i.e. fighter druids can't get proficiency in katana or mace nor can swashbucklers get proficiency in bastard sword), likewise high mastery of a weapon imparts specialization in all "relatives".

You will need to turn party AI on for a couple of seconds after joining a new NPC or allocating their proficiencies in order for this component to work, as the changes are applied by script.

This component should be compatible with "Rebalanced Weapon Proficiencies" from BG2 Tweak Pack.

2) NPC IMPROVEMENTS FOR SOA: I find it frustrating on the nth replay recruiting NPCs who have useless spells memorized and - worse - mispent proficiencies. Admittedly it only takes one rest to refresh their spell slots but NPC's have time-limited quests and if you play with tactical mods (like me) you can easily find yourself running out of time.

You'll be asked about each NPC:

Anomen: More useful spells memorized and specialized in warhammer and flail, if you recruit him at level 12+ he will have mastered flails.

Cernd: Kit changed to avenger, stats reallocated - though stat point total is left the same - to 12, 16, 9, 10, 18, 15 (previously 13, 9, 13, 12, 18, 15 - he was the only NPC without a single good physical stat!).

Jaheira: Better spell choice and either
          i) Specialized in quaterstaff and sling, with one star in two handed style and spears
	  ii) Specialized in scimitar, dagger and two weapon style

Keldorn: Gains halberd and two handed proficiency or specialization (depending on level)

Minsc: i) Keep Minsc as a ranger but give him specialization in bastard sword rather than two handed sword and an extra star in two weapon fighting
        ii) Change Minsc to a barbarian but keep vanilla game proficiencies (except two weapon style)
        iii) Change Minsc to a barbarian specialized in two weapon, axes and bastard swords

Minsc receives an appropriate hp boost with either "barbarian" option.

Nalia: Most players think of her as a less useful Imoen clone, I’ve tried to make her more distinctive; now swashbuckler 5 -> mage (slightly less XP on joining).

Valygar: Racial enemy changed to demon (a THAC0 bonus vs golems is almost useless as they have poor AC), gains an extra star in two weapon fighting, specialization in long sword rather than spear and in short bow rather than long bow (he doesn't have sufficent strength to use the "best" longbows... which are a pretty useless weapon category anyway).

Viconia: Largely empty spellbook filled

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXX|/|__Items and Icons__|\|XXXXXXXXXXXXXXXXXXXXXX
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

1) DISTINCTIVE ICONS FOR BLACKRAZOR & fLAMETONGUE: Blackrazor looked a lot like Haer'Dalis's Chaos sword (it's blade is supposed to resemble the night sky) and Flametongue shared an icon with the sword of flame (it now has a wavy, flamberege design).

2) PNP DISTUPTION WEAPONS: Disruption weapons in unmodded BG2 were rather overpowered versus undead, because the chance of disruption was implemented as a saving throw with a -4 penalty, meaning even the highest level vampires and liches were almost guaranteed to be disrupted in a round if assaulted by someone with multiple attacks. Disruption weapons now use the following table:

HD of undead____________________Chance of Disruption

6 (such as wraiths) or less_____95%_________________
7 (such as mummies)_____________80%_________________
8 (such as spectres)____________65%_________________
9 (such as fledgling vampires)__50%_________________
10 (such as ghosts)_____________35%_________________
11 (such as basic liches)_______20%_________________
12 or more______________________5%__________________

On the other hand, evil extraplanar creatures like demons and rakshasas are also now affected by disruption weapons, suffering extra magic damage with each hit and a chance of destruction as if they were 12+ HD undead.

This component affects Azuredge and of course the Mace of Disruption (both versions), which gets a new icon. The price of Azuredge is also increased to 10,000 gp.

************************************************

Acknowledgements: 
Westley Weimer and Valerio Biggiani for Weidu 
aVENGER for his similar PnP creatures components in aTweaks (a partial inspiration for this mod)
Avenger_teambg for DLTCEP
Kreso for playtesting and bug reports
And of course Bioware and Black Isle for making the games in the first place