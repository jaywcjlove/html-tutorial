HTML canvas closePath() 方法
===

## 示例

画一条路径，形状为字母 L，然后画一条线回到起点：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.lineTo(20, 100);
ctx.lineTo(70, 100);
ctx.closePath();
ctx.stroke();
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.lineTo(20, 100);
ctx.lineTo(70, 100);
ctx.closePath();
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| closePath() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

closePath() 方法创建从当前点回到起点的路径。

**提示：** 使用 [stroke()](canvas_stroke.md) 方法在画布上实际绘制路径。

**提示：** 使用 [fill()](canvas_fill.md) 方法填充绘图（默认为黑色）。 使用 [fillStyle](canvas_fillstyle.md) 属性填充另一种颜色/渐变。

| JavaScript 语法: | *context*.closePath(); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 更多示例

使用红色作为填充颜色：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.lineTo(20, 100);
ctx.lineTo(70, 100);
ctx.closePath();
ctx.stroke();
ctx.fillStyle = "red";
ctx.fill();
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.lineTo(20, 100);
ctx.lineTo(70, 100);
ctx.closePath();
ctx.stroke();
ctx.fillStyle = "red";
ctx.fill();
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
