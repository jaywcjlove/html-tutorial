HTML canvas bezierCurveTo() 方法
===

## 示例

绘制三次贝塞尔曲线：

```html idoc:preview:iframe
<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;">您的浏览器不支持 HTML5 canvas 标签。</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.bezierCurveTo(20, 100, 200, 100, 200, 20);
ctx.stroke();
</script> 
```

JavaScript:

```js
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.moveTo(20, 20);
ctx.bezierCurveTo(20, 100, 200, 100, 200, 20);
ctx.stroke();
```

## 浏览器支持

![chrome][1] ![edge][2] ![firefox][3] ![safari][4] ![opera][5]

Internet Explorer 9、Firefox、Opera、Chrome 和 Safari 支持 bezierCurveTo() 方法。

## 定义和用法

bezierCurveTo() 方法通过使用表示三次贝塞尔曲线的指定控制点向当前路径添加一个点。

三次贝塞尔曲线需要三个点。 前两个点是三次贝塞尔计算中使用的控制点，最后一个点是曲线的终点。 曲线的起点是当前路径中的最后一个点。 如果路径不存在，请使用 [beginPath()](canvas_beginpath.md) 和 [moveTo()](canvas_moveto.md) 方法定义起点。

![三次贝塞尔曲线](../assets/img_beziercurve.gif)

起点 <i></i><!--rehype:style=display: inline-block; background: #ff9000; width: 9px; height: 9px;-->

```js
moveTo(20,20)
```

控制点 1 <i></i><!--rehype:style=display: inline-block; background: #FF0000; width: 9px; height: 9px;-->

```js
bezierCurveTo(20,100,200,100,200,20)
```

控制点 2 <i></i><!--rehype:style=display: inline-block; background: #FF0000; width: 9px; height: 9px;-->

```js
bezierCurveTo(20,100,200,100,200,20)
```

终点 <i></i><!--rehype:style=display: inline-block; background: #b0ef4e; width: 9px; height: 9px;-->

```js
bezierCurveTo(20,100,200,100,200,20)
```

**提示：** 查看 [quadraticCurveTo()](canvas_quadraticcurveto.md) 方法。它有一个控制点而不是两个。


| JavaScript 语法: | *context*.bezierCurveTo(*cp1x,cp1y,cp2x,cp2y,x,y*); |
| ----- | ----- |
<!--rehype:style=width: 100%; display: inline-table;-->

## 参数值

| 参数 | 描述 Description |
| ----- | ----- |
| *cp1x*    | 第一个贝塞尔控制点的 x 坐标 |
| *cp1y*    | 第一个贝塞尔控制点的 y 坐标 |
| *cp2x*    | 第二个贝塞尔控制点的 x 坐标 |
| *cp2y*    | 第二个贝塞尔控制点的 y 坐标 |
| *x*       | 结束点的 x 坐标 |
| *y*       | 结束点的 y 坐标 |
<!--rehype:style=width: 100%; display: inline-table;-->


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg