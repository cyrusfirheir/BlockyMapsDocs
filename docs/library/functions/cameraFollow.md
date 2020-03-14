
### cameraFollow() :id=fn-camerafollow

`setup.bm.cameraFollow([target])`

Focuses the 'camera' on the specified target. Defaults to focusing on the very first block of the map.

**Since:**
- `v1.0.0`

**Parameters:**
- `target` : (optional, *string*) A CSS selector for the camera to target. Defaults to `"#r0c0"`, which is the first block of the map.

**Example:**
```js
// focusing on the player
setup.bm.cameraFollow(".player");
```
