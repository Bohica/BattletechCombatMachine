# Battletech Combat Machine
<b>BattleTech</b> is a wargaming and science fiction franchise launched by FASA Corporation in 1984, acquired by WizKids in 2000, and owned since 2003 by Topps. The series began with FASA's debut of the board game BattleTech (originally named BattleDroids) by Jordan Weisman and L. Ross Babcock III and has since grown to include numerous expansions to the original game, several computer and video games, a collectible card game, a series of more than 100 novels, an animated television series and more.

===========

This project focuses on combat assisting tools for Battletech table top miniatures.  It automates and streamlines various parts of gameplay in an effort to assist in eliminating the minutia of calculating modifiers, executing weapons fire and damage generation, tracking heat, etc... in an effort to speed up gameplay. 

A game consists of a series of turns. During each turn, all Units on the map have an opportunity to move and  fire their weapons or make physical attacks. Each turn consists of several smaller segments of time, called phases. During each phase, players may take one type of action, such as movement or combat. The players execute the phases in a given order. Specific actions, movement, e ects of damage and so on are fully explained in separate sections later in these rules.

<b>Functionality to support</b> (expanded design details for each below):

* Player Managemnt
* Pilots
* Units
* Team Management
* Missions

1. Initiative Phase
2. Movement Phase (Ground)
3. Movement Phase (Aerospace)
4. Weapon Attack Phase
5. Physical Attack Phase
6. Heat Phase
7. End Phase

===========

### PLAYER MANAGEMENT - NYD
Each participant in a match will have several units to manage.

1. Register an account for use in tracking a variety of information
2. Pilots
3. Units
4. Missions participated in and their associated data

===========

### PILOTS - NYD
A player can have multiple pilots with varying attributes

1.

===========

### UNITS - NYD
A player can have multiple units

1.

===========

### TEAM MANAGEMENT - NYD
Each match will consist of 1 or more players allied with each other

1. Register a team for use in tracking a variety of information
2. Add players
3. Missions

===========

### MISSIONS - NYD
A mission will include multiple teams and maps out the turns taken during a match

1. Description and other criteria defining the match
2. Add teams
3. Add players if they are not part of a team
4. Track all turns in the match
5. Outcome
6. AAR

===========

### INITIATIVE PHASE - NYD
Each player rolls 2D6 and adds the results together to deter- mine his or her Initiative; re-roll ties. The player with the higher result is the Initiative Winner. The other player is the Initiative Loser for this turn.

* Roll the 2D6
* Store the roll in the DB for the turn
* Accumulate intiative rolls for all the players on that side
* If the sides differ in number of players, apply extra 2D6 rolls to balance the rolls
* Archive the accumulted initiative rolls for the sides

===========

### MOVEMENT PHASE (GROUND) - NYD
The team that lost Initiative chooses one ground unit (non- aerospace; this includes VTOLs) and moves it  rst. If this team has more ground units than the team that won Initiative, it may need to move more than one ground unit, as described in Unequal Numbers of Units, p. 39. Units include hover-craft, naval vessels, tracked vehicles, VTOLs, wheeled vehicles, and WiGEs.

<b>UNEQUAL NUMBERS OF UNITS</b>
Phases require each player to alternate moving or declaring attacks with his or her units. When both sides have an equal number of units, each player simply takes a turn moving or declaring a single unit’s action, then the other player declares movement or an action for one unit, and so on. If the number of units on each side is not equal, however, this procedure must be altered.

If, prior to any pair of movement or attack declarations, one team has at least twice as many units left to declare for as the other team, the team with twice as many units declares for two units rather than one. If one team has at least three times as many units, it declares for three each time, and so on.
See the example below for how to handle unequal numbers of units.


The team that won Initiative then moves one ground unit. If this team has more ground units than the team that lost Initiative, it may need to move more than one ground unit (see Unequal Numbers of Units).

Movement alternates between sides until all ground units have been moved. Each time a player must move a ground unit, he may designate movement for any ground unit that has not been destroyed, even if a unit is completely immobile, as long as it is not destroyed it can still be given a “move” action, and it will remain in its hex. For example, units whose warriors are unconscious are not destroyed and can be designated to remain immobile.

1.

===========

### MOVEMENT PHASE (AEROSPACE) - NYD
The team that lost Initiative chooses one aerospace (non- ground) unit and moves it first. If this team has more aerospace units than the team that won, it may need to move more than one aerospace unit (see Unequal Numbers of Units). Units include Aerospace Fighters, Air- ships, Conventional Fighters, DropShips, Fixed-Wing Support Elements and Small Craft.

The team that won Initiative then moves one aerospace unit. If this team has more aerospace units than the team that lost, it may need to move more than one aerospace unit.

Movement alternates between sides until all aerospace units have been moved. Each time a player must move an aerospace unit, he may designate movement for any aerospace unit that has not been destroyed, even if the move is to expend no thrust. Aerospace units whose warriors are unconscious are not destroyed and can be designated to expend no thrust, even if the unit is currently out of control; see Out-of-Control E ects, p. 93.

Any aerospace units that are grounded or that crashed but survived are considered a ground unit. Players may move them during the Movement Phase (Ground).

1.

===========

### WEAPON ATTACK PHASE - NYD
The team that lost Initiative chooses a unit (ground or aerospace) to declare  re  rst. If this team has more units than the team that won Initiative, the players may need to declare attacks for more than one unit as described in Unequal Numbers of Units, p. 39. The player controlling the  ring unit declares whether it will twist its torso or  ip its arms or turn its turret, and in which direction. He must declare any attacks he plans to make using his unit’s weapons—or the type of attack in the case of aerospace units—specifying which weapons he will  re and at what target(s). If a weapon uses special ammo loads, such as LB-X cluster munitions, or can make special types of attacks, such as double- ring an Ultra autocannon, or can produce any other unusual e ects, the player must declare those e ects at this time.

The team that won Initiative then chooses a unit (ground or aerospace) to declare  re. If this team has more units than the team that lost Initiative, the players may be required to declare attacks for more than one unit (see Unequal Numbers of Units). The player controlling the  ring unit declares any torso or turret twists and attacks he plans to make using that unit’s weapons, as described above.

The act of declaring attacks alternates between players until all  re has been declared. Each time a player must declare an attack, he may do so for any unit that has not been destroyed, even if the declaration is to make no attack.

<b>Torso/Turret Twist</b>
Torso or turret twists are made when declaring a weapon attack, but the torso or turret remains pointed in the same direction throughout the remainder of the turn. This a ects physical attack  ring arcs as well; the torso or turret returns to its forward-facing position during the End Phase (see below).

<b>Resolving Weapons Fire</b>
Players resolve weapons  re one unit at a time. The order in which each unit’s successful attacks are resolved is up to that unit’s controlling player. All weapons attacks by one unit should be resolved before those of the next unit in order for the players to more easily track which weapons have  red.

All declared attacks must be made, even if the intended target is destroyed before all attacks against it have been resolved. Also, players must resolve all declared weapons  re for the purpose of tracking ammunition and heat. In addition, players may not change an attack declaration once made, as the time-scale (and the general confusion of battle) makes it impossible to do other than follow through with a declared attack.

<b>Determining Damage</b>
Damage from weapon attacks takes e ect next. Players record damage as attacks are resolved, but this damage does not a ect the unit’s ability to attack during this phase. This means a unit may make its declared attacks in the same phase even if that unit or its weapons are destroyed.

At the end of the phase, all damage takes e ect immediately. Players must make any Piloting Skill Rolls and/or Control Rolls required according to the e ects of weapon attacks. Damage taken by a unit during the Weapon Attack Phase takes e ect before the start of the same turn’s Physical Attack Phase. As needed, Piloting Skill Rolls, Control Rolls and Consciousness Rolls may be required at the end of the Weapon Attack Phase.

Note that even though damage does not take e ect until the end of the phase, destroyed sections take e ect immediately for the purposes of assigning damage. For example, if a ’Mech’s torso is destroyed during the Weapon Attack Phase, the appropriate arm falls o  immediately, and so any other damage in the same Weapon Attack Phase that strikes the arm automatically transfers.

1.

===========

### PHYSICAL ATTACK PHASE - NYD
Players repeat the steps given for the Weapon Attack Phase, with all damage from physical attacks taking e ect before the Heat Phase. As needed, Piloting Skill rolls, Control rolls and Consciousness rolls may be required at the end of the Physical Attack Phase.

1.

===========

### HEAT PHASE - NYD
Players adjust their units’ heat scales for units that track heat, to re ect any heat built up or lost during the turn. Resolve any temporary or permanent damage caused by excessive internal heat at this time. Heat e ects may also damage a warrior, resulting in a Consciousness roll (see p. 41).

ProtoMechs, infantry, and Combat and Support Vehicles do not keep track of heat. See Heat, p. 158, for speci c rules regarding such units during this phase.

1.

===========

### END PHASE - NYD
Players whose warriors were unconscious during the Initiative Phase of this turn now roll 2D6 to see if the pilot regained consciousness during this turn. Players may also execute any miscellaneous actions remaining in the turn, such as switching heat sinks on or o . The speci c rules for such actions state whether or not they take place during the End Phase.

Players repeat all the steps given above until one team meets its victory conditions for the scenario. Under normal circumstances, the team with the last surviving unit(s) left on the map wins. If the last units from each team are destroyed simultaneously in the same turn, or if the last units from each team cannot move and have no ability to damage one another, the game is a draw. The players may set other victory conditions by mutual agreement before play begins or by using the victory conditions given in a FanPro (or FASA) published scenario. See Creating Scenarios, page 256, for guidelines on setting up unique scenarios.

Torso/Turret Twist: Torsos and turrets that were turned or twisted return to a forward-facing position during the End Phase. Turrets jammed by damage (see Ground Combat Vehicle Critical Hit E ects, p. 193) do not return to a forward-facing position, but remain in their current facing for the remainder of the game. BattleMech torsos cannot be jammed in this fashion.

1.






