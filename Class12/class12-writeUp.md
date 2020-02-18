[Class12](https://cassandraortiz.github.io/reading-notes/Class12/class12)

# Canvas

the `<canvas></canvas>` element has only two attributes `height` and `weight`.  You are able to set the `id`.   When a height and weight is NOT SET, the default size is **300px wide and 150px high**.  CSS can set the size, but if hte aspect ration is next cosidered, the canvas may look distorted.

## Drawing on the Canvas

The canvas essentially is a grid that the 0,0 axis is the top-left corner of the canvas.

Canvas only supports *rectangle* and *paths* (lists of points connected by lines).

### Rectangles
you will need to reference the following to create a Rectangle: 

`(x, y, width, height)`

- `fillRect()` - Draws a filled rectangle
- `strokeRect()` - Draws a rectangular outline
- `clearRect()` - Clears the specified Rect area (transparent)

### Paths

A list of points connected by segments (curved and different widths), which could be open or closed.

- `beginPath()` - creates new path
- `moveTo(x,y)` - moves line to specific point
- `lineTo(x,y)` - creates line to next point
- `arc(x,y, radius, startAngle, endAngle, anticlockwise)` - creates an arc. 
- `closePath()` - creates a straight line to the beginning point
- `stroke()` - draws shape by stroking the outline
- `fill()` - draws a solid shape by filling the baths content area

``` JavaSript
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

### Path2D()

these constructors return a newly instantiated Path2D object.  All the MoveTo, Rect, arc etc. are all Path2d objects. 

## Colors

`fillStyle = color` Sets the style used when filling shapes.

`strokeStyle = color` Sets the style for shapes' outlines.

`createLinearGradient(x1, y1, x2, y2)`

### Line Styles

`lineWidth = value` Sets the width of lines drawn in the future.

`lineCap = type` Sets the appearance of the ends of lines (butt, round, square)

`lineJoin = type` Sets the appearance of the "corners" where lines meet (round, bevel, miter).

`miterLimit = value` Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

`getLineDash()` Returns the current line dash pattern array containing an even number of non-negative numbers.

`setLineDash(segments)` Sets the current line dash pattern.

`lineDashOffset = value` Specifies where to start a dash array on a line.


---

[HOME](https://cassandraortiz.github.io/reading-notes)