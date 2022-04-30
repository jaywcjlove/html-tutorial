HTML 画布图形
===

HTML \<canvas> 元素用于在网页上绘制图形。

左边的图形是用 \<canvas> 创建的。 它显示四个元素：红色矩形、渐变矩形、多色矩形和多色文本。

## 什么是 HTML 画布？

HTML `<canvas>` 元素用于通过 JavaScript 动态绘制图形。

`<canvas>` 元素只是图形的容器。 您必须使用 JavaScript 来实际绘制图形。

Canvas 有多种方法用于绘制路径、框、圆、文本和添加图像。

## 浏览器支持

表中的数字指定了第一个完全支持 `<canvas>` 元素的浏览器版本。

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ---- | ---- | ---- | ---- | ---- | ---- |
| \<canvas> | 4.0 | 9.0 | 2.0 | 3.1 | 9.0 |

## Canvas 示例

画布是 HTML 页面上的一个矩形区域。 默认情况下，画布没有边框，也没有内容。

标记如下所示：

```html idoc:preview
<canvas id="myCanvas1" width="200" height="100"></canvas>
```

**注意：** 始终指定一个 `id` 属性（在脚本中引用），以及一个 `width` 和 `height` 属性来定义画布的大小。 要添加边框，请使用 `style` 属性。

这是一个基本的空画布示例：

```html idoc:preview:iframe
<canvas id="myCanvas2" width="200" height="100" style="border:1px solid #000000;"></canvas>
```
<!--rehype:style=min-height: 120px;-->

## 添加一个 JavaScript

创建矩形画布区域后，您必须添加 JavaScript 来进行绘图。

这里有些例子：

### 画一条线

```html idoc:preview:iframe
<canvas id="myCanvas3" width="200" height="100"></canvas>
<script>
  var c = document.getElementById("myCanvas3");
  var ctx = c.getContext("2d");
  ctx.moveTo(0, 0);
  ctx.lineTo(200, 100);
  ctx.stroke();
</script>
```
<!--rehype:style=min-height: 120px;-->

### 画一个圆

```html idoc:preview:iframe
<canvas id="myCanvas4" width="200" height="100"></canvas>
<script>
var c = document.getElementById("myCanvas4");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
</script>
```
<!--rehype:style=min-height: 120px;-->

### 绘制文本

```html idoc:preview:iframe
<canvas id="myCanvas5" width="200" height="100"></canvas>
<script>
var c = document.getElementById("myCanvas5");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
</script>
```
<!--rehype:style=min-height: 120px;-->

### 描边文字

```html idoc:preview:iframe
<canvas id="myCanvas6" width="200" height="100"></canvas>
<script>
var c = document.getElementById("myCanvas6");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World", 10, 50);
</script>
```
<!--rehype:style=min-height: 120px;-->

### 绘制线性渐变

```html idoc:preview:iframe
<canvas id="myCanvas7" width="200" height="100"></canvas>
<script>
var c = document.getElementById("myCanvas7");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createLinearGradient(0, 0, 200, 0);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
</script>
```
<!--rehype:style=height: 120px;-->

### 绘制圆形渐变

```html idoc:preview:iframe
<canvas id="myCanvas" width="200" height="100"></canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
</script>
```
<!--rehype:style=height: 120px;-->

### 绘制图像

```html idoc:preview:iframe
<img id="scream" src="../assets/example.png" alt="The Scream" />
<canvas id="myCanvas" width="250" height="300"></canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  var img = document.getElementById("scream");
  console.log(img, c)
  ctx.drawImage(img, 10, 10);
</script>
```
<!--rehype:style=height: 420px;-->
