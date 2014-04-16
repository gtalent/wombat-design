# World Package

## Types

### Tile
#### Attributes
* tileClass	*TileClass
* sprite		*Sprite

#### Methods
* draw(Graphics *gfx, Point pt)
	* Input:
		* gfx - Graphics context to draw with
		* pt  - where to draw the Tile on screen

### TileClass
#### Attributes
* terrainFlags	uint8
* lowerAnims	AnimLayer[]
* upperAnims	AnimLayer[]
