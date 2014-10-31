Unisystem CG by Gizmo
GNU Public License
------------------
Various softcoded character generation systems.

1) How this works

	It's a unisystem base Database with various dropins that specialize the database 
	for the specific system you want it to run.
	
2) Steps

	A) Install Library.txt

	B) Install your Dropin
	
3) Old Folders

	Ignore anything not Unisystem CG. The other folders are old systems I was making. 
	I only keep them around because they have large amounts of pretyped data. 
	Especially in the case of L5R, it's not attractive to retype all the things that I would need to. 

4) Specialties

	If your system uses specialties, then make sure you also install the contents
	of the specialtymod text file after running the library setup file.
	
5) How are things stored

	All the information is on the library. The library controller has the functions
	and commands for interacting with that information. The stats are set on the
	players in a consistent way with the following format with all spaces
	replaced by an underscore:
		Player->Stat Category - Individual listing of skills separated by |
		Player->Stat Category.SPECS - Specialties
		
	Stats are listed in this format.
		Name~Level~Note
		Skill~Spec
		
	
5) Commands

	Add a specialty to a player
	+stat/set player/type=specialty:whatever.specialty name
	
	Add a stat to a player (note is optional)
	+stat/set player/type=name:level/note
	
	Remove a specialty from a player
	+stat/set player/type=!specialty:whatever.specialty name
	
	Remove a stat from a player
	+stat/set player/type=!name:level/note
	
	Add a new stat type or category
	+stat/addtype Name
	
	Add a new stat to a type/category
	+stat/add type=name of stat
	
	Add a new stat to a type/category (Extended)
	+stat/addex type=name/levels
	
	Remove a stat from a category
	+stat/rem type=name
	
	Add descriptor text to a stat (Supports formatting)
	+stat/desc type/name=description
	
	View a descriptor for stat
	+stat/view type/name
	
	List all types
	+stat/list
	
	List all stats in a specific category
	+stat/list type
	
	Set display method to single or dual for type
	+stat/display type=SINGLE|DUAL
	
6) What is this display method thing?

	In single mode, the stats will simple be listed side by side as their names.
	In dual mode, it will list the stats and then their levels out to the side.
	