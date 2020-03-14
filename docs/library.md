
# The Library

As mentioned earlier, map data is handled as a JSON object, and this allows for a lot of flexibility in regards to management of multiple maps.

The simplest map object might look something like this (*See [The Map object](library?id=mapobj) for more details*):

```js
const mapObj = {
	id: "uniqueMapID",
	size: {
		rows: 3,
		cols: 3
	},
	zoom: 1,
	r1c1: {
		cssClass: "player"
	}
};
```

Global Twine variables currently used by the library:  
- `$curMap` : (*object*) Map object which is currently being displayed.  
- `$curPos` : (*string*) Position of the player on the map.

## Functions

?> All library functions are under the `setup.bm` namespace.  

---
[gotoMap](./library/functions/gotoMap.md ':include type=markdown')

---
[pMove](./library/functions/pMove.md ':include type=markdown')

---
[pMoveCoords()](./library/functions/pMoveCoords.md ':include type=markdown')

---
[cameraFollow()](./library/functions/cameraFollow.md ':include type=markdown')

---
[mapZoom()](./library/functions/mapZoom.md ':include type=markdown')

---
[drawMap()](./library/functions/drawMap.md ':include type=markdown')

---
[The Map object](./library/mapObj.md ':include type=markdown')

---
[The UI](./library/ui.md ':include type=markdown')

---
[The Markup](./library/markup.md ':include type=markdown')
