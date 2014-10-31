Universal Sheet System
For Use With
Unisystem CG System
By Gizmo
GNU Public License
------------------
An attempt at a Universal +sheet for the games in my unisystem cg

1) How this works

	It's a +sheet that should theoretically work with any of the games in the unisystem CG.
	You might have to make minor modifications. Those can be added however. If you add them,
	I would appreciate if you let me know at ccubed.techno@gmail.com so I can add them
	to the github for other people! Or if you have a github, then ask to pull and I'll
	accept! Put them in a separate folder in the Universal Sheet Folder as a mod under
	the specific game it's for.
	
2) Steps

	A) Install Universal Sheet
	B) Set Display-Stats and display types
	B2) Example: Attributes~2 Skills~2 Merits~3 Disciplines~2 Archetypes~1
	
3) What Happens

	Essentially. The sheet supports some basic demographic information by default.
	Name, Age, Date of Birth, Concept.
	Then it goes through each stat type in Display Stats. If the PC has it on
	them then it displays all the individual stats in that category.
	That's it.

4) Display Types?

	1 - Only show the names
	2 - Show names, levels (no notes, even if present)
	3 - Show names, Levels and notes if present
	
5) How do I set display-stats?

	&Display-Stats <dbref sheet object>=List of stats spelled as they are on the library object and their view types, see example
	
6) Display Order
	
	Display order is the order in which the stats are in display-stats. So if you do Attributes Skills, the display order would
	be Attributes and then Skills. If you do skills attributes then it would be Skills and then Attributes.
	
7) Changing

	Everything is modular so it should be easy to move things around. Specs can easily be moved wherever as it's a single function
	at the end with a single formatter. This will probably eventually break the buffer, but then, so does any sheet anywhere given 
	enough time and player xp accrual.