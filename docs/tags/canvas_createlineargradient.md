HTML canvas createLinearGradient() 方法
===

## 示例

定义从黑色到白色的渐变（从左到右），作为矩形的填充样式：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var grd = ctx.createLinearGradient(0, 0, 170, 0);
grd.addColorStop(0, "black");
grd.addColorStop(1, "white");

ctx.fillStyle = grd;
ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var grd = ctx.createLinearGradient(0, 0, 170, 0);
grd.addColorStop(0, "black");
grd.addColorStop(1, "white");

ctx.fillStyle = grd;
ctx.fillRect(20, 20, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| createLinearGradient() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

createLinearGradient() 方法创建一个线性渐变对象。

渐变可用于填充矩形、圆形、线条、文本等。

**提示：** 将此对象用作 [strokeStyle](canvas_strokestyle.md) 或 [fillStyle](canvas_fillstyle.md) 属性的值。

**提示：** 使用 [addColorStop()](canvas_addcolorstop.md) 方法指定不同的颜色，以及颜色在渐变对象中的位置。

| JavaScript 语法: | *context*.createLinearGradient(*x0,y0,x1,y1*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x0*      | 渐变起点的 x 坐标 |
| *y0*      | 渐变起点的 y 坐标 |
| *x1*      | 渐变终点的x坐标 |
| *y1*      | 渐变结束点的 y 坐标 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

定义渐变（从上到下）作为矩形的填充样式：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var my_gradient = ctx.createLinearGradient(0, 0, 0, 170);
my_gradient.addColorStop(0, "black");
my_gradient.addColorStop(1, "white");
ctx.fillStyle = my_gradient;
ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var my_gradient = ctx.createLinearGradient(0, 0, 0, 170);
my_gradient.addColorStop(0, "black");
my_gradient.addColorStop(1, "white");
ctx.fillStyle = my_gradient;
ctx.fillRect(20, 20, 150, 100);
```

定义从黑色到红色再到白色的渐变作为矩形的填充样式：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
您的浏览器不支持 HTML5 canvas 标签。
</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var my_gradient = ctx.createLinearGradient(0, 0, 170, 0);
my_gradient.addColorStop(0, "black");
my_gradient.addColorStop(0.5 ,"red");
my_gradient.addColorStop(1, "white");
ctx.fillStyle = my_gradient;
ctx.fillRect(20, 20, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var my_gradient = ctx.createLinearGradient(0, 0, 170, 0);
my_gradient.addColorStop(0, "black");
my_gradient.addColorStop(0.5 ,"red");
my_gradient.addColorStop(1, "white");
ctx.fillStyle = my_gradient;
ctx.fillRect(20, 20, 150, 100);
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg