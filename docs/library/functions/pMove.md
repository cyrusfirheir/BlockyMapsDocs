
### pMove() :id=fn-pmove

`setup.bm.pMove(dir [, dist])`

Moves the `player` CSS class across the map in the specified direction, and optionally, by the specified amount of blocks. Focuses the camera on the player.

**Since:**
- `v1.0.0`

**Parameters:**
- `dir` : (*string*) The direction of movement (either one of `"up"`, `"left"`, `"right"`, or `"down"`).
- `dist` : (optional, *non-negative integer*) The amount of blocks to move in specified direction. Default to 1.

**Example:**
```js
// moves a block to the left
setup.bm.pMove("left");

// creates a link which causes the player to move two blocks down
// (in SugarCube)
<<link "Run South">>
	<<run setup.bm.pMove("down", 2);
<</link>>
```
