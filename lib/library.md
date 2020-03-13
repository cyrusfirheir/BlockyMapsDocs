As mentioned earlier, map data is handled as a JSON object, and this allows for a lot of flexibility in regards to management of multiple maps.

The simplest map object might look something like this (*See [Map Object Template](lib/map-obj.md) for more details*):

```json
{
	"id": "uniqueMapID",
	"size": {
		"rows": 3,
		"cols": 3
	},
	"zoom": 1,
	"r1c1": {
		"cssClass": "player"
	}
}
```

Global Twine variables currently used by the library:  
- `$curMap` : (*object*) Map object which is currently being displayed.  
- `$curPos` : (*string*) Position of the player on the map.

{% hint style="info" %}  
**NOTE:** All library functions are under the `setup.bm` namespace.  
{% endhint %}
