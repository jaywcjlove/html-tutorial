HTML canvas fill() 方法
===

## 示例

绘制两个 150\*100 像素的矩形。 用红色填充一个，另一个用蓝色填充：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.rect(20, 20, 150, 100);
ctx.fillStyle = "red";
ctx.fill();

ctx.beginPath();
ctx.rect(40, 40, 150, 100);
ctx.fillStyle = "blue";
ctx.fill();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

ctx.beginPath();
ctx.rect(20, 20, 150, 100);
ctx.fillStyle = "red";
ctx.fill();

ctx.beginPath();
ctx.rect(40, 40, 150, 100);
ctx.fillStyle = "blue";
ctx.fill();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----- | --- | --- | --- | --- | --- |
| fill() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

`fill()` 方法填充当前图形（路径）。 默认颜色为黑色。

**提示：** 使用 [fillStyle](canvas_fillstyle.md) 属性填充另一种颜色/渐变。

**注意：** 如果路径没有闭合，`fill()` 方法会在路径的最后一点到起点添加一条线来闭合路径（如[closePath()](canvas_closepath.md)）， 然后填充路径。

| JavaScript 语法: | *context*.fill(); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg
