
### drawMap() :id=fn-drawmap

`setup.bm.drawMap(mapObj)` → *string*

Returns a string of html to be displayed on a passage. *Usually,* this function is not needed to be used directly, as the drawing to a passage is already handled entirely by the [`gotoMap()`](library?id=fn-gotomap) function. (*See [The Markup](library?id=markup) for more details.*)

**Since:**
- `v1.0.0`

**Parameters:**
- `mapObj` : (*object* | *string*) A valid JSON string or a JavaScript object containing valid map data. (*See [The Map object](library?id=mapobj) for more details.*)

**Returns:**
- (*string*) SugarCube + HTML markup to be rendered to the page.

**Example:**
```js
// returns a html string needed to draw the map stored as JSON in the 'forest-map' passage
setup.bm.drawMap(Story.get("forest-map").text);
```
