HTML canvas createRadialGradient() 方法
===

## 示例

绘制一个矩形并填充径向/圆形渐变：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML5 canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 100);
</script>
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 100);
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ----------- | --- | --- | --- | --- | --- |
| createRadialGradient() | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

createRadialGradient() 方法创建一个径向/圆形渐变对象。

渐变可用于填充矩形、圆形、线条、文本等。

**提示：** 将此对象用作 [strokeStyle](canvas_strokestyle.md) 或 [fillStyle](canvas_fillstyle.md) 属性的值。

**提示：** 使用 [addColorStop()](canvas_addcolorstop.md) 方法指定不同的颜色，以及颜色在渐变对象中的位置。

| JavaScript 语法: | *context*.createRadialGradient(*x0,y0,r0,x1,y1,r1*); |
| ----------- | ----------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x0*      | 渐变起始圆的 x 坐标 |
| *y0*      | 渐变起始圆的 y 坐标 |
| *r0*      | 起始圆的半径 |
| *x1*      | 渐变结束圆的 x 坐标 |
| *y1*      | 渐变结束圆的 y 坐标 |
| *r1*      | 结束圆的半径 |
<!--rehype:style=width: 100%; display: inline-table;-->



[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg