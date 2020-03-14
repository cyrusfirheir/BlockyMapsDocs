
## The Markup :id=markup

The default html of the drawn map is structured as follows (*Please note that these are the contents of the `bmPlayMap` passage after being rendered to the page*):

```html
<div id="map-container">
	<!-- the following #map portion is rendered by the setup.bm.drawMap() function -->
	<div id="map">
		<span id="r0c0" class="map-cell"></span>
		<span id="r0c1" class="map-cell"></span>
		<span id="r0c2" class="map-cell"></span>
		<!-- the rest of the blocks -->		
	</div>
</div>

<div id="map-ui">
	<div id="cur-block-name">
		<div class="content"></div>
	</div>
	<div id="cur-block-desc">
		<div class="content"></div>
	</div>
	<div id="cur-block-pos">
		<div class="content"></div>
	</div>
	<div id="cur-block-acts">
		<div class="content"></div>
	</div>
</div>
```
