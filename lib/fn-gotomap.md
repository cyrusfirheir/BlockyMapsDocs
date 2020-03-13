
`setup.bm.gotoMap(mapObj)`

Loads and goes to the `bmPlayMap` passage to display a map. Adds a moment to the history.

**Since:**
- `v1.0.0`

**Parameters:**
- `mapObj` : (*object* | *string*) A valid JSON string or a JavaScript object containing valid map data. *See [Map Object Template](../lib/map-obj.md) for more details.*

**Example:**
```js
// the quickest way to load and run a map in a project
// (in JavaScript)
var mapObj = {/* the actual object */};
setup.bm.loadMap(mapObj);
```
