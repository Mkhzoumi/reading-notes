# *charts*
+ ## *charts are used to display data visually, They’re easier to look at and convey data quickly.*
+ ## *chart.js is a javascript plugin that uses html5's canvas element to draw the graph onto a page.*
## *to use chart.js you have to download it and unzip it into the directory you esnt to use in, then creat an html page and import the script.*

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
```

## *Drawing a line chart:*

```
HtML
<canvas id="buyers" width="600" height="400"></canvas>

JAVASCRIPT
 var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);

var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```
# *usage of canvas element*

```
<canvas id="tutorial" width="150" height="150"></canvas>
```

## *canvas element looks like the img element yet canvas doesnt have src or alt attributes, canvas can take two attributes, width and height, and if we didnt spacify the width and height they will take a default value which is 300px X 150px.*

## *canvas only supports drowing rectangles and paths (list of points connected by lines).*

## *there are three functions to draw a rectangle:*
1. ## *fillRect(x, y, width, height): draw a filled rectangle.*
2. ## *strokeRect(x, y, width, height): Draws a rectangular outline.*
3. ## *clearRect(x, y, width, height): Clears the specified rectangular area making it fully transparent.*
## * x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle.*
## *ex:*

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}
```

![screen shot of rectangle](https://mdn.mozillademos.org/files/245/Canvas_rect.png)

## *drawing by path functions:*
+ ## *beginPath(): Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.*
+ ## *Path methods: Methods to set different paths for objects.*
+ ## *closePath(): Adds a straight line to the path, going to the start of the current sub-path.*
+ ## *stroke(): Draws the shape by stroking its outline.*
+ ## *fill(): Draws a solid shape by filling the path's content area.*

## *ex:*

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }
}
```

![triangle](https://mdn.mozillademos.org/files/9847/triangle.png)

## *moving the pen*
+ ## *moveTo(x, y): Moves the pen to the coordinates specified by x and y.*
+ ## *lineTo(x, y): Draws a line from the current drawing position to the position specified by x and y.*

## *ex:*

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    // Filled triangle
    ctx.beginPath();
    ctx.moveTo(25, 25);
    ctx.lineTo(105, 25);
    ctx.lineTo(25, 105);
    ctx.fill();

    // Stroked triangle
    ctx.beginPath();
    ctx.moveTo(125, 125);
    ctx.lineTo(125, 45);
    ctx.lineTo(45, 125);
    ctx.closePath();
    ctx.stroke();
  }
}
```

![two triangles](https://mdn.mozillademos.org/files/238/Canvas_lineTo.png)

## *you can also draw by using archs, and you can apply a style by changing the colors of the shapes.*








# [back](../README.md)