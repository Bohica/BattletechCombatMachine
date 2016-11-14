# Battletech Combat Machine
<b>BattleTech</b> is a wargaming and science fiction franchise launched by FASA Corporation in 1984, acquired by WizKids in 2000, and owned since 2003 by Topps. The series began with FASA's debut of the board game BattleTech (originally named BattleDroids) by Jordan Weisman and L. Ross Babcock III and has since grown to include numerous expansions to the original game, several computer and video games, a collectible card game, a series of more than 100 novels, an animated television series and more.

===========

This project focuses on combat assisting tools for Battletech table top miniatures.  It automates and streamlines various parts of gameplay in an effort to assist in eliminating the minutia of calculating modifiers, executing weapons fire and damage generation, tracking heat, etc... in an effort to speed up gameplay. 

A game consists of a series of turns. During each turn, all Units on the map have an opportunity to move and  fire their weapons or make physical attacks. Each turn consists of several smaller segments of time, called phases. During each phase, players may take one type of action, such as movement or combat. The players execute the phases in a given order. Specific actions, movement, e ects of damage and so on are fully explained in separate sections later in these rules.

<b>Functionality to support</b> (expanded design details for each below):

1. Initiative Phase
2. Movement Phase (Ground)
3. Movement Phase (Aerospace)
4. Weapon Attack Phase
5. Physical Attack Phase
6. Heat Phase
7. End Phase

===========

### INITIATIVE PHASE
Each player rolls 2D6 and adds the results together to deter- mine his or her Initiative; re-roll ties. The player with the higher result is the Initiative Winner. The other player is the Initiative Loser for this turn.

* Roll the 2D6
* Store the roll in the DB for the turn
* Accumulate intiative rolls for all the players on that side
* If the sides differ in number of players, apply extra 2D6 rolls to balance the rolls
* Archive the accumulted initiative rolls for the sides

===========

### MOVEMENT PHASE (GROUND)
The team that lost Initiative chooses one ground unit (non- aerospace; this includes VTOLs) and moves it  rst. If this team has more ground units than the team that won Initiative, it may need to move more than one ground unit, as described in Unequal Numbers of Units, p. 39.

The team that won Initiative then moves one ground unit. If this team has more ground units than the team that lost Initiative, it may need to move more than one ground unit (see Unequal Numbers of Units).

Movement alternates between sides until all ground units have been moved. Each time a player must move a ground unit, he may designate movement for any ground unit that has not been destroyed, even if a unit is completely immobile, as long as it is not destroyed it can still be given a “move” action, and it will remain in its hex. For example, units whose warriors are unconscious are not destroyed and can be designated to remain immobile.




