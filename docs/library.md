
## The Library {docsify-ignore}

As mentioned earlier, map data is handled as a JSON object, and this allows for a lot of flexibility in regards to management of multiple maps.

The simplest map object might look something like this (*See [The Map object](library?id=the-map-object) for more details*):

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

?> **NOTE:**  
All library functions are under the `setup.bm` namespace.  

---

### gotoMap()
[gotoMap](lib/gotoMap.md ':include')

---

### pMove()
[pMove](lib/pMove.md ':include')

---

### pMoveCoords()
[pMoveCoords()](lib/pMoveCoords.md ':include')

---

### cameraFollow()
[cameraFollow()](lib/cameraFollow.md ':include')

---

### mapZoom()
[mapZoom()](lib/mapZoom.md ':include')

---

### drawMap()
[drawMap()](lib/drawMap.md ':include')

---

[The Map object](lib/mapObj.md ':include')
