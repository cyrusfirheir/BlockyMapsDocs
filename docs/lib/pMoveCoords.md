
`setup.bm.pMoveCoords(coords [, override])`

Moves the `player` CSS class across the map to the specified coordinates, and optionally, even to `solid` CSS class blocks, which the player isn't supposed to be able to move through otherwise.

Focuses the camera on the player.

**Since:**
- `v1.0.0`

**Parameters:**
- `coords` : (*string* | *array* | *object*) The coordinates where to move the player. Accepts three kinds of input:  
```
As a string with the format "r{Row}c{Column}":  
	e.g. - "r0c0"  
As an array with the format [row, column]:  
	e.g. - [0, 2]  
As an object with the format {row: row, col: column}:  
	e.g. - {row: 2, col: 3}
```
- `override` : (optional, *boolean*) Whether to override normal behavior and move the player into a solid block. Defaults to false.

**Example:**
```js
// using a string
setup.bm.pMoveCoords("r0c0");

//using an array
setup.bm.pMoveCoords([0, 2]);

//using an object
setup.bm.pMoveCoords({
	row: 2,
	col: 3
});
```
