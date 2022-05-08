HTML canvas beginPath() 方法
===

## 示例

在画布上绘制两条路径； 一绿一紫：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.beginPath();              
ctx.lineWidth = "5";
ctx.strokeStyle = "green";  // Green path
ctx.moveTo(0, 75);
ctx.lineTo(250, 75);
ctx.stroke();  // Draw it

ctx.beginPath();
ctx.strokeStyle = "purple";  // Purple path
ctx.moveTo(50, 0);
ctx.lineTo(150, 130);            
ctx.stroke();  // Draw it
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.beginPath();
ctx.lineWidth = "5";
ctx.strokeStyle = "green"; // Green path
ctx.moveTo(0, 75);
ctx.lineTo(250, 75);
ctx.stroke(); // Draw it

ctx.beginPath();
ctx.strokeStyle = "purple"; // Purple path
ctx.moveTo(50, 0);
ctx.lineTo(150, 130);
ctx.stroke(); // Draw it
```

## 浏览器支持

表中的数字指定了完全支持该方法的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| beginPath() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`beginPath()` 方法开始一条路径，或重置当前路径。

**提示：** 使用 [moveTo()](./canvas_moveto.md)、[lineTo()](./canvas_lineto.md)、[quadricCurveTo()](./canvas_quadraticcurveto.md)、[bezierCurveTo()](./canvas_beziercurveto.md)、[arcTo()](./canvas_arcto.md) 和 [arc()](./canvas_arc.md) 创建路径。

**提示：** 使用 [stroke()](canvas_stroke.md) 方法在画布上实际绘制路径。

| JavaScript 语法: | *context*.beginPath(); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
