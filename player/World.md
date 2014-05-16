## World Package

#### Description
The World package needs to be able to handle the world, giving the user an overhead view of a tile based environment.

#### Types

* CreatueSpawn
	* Attributes
		* spawnChance	uint8  # % chance chance creature will spawn
		* creature		string # path to creature

* TileInstance
	* Attributes
		* tileClass	*Tile
		* occupant	*Sprite
	* Methods
		* draw(Graphics *gfx, Point pt)
			* Input:
				* gfx	- Graphics context to draw with
				* pt	- where to draw the TileInstance on screen

* Tile
	* Attributes
		* terrainType	uint8
			* Values:
				* 0 - Land
				* 1 - Water
				* 2 - Whirlpool
				* 3 - Waterfall
		* upperAnim		AnimLayer
		* lowerAnim		AnimLayer
		* spawn			[]CreatureSpawn

* Zone
	* Extends: core package's Task
	* Attributes
		* zoneClass	*ZoneClass
		* location	Point
		* loaded		bool
	* Methods
		* run() int64 

* ZoneClass
	* Attributes
		* tiles [][][]TileInstance
