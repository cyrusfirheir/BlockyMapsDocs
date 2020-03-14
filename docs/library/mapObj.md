
## The Map object :id=mapobj
*(This section is a work in progress)*

A typical map-object is structured in the following manner:

```js
const mySpeshlMap = {
	id: "mySpeshlMap",
	size: {
		rows: 7,
		cols: 9
	},
	zoom: 80,
	cssClass: "winter night",
	r4c2: {
		name: "The Speshlest part of Speshl district",
		desc: "This is the most coveted place in the entire universe yes!",
		content: "<img src='media/allStar.png'>"
		acts: "<<link 'Stay'>><</link>>"
	},
	/* ... */
	_default: {
		name: "The Speshl district",
		desc: "This is the Speshl district, consisting of marvelous occupants, yes!",
		content: "<img src='media/noQuestionsAsked.png'>",
		cssClass: "ground",
		acts: "<<link 'Good for nothing'>><</link>>"
	}
};
```

- `id` : (optional, *string*) An identifier which doesn't serve any purpose for the library or its functions itself, but can be useful for keeping track of multiple maps.
- `size` : (*object*) The dimensions of the map.
	- `rows` : (*positive integer*) The number of rows in the map.
	- `cols` : (*positive integer*) The number of columns in the map.
- `zoom` : (optional, *positive integer*) The zoom level of the map when its first displayed on screen. Recommended range between 10 to 250. Defaults to 100.
- `cssClass` : (optional, *string*) A space separated list of classes to attach to the map for styling purposes.
- `_default` : (optional, *mapBlock object*) A `mapBlock` object which defines data to be used as a fallback for every block on the map, i.e., if no data is found for a specific block, it inherits the data of the default block.
- `r{R}c{C}` : (optional, *mapBlock object*) The `mapBlock` object which defines data for the block of the `R`*th row* & the `C`*th column*.

`mapBlock` objects are what make up the map. They hold inner properties of each block on the map. Each block can have *one* `mapBlock` object for itself, and is entirely optional. It is structured as follows:
- `name` : (optional, *string*) Text to be displayed as the name of the block the player is currently on.  
	(*See `1` in [In-game UI](library?id=ui)*)
- `desc` : (optional, *string*) Text to be displayed as the description of the block the player is currently on.  
	(*See `2` in [In-game UI](library?id=ui)*)
- `content` : (optional, *string*) SugarCube/HTML markup to be inserted inside the block. Recommended use-case: Images/Icons.  
	(*See `5` in [In-game UI](library?id=ui)*)
- `cssClass` : (optional, *string*) A space separated list of classes to attach to the block for styling purposes.
- `css` : (optional, *string*) Inline CSS to apply to the block. Use-case: Extremely-specific/One-time-only styling.
- `acts` : (optional, *string*) SugarCube/HTML markup to be displayed as the available-actions of the block the player is currently on. Recommended use-case: Links/buttons.  
	(*See `6` in [In-game UI](library?id=ui)*)
