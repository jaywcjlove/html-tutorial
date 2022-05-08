HTML canvas rect() 方法
===

## 示例

绘制一个 150\*100 像素的矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML5 canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.rect(20, 20, 150, 100);
ctx.stroke();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.rect(20, 20, 150, 100);
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| rect() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`rect()` 方法创建一个矩形。

**提示：** 使用 [stroke()](canvas_stroke.md) 或 [fill()](canvas_fill.md) 方法在画布上实际绘制矩形。

| JavaScript syntax: | *context*.rect(*x,y,width,height*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x*       | 矩形左上角的 x 坐标 |
| *y*       | 矩形左上角的 y 坐标 |
| *width*   | 矩形的宽度，以像素为单位 |
| *height*  | 矩形的高度，以像素为单位 |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

使用 `rect()` 方法创建三个矩形：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// 红色矩形
ctx.beginPath();
ctx.lineWidth = "6";
ctx.strokeStyle = "red";
ctx.rect(5, 5, 290, 140);  
ctx.stroke();

// 绿色矩形
ctx.beginPath();
ctx.lineWidth = "4";
ctx.strokeStyle = "green";
ctx.rect(30, 30, 50, 50);
ctx.stroke();

// 蓝色矩形
ctx.beginPath();
ctx.lineWidth = "10";
ctx.strokeStyle = "blue";
ctx.rect(50, 50, 150, 80);
ctx.stroke();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// 红色矩形
ctx.beginPath();
ctx.lineWidth = "6";
ctx.strokeStyle = "red";
ctx.rect(5, 5, 290, 140);
ctx.stroke();

// 绿色矩形
ctx.beginPath();
ctx.lineWidth = "4";
ctx.strokeStyle = "green";
ctx.rect(30, 30, 50, 50);
ctx.stroke();

// 蓝色矩形
ctx.beginPath();
ctx.lineWidth = "10";
ctx.strokeStyle = "blue";
ctx.rect(50, 50, 150, 80);
ctx.stroke();
```

[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
