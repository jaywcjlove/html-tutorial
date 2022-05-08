HTML canvas arc() 方法
===

## 示例

创建一个圆圈：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(100, 75, 50, 0, 2 * Math.PI);
ctx.stroke();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(100, 75, 50, 0, 2 * Math.PI);
ctx.stroke();
```

## 浏览器支持

表中的数字指定了完全支持该属性的第一个浏览器版本。

| 方法 Method | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| arc()  | Yes | 9.0 | Yes | Yes | Yes |
<!--rehype:style=width: 100%; display: inline-table;-->

## 定义和用法

arc() 方法创建一个弧/曲线（用于创建圆或圆的一部分）。

**提示：** 使用 arc() 创建圆：将起始角度设置为 0，将结束角度设置为 2\*Math.PI。

**提示：** 使用 [stroke()](canvas_stroke.md) 或 [fill()](canvas_fill.md) 方法在画布上实际绘制弧线。

![一条弧线](../assets/img_arc.gif)

中心 <i></i><!--rehype:style=display: inline-block; background: #00ff00; width: 9px; height: 9px;-->

```js
arc(100,75,50,0 * Math.PI,1.5 * Math.PI)
```

起始角度 <i></i><!--rehype:style=display: inline-block; background: #ff0000; width: 9px; height: 9px;-->

```js
arc(100,75,50, 0 ,1.5 * Math.PI)
```

结束角度 <i></i><!--rehype:style=display: inline-block; background: #0000ff; width: 9px; height: 9px;-->

```js
arc(100,75,50,0 * Math.PI,1.5 * Math.PI)
```

| JavaScript 语法: | *context*.arc(*x,y,r,sAngle,eAngle,counterclockwise*); |
| ------- | ------- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *x*                | 圆心的 x 坐标 |
| *y*                | 圆心的 y 坐标 |
| *r*                | 圆的半径 |
| *sAngle*           | 起始角度，以弧度为单位（0 为圆弧的 3 点钟位置） |
| *eAngle*           | 结束角度，以弧度为单位 |
| *counterclockwise* | 选修的。 指定绘图应该是逆时针还是顺时针。 默认为 false，表示顺时针方向，而 true 表示逆时针方向。 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg