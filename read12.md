[**HOME**](https://mousasbbah.github.io/reading-notes/)

# HTML Canvas


## **What is HTML Canvas?**
The HTML `<canvas>` element is used to draw graphics, on the fly, via JavaScript.

The `<canvas>` element is only a container for graphics. You must use JavaScript to actually draw the graphics.

Canvas has several methods for drawing paths, boxes, circles, text, and adding images.


<br>
<hr>
A canvas is a rectangular area on an HTML page. By default, a canvas has no border and no content.

The markup looks like this:

```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```



## **Drawing paths**

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:


First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

`beginPath()`

Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.

`closePath()`

Adds a straight line to the path, going to the start of the current sub-path.

`stroke()`

Draws the shape by stroking its outline.

`fill()`

Draws a solid shape by filling the path's content area.


## **Add a JavaScript**
After creating the rectangular canvas area, you must add a JavaScript to do the drawing.

Here are some examples:

### **Draw a Line**

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.moveTo(0, 0);
ctx.lineTo(200, 100);
ctx.stroke();
```

**RESULT :**

![line](/image/line.png)

### **Draw a Circle**

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
```
**RESULT :**

![circle](/image/circule.png)

### **Draw a Text**

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
```

**RESULT :**

![drawText](/image/drawtext.png)

[**HOME**](https://mousasbbah.github.io/reading-notes/)