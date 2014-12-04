# Pointerest

Show the key features of your product using elegant points

---

#### Demo example
http://ayoubgdah.github.io/pointerest/

#### How to use the plugin

- Add jQuery
```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
```
- Add the javascript for the file: ***pointerest.js***
```html
<script src="pointerest.js"></script>
```
- Add the CSS file: ***pointrerest.css***
```html
<link rel="stylesheet" href="pointerest.css">
```
- Setup your markup and add the points
```html
	<div class="container">
		<span class="point" data-x="280" data-y="200" data-content="Keep your house warm and your wallet full"></span>
		<span class="point" data-direction="left" data-color="#4AA3DF" data-x="550" data-y="200" data-content="A better understanding of water consumption"></span>
		<span class="point" data-x="820" data-y="200" data-content="Save energy and money"></span>
		<span class="point" data-x="900" data-y="910" data-content="Pay whenever you are ready"></span>
		<span class="point" data-x="750" data-y="350" data-content="Shows you if you have saved or should do better"></span>
		<span class="point" data-x="850" data-y="530" data-content="Hourly, daily, and monthly reporting"></span>
	</div>
```
Attribute | Description
--- | ---
data-x | left position of the point
data-y | top position of the point
data-direction | direction the line should go
data-color | color to be applied to the point
data-content | the content related to the point
- Fire up the plugin with:
```javascript
$(".container").Pointerest();
```

#### Plugin Options
Option | Default | Description
--- | --- | ---
radius | 10 | The radius of the point in px
color | #333 | The color of the points, could be any css valid color (i.e #ffff, rbg(255, 255, 255), rgba ...).
lineHeight | 2 | The height of the line that goes from the point to the text in px.
direction | null | Which direction the line goes to. It could be right or left. If nothing is provided then it is based on the nearest side.
margin | 20 | The distance between the text and the container. So far only left and right are supported.
animationSpeed | 300 | The speed of the animations: width of the line and text showing.
